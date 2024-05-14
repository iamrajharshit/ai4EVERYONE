# Week 1 (What is AI?)

## Content Index
|Topic|Description|
|--|--|
|[Introduction](#Introduction)||
|[Machine Learning](#Machine-Learning)||
|[What is Data?](#What-is-Data?)||
|[The terminology of AI](#The-Terminology-of-AI)||
|[What ML can and cannot do](#What-ML-can-and-cannot-do)||

## Introduction
###  Artificial intelligence (AI), three key concepts shape its evolution and impact:

- **Artificial Narrow Intelligence (ANI):** ANI refers to AI systems tailored for specific tasks or narrow domains. These systems excel in performing predefined tasks but lack adaptability beyond their designated scope. Examples include virtual assistants like Siri and recommendation algorithms.

- **Generative AI (Gen AI):** Gen AI encompasses AI technologies capable of generating new content, such as text, images, or audio, indistinguishable from human-generated content. This includes models like GPT (Generative Pre-trained Transformer) and image generators like DALL-E.

- **Artificial General Intelligence (AGI):** AGI represents the aspirational goal of creating AI systems with human-like cognitive abilities, capable of performing any intellectual task a human can. Unlike ANI, AGI exhibits general intelligence, enabling learning, reasoning, and adaptation across various tasks and contexts.

## Machine Learning
Machine learning is a subset of artificial intelligence (AI) that focuses on the development of algorithms and models that enable computers to learn and improve from experience without being explicitly programmed. In traditional programming, a human programmer writes rules and instructions that direct the computer's behavior. In contrast, in machine learning, the computer learns patterns and insights directly from data.
### Supervised Learning

In supervised learning, the algorithm is trained on labeled data, where each example in the dataset is associated with a corresponding target label. The goal is to learn a mapping from input features to output labels.
<img src="img\week1\ml examples.jpg">

The most commonly used type of machine learning, where the AI learns input-output mappings (A to B).
- Examples include spam filtering, speech recognition, machine translation, and more.

#### How LLMs works

- Training Data: LLMs are trained on massive datasets containing billions or even trillions of words. These datasets are collected from various sources on the internet and serve as the basis for teaching the model how language works and how words relate to each other.

- Supervised Learning: During the training process, the LLM is presented with sequences of text as input and is tasked with predicting the next word in each sequence. This process is a form of supervised learning, where the input-output pairs (sequences of words and their subsequent words) serve as training examples.

- Pattern Recognition: As the LLM processes more and more text data during training, it learns to recognize patterns and correlations between words. By analyzing the context of each word within a sequence, the model can make probabilistic predictions about which word is likely to come next.

- Generative Capability: Once trained, the LLM can generate new text by providing it with an initial prompt or seed text. The model uses its learned knowledge about language and word relationships to predict and generate the next words in the sequence, effectively continuing the text based on the input it receives.

- Fine-tuning and Specialization: LLMs can be fine-tuned on specific tasks or domains by further training them on smaller, domain-specific datasets. This process helps tailor the model's language generation capabilities to particular applications or contexts, making it more effective for tasks like summarization, translation, or dialogue generation.

<img src="img\week1\llms.jpg">


 The idea of supervised learning has been around for many decades, but it's really taken off in the last few years. Why is this?
<img src="img\week1\perf vs amt data.jpg">
There's a picture I draw for them and I want to show you this picture now. You may be able to draw this picture for others that ask you the same question as well. Let's say on the horizontal axis, you plot the amount of data you have for a task. For speech recognition, this might be the amount of audio data and transcripts you have. In a lot of industries, the amount of data you have access to has really grown over the last couple of decades. Thanks to the rise of the Internet, the rise of computers. A lot of what used to be, say, pieces of paper are now instead recorded on a digital computer. We've just been getting more and more and more data.

- Traditional AI system performance get constant
- With complex NN performance gets better!

For applications like speech recognition, online advertising, building self-driving car, where having a high performance, highly accurate say speech recognition system is important, this has enable these AI systems get much better and make, say, speech recognition products much more acceptable to users, much more valuable to companies and to users.

- We need Big DATA and good GPUs to train large NN for better performance.

### Unsupervised Learning 
In unsupervised learning, the algorithm is given unlabeled data and must find patterns and structures within the data on its own. This can include tasks such as clustering similar data points together or dimensionality reduction.

### Reinforcement Learning
Reinforcement learning involves training an agent to interact with an environment in order to achieve a goal. The agent learns through trial and error, receiving feedback in the form of rewards or penalties based on its actions.

### Semi-supervised Learning
Semi-supervised learning combines elements of supervised and unsupervised learning, where the algorithm is trained on a combination of labeled and unlabeled data.

### Deep Learning
Deep learning is a subset of machine learning that uses neural networks with many layers (deep architectures) to learn intricate patterns in large amounts of data. Deep learning has shown remarkable success in various tasks such as image recognition, natural language processing, and speech recognition.



## What is Data?


## The terminology of AI


## What ML can and cannot do


