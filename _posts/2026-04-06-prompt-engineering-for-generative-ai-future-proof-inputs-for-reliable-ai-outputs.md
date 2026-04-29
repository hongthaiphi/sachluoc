---
layout: default
title: "Prompt Engineering for Generative AI – Future-Proof Inputs for Reliable AI Outputs"
date: 2026-04-06
published: true
---

*Author: **James Phoenix***

_James Phoenix_

Reading time: 20 minutes

### Synopsis

*Prompt Engineering for Generative AI* (2024) is a complete guide to using AI that creates text and images. It explains five main rules for making good prompts. These rules help you use large language models like ChatGPT and image models like Stable Diffusion. The book also looks at how these AI models work. It gives many useful tips to help you use AI better.

## What’s in it for me? Learn to give good instructions to AI.

AI models that create things are improving very quickly every day. They change so fast it’s hard to follow. 

But we need to keep learning. One thing is certain: AI will stay. As AI changes, jobs will change too. It will be used in many more jobs in the future. 

However, AI cannot read your mind – at least, not yet. It will not always give you what you want. In fact, it will often make things up with great confidence. This is called *hallucination*. The results you get from AI depend on the quality of your instructions. 

So, you need to be able to create good instructions. This skill is called *prompt engineering*. It will likely be needed for many jobs in the future. It will be like being good at Microsoft Excel today. 

Luckily, the authors have used AI that creates things since 2020, when it was new. They have found good ways to work. These are rules that have worked well with old AI models and new ones. This summary will explain these rules. 

The authors’ book shows many ways to give prompts. Many of these need you to write code in Python. In this summary, we will talk about what you can do with simple English. But don’t worry – the same rules for prompt engineering work for all types of prompts. 

So, let's start. Let's look at the big book of AI tips.

## Blink 1 - Three rules for good AI prompts

Let’s start with a simple prompt: “Can you give me a list of names for shoes that will fit any size?” If you put this into a Large Language Model like ChatGPT, it will give you names like OmniFit or Universole.

This is already very impressive. But if you want to use AI for more than just fun, you need to be more exact. This is where the *five rules for prompt engineering* come in. These rules always work, say the authors. They work for humans and for AI. 

The first rule is to always *give clear instructions*. Simply put, the more details you give, the more likely the AI will give you what you want. 

A good way to do this is by using a method called *prewarming*, or *internal retrieval*. For example, with the shoe names, you would first ask your AI model for a full list of tips for naming products, using expert ideas. Then, you would ask your AI for product names, using the advice it just gave you. 

Giving clear instructions is also important for AI models that create images. If you ask for an image of "a business meeting around a round glass table," you will get a more exact image. This is better than just asking for "a business meeting." But be careful: if you are too specific, the AI might get ideas that don't fit together. Then it won't know what to do.

The second rule for prompts is about *telling the AI what format to use*. AI models can give you information in almost any style. This could be a language like French, or a computer format like JSON or Python. Image AI can create many kinds of images, like stock photos, oil paintings, mosaics, or even Minecraft pictures. 

But if you don’t say what format you want, it’s less likely you will get it. If you are using AI in programs you build, you must be very careful to say what format you need. Small changes can cause many problems.

To make sure you get the right results, use the third rule for prompt engineering: *give examples*. Prompts without examples are called *zero-shot* prompts. If you add one example, it’s a *one-shot prompt*. If you add more than one, it’s a *few-shot prompt*. The more examples you give, the more you can guess what the AI will create. But remember, you have to choose between getting reliable results and getting creative ones. If you give too many examples that are all very similar, your AI cannot give you new or unexpected ideas.

## Blink 2 - Two more rules for prompts

Let’s now look at the fourth rule for prompts: *check the results*. For prompts you use only once, just trying different things until it works is usually fine. This is called *blind prompting*. But if you will use your prompt many times, or if you build a program with it, you need to do more. 

Often, the way to check results is simple: a 'good' or 'bad' rating. Choose some prompts you want to test. Give each prompt to your AI model many times. Then, put all the results next to each other in a table. Mark them with a 'good' or 'bad' sign. If you want to be more exact, you can use a number score instead. You can also use a computer program to do this, but we won't explain how here. 

You can check images in the same way, using a method called *permutation prompting*. This means you give your AI model many prompts. Each prompt has different instructions and styles. Then you put all the images the AI made next to each other to compare them. This helps you see what works best for the future.

Alright – we’ve now come to the fifth and last rule for prompts. This is about *splitting up the work*. Think of it this way: when you put more things into your prompt, you ask the AI to do too much at once. Prompts with too many details can be too much for the AI. This can cause more hallucinations and strange results.

That’s when *breaking down tasks* becomes important. Just like with humans, breaking big tasks into smaller, easier parts for AI can get better results. It also lets you see which parts work well and which don’t. Even adding the words “let’s think step by step” to your prompt can help a lot. This is a key part of something called *chain of thought reasoning*.

You can even split the work between text AI and image AI. You already have names for shoes that fit any size. Now ask your text AI to give you a full description of those shoes. Then you can use that description as a prompt for your image AI. This will create a good image for your product.

So, those are the five rules for prompts. They have worked well for a long time, so far. Yes, the newest technology today might be old in a few months. But the authors are sure that these rules will always help you get what you want from your AI models.

## Blink 3 - How Large Language Models (LLMs) work

It's a common idea that you can use something better if you understand how it works. So, let's now try to understand large language models, or LLMs.

It all starts with something called a *token*. This is the basic part in natural language processing (NLP). Tokens can be sentences, words, or even small parts of words. To give you an idea of size, 100 tokens are about 75 words long. 

Why are tokens important? To get text ready for NLP, LLMs first need to do *tokenization*. This means they turn text into tokens. A common method is *byte-pair encoding*, or BPE. This process builds a list of words by seeing how often letters or groups of letters appear. It starts with single letters. Then it joins together the letters that appear next to each other most often, again and again. For example, the common group "c", "a", and "t" (which spells "cat") becomes one token. This way, the LLM is very flexible. It remembers common words as full units. But it can also understand new or rare words by putting together these smaller, known parts.

After turning them into tokens, these units are changed into lists of numbers. These are called *vectors*, or *word embeddings*. These numbers show both how a word is built and what it means. When the LLM learns, it places these numbers onto a very big, complex map. Words with similar meanings, like “swimming” and “swam,” or “immoral” and “sin,” appear close to each other on this map. This closeness helps the AI understand how ideas are linked.

The main part that works with these numbers is the *transformer*. Its most important part is called *self-attention*. This lets every word in a sentence look at every other word at the same time. This makes sure the AI understands the full meaning, not just words in order.

So, that’s how LLMs understand text. But how do they generate their own words?

It all comes down to chances. Simply put, the AI works out which token is most likely to come next after the words it already has. Then it chooses the most likely token. It adds this new token to the previous ones and repeats the process. It sends the text through the transformer to create the next token. This goes on until the AI has finished its answer.

Alright – that’s how LLMs work. Now, let’s look at some ways to use them best. 

## Blink 4 - Easy ways to create text with AI

Before you can give your LLM a prompt, you need to choose which one to use. There are many models, each with its own design, good points, and bad points. You have the main ones like OpenAI’s ChatGPT, Anthropic’s Claude, and Google’s Gemini. But there are also smaller models like Meta’s Llama and Mistral, from the French company Mistral AI.

The best way is to give the same prompt to a few different LLMs. Then see which result works best for your exact need. 

A warning: keeping your data private is important when using any of these models. If the models use your own data to learn or get better, be careful. Do not put in any private information.

Once you have chosen your model, there are a few simple methods that can help you use them best. This is especially true when you use them with the five prompt rules you learned earlier.

One of these methods is called *text style unbundling*. This means you ask your AI model to find the main parts of a text. This could be its feeling, its words, or how it is built. This can be very useful for creating new text that still sounds like your brand. Or you can change old text to new styles or forms, but keep the main idea. 

One way to unbundle a text style is to say exactly what parts you want to find. Then ask your AI model to look at the text for those parts. Another way is to use *meta prompting*. This is when you make a prompt that then makes another prompt. For example, you could ask your AI to look at a text and find its main features. Then you can copy those features. The AI would then give you these features as a writing guide. You could use this guide for future documents. You could then add this writing guide to your next prompts for creating text.

Another type of meta prompting is asking your AI to make an old prompt better. This is to reach a certain aim. For example, you could ask your AI to look at your writing guide and make it better. This would help all your texts sound the same for your brand.  

*Role prompting* also helps you keep the same style in all results. This means you tell your AI to act like a certain person or character. For example, you could ask your AI to act like a tech reviewer. Or it could copy how famous people like Donald Trump speak.

Besides keeping your brand style, role prompting can help your AI give you different ideas on a topic. Or it can add some humor to your results to make them more interesting for users. Just make sure to always check what your AI creates. It can slowly stop acting like its role over time.

## Blink 5 - How image generation works

They say a picture is worth a thousand words. Well, with AI, you can generate thousands of pictures with just a few words. But how exactly does it work?

The most popular AI models that create images from text are called *diffusion models*. As of late 2025, these include OpenAI’s GPT Image, Google’s Nano Banana, and free and open models such as Stable Diffusion.

When learning, diffusion models take a clear image and slowly make it blurry by adding random dots, called *noise*. They do this until the image is just a blur. Then, they learn to undo this. They clean up the fuzz step-by-step to get the clear picture back. A text description helps them clean it up. If the picture doesn't match the description, the AI fixes it. This happens billions of times. Once trained, the AI can take a square of random fuzz and make it into a detailed image based on your instructions.

This process teaches the AI how objects and styles look. It saves these looks as lists of numbers, or vectors. This is like how LLMs save words. These vectors show exact places in a *latent space*. This is a very big, complex map where the AI stores every image idea it can make.

When you give the AI a text prompt, it changes your words into these number places. It creates the image that is at that place on the map. Finally, it turns that information into pixels for your screen.

There are many diffusion models, and each is good at different things. Just like with text models, the best way to choose is to use the same prompt with different models and compare the results. 

## Blink 6 - Ways to create images

We’ll finish with some useful tips for creating images. A good tool when using diffusion models is *reverse engineering prompts*. Sometimes you know what image you want, but you don't know how to describe it with words. Luckily, models like Image GPT and Nano Banana let you upload an image and ask the AI to describe it. You can then take this description and change it a little to get the image you want.

You can also include *words that make images better* in your prompt. These are simple words like “beautiful,” “high resolution,” or “trending on ArtStation.” You can add them to your prompt to make the image better.

*Negative prompting* is when you tell your AI what to avoid. For example, if you say “Tom and Jerry, no cartoon,” you would get a real-looking picture of the two famous characters.

If you want to be more exact with your prompts, some models let you give more importance (*weights*) to certain words. All words in a prompt usually have a weight of 1. However, words at the start of the prompt are more important. You can clearly change this to get special results. In models like Midjourney, you do this by adding two semi-colons and a number. This number shows how important you want it to be, with no spaces. For example, you could write: “painting of Tom and Jerry, in the style of Rembrandt::0.8, in the style of Pollock::0.2.” This would give you a painting mostly like Rembrandt but also a little like Pollock.

You can create endless prompts. As AI keeps changing, new choices will appear. But with the rules you’ve learned in this summary, you’ll be ready to use new AI tools very well.

## Final summary

The main idea of this summary of *Prompt Engineering for Generative AI* by James Phoenix and Mike Taylor is this: you can use AI that creates text and images very well. To do this, follow five important rules for prompt engineering. These are: give clear instructions, say what format to use, give examples, check results, and split up the work. 

You’ve also learned how large language models work, and some simple ways to use them best. Then, we looked at how diffusion models work, and the best ways to use them. With all this information, you can now understand and use the changing world of AI that creates things, with confidence. 

Okay, that’s it for this Blink. We hope you enjoyed it. If you can, please take the time to leave us a rating – we always appreciate your feedback. See you in the next Blink.

Source: https://www.blinkist.com/https://www.blinkist.com/en/books/prompt-engineering-for-generative-ai-en