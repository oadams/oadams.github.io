---
layout: post
title:  "Imagen and Meaning"
date:   2022-06-11 00:00:00 +1000
categories: machine-learning
---
Imagen is a new state of the art text-image model. [Website](https://imagen.research.google/). [Paper](https://arxiv.org/abs/2205.11487).

The most interesting aspect of it for me is the effect that using a large pre-trained language model (T5) for the text encoder has. They keep the weights of the encoder frozen and they find that bigger language models lead to better performance in text to image alignment and image fidelity. I have no idea why the language model size is important for image fidelity, but on the text&ndash;image alignment side it makes sense that a larger language model would make the model better at dealing with richer descriptions of the scene to be generated. In particular, they find that such models were better at ‘encoding complex and compositional text prompts’.

This immediately reminded me of the debate regarding form and meaning in large language models and the article [To Dissect an Octopus](https://julianmichael.org/blog/2020/07/23/to-dissect-an-octopus.html) by Julian Michael that we looked at in the ML reading group at work some time ago. Specifically, the article pushed back against the argument that language models can’t glean meaning from text alone. The argument it pushes back against is essentially this: since text is just a sequence of symbols and isn’t grounded or contextualized in the real world, the underlying meaning simply cannot be accessed and therefore language models can’t learn meaning or ‘understand’ anything. Julian makes a convincing counterargument using the example of an Octopus that lives deep underwater and never sees color but learns all about where each color word sits in terms of lightness, darkness, warmth, coolness, saturation, and washed-outness. The octopus then rises from the deep, sees one example of a color and is immediately able to ground its whole vast lexicon of colors.

> This raises the question: When, or from where, did O learn the meaning of the word “lavender”? It’s hard for me to accept any answer other than “partly underwater, and partly on land.”

Imagen seems in some ways to be a concrete instantiation of this argument. By analogy the frozen language model is the purely text-based knowledge the octopus has prior to any exposure to images. The text-image modeling component on the other hand is like the octopus’s first exposure to color. The paper indicates that the overall model does better because it has a bigger language model. For example, Imagen did better than DALL-E 2 at correctly understanding subject&ndash;object relationships in some settings. See the example images below generated from the prompt ‘a panda making latte art’. The four images on the left are from Imagen, the four on the right from DALL-E 2. When, or from where, did the model learn the meaning of the word ‘make’ and the associated subject&ndash;object relationship? It’s hard for me to accept any answer other than “partly from pure text, partly from text&ndash;image mappings”.

<div style="text-align:center"><img src ="https://oadams.github.io/pandas.png"/></div>
