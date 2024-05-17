# Week 1 (What is AI?)

## Content Index
|Topic|Description|
|--|--|
|[Introduction](#Introduction)||
|[Machine Learning](#Machine-Learning)||
|[What is Data?](#What-is-Data)||
|[The Terminology of AI](#The-Terminology-of-AI)||
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

### How LLMs works

- **Training Data:** LLMs are trained on massive datasets containing billions or even trillions of words. These datasets are collected from various sources on the internet and serve as the basis for teaching the model how language works and how words relate to each other.

- **Supervised Learning:** During the training process, the LLM is presented with sequences of text as input and is tasked with predicting the next word in each sequence. This process is a form of supervised learning, where the input-output pairs (sequences of words and their subsequent words) serve as training examples.

- **Data Representation:** Each sentence in the training data is turned into multiple input-output pairs (A to B data points). For example, given the sentence "my favorite drink is lychee bubble tea," the model learns to predict the next word after phrases like "my favorite drink" or "is lychee."

- **Pattern Recognition:** As the LLM processes more and more text data during training, it learns to recognize patterns and correlations between words. By analyzing the context of each word within a sequence, the model can make probabilistic predictions about which word is likely to come next.

- **Generative Capability:** Once trained, the LLM can generate new text by providing it with an initial prompt or seed text. The model uses its learned knowledge about language and word relationships to predict and generate the next words in the sequence, effectively continuing the text based on the input it receives.

- **Fine-tuning and Specialization:** LLMs can be fine-tuned on specific tasks or domains by further training them on smaller, domain-specific datasets. This process helps tailor the model's language generation capabilities to particular applications or contexts, making it more effective for tasks like summarization, translation, or dialogue generation.

<img src="img\week1\llms.jpg">


 The idea of supervised learning has been around for many decades, but it's really taken off in the last few years. Why is this?
<img src="img\week1\perf vs amt data.jpg"><br>
I want to show you this picture now. Let's say on the horizontal axis, you plot the amount of data you have for a task. For speech recognition, this might be the amount of audio data and transcripts you have. In a lot of industries, the amount of data you have access to has really grown over the last couple of decades. Thanks to the rise of the Internet, the rise of computers. A lot of what used to be, say, pieces of paper are now instead recorded on a digital computer. We've just been getting more and more and more data.

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



## What is Data

<img src="img\week1\data.jpg"><br>
- **Data set:** A collection of data organized in a table format, similar to an Excel spreadsheet.
- **Machine learning input (A):** The features or attributes used to train the model.
- **Machine learning output (B):** The target variable the model is trying to predict.
- **Defining A and B:** Depends on the specific business use case.
- **Examples:**
    - Real estate pricing: A - house size and number of bedrooms, B - house price.
    - House affordability: A - budget, B - affordable house size.
    - Cat image recognition: A - image, B - label (cat or not).

**Trivia:** *Cats are popular in machine learning! It seems to have started with a project where a Google AI system learned to identify cats by watching YouTube videos. This led to a funny and enduring tradition of using cats as examples when explaining machine learning concepts.*  

### Acquiring Data

<img src="img\week1\acquiring data.jpg"><br>
The different ways to acquire data for machine learning:

- **Manual Labeling:**
Manually label data points (e.g., identifying cats in pictures).
Time-consuming but ensures high-quality data (A and B are clear).
- **Observing User/Machine Behavior:**
Collect data from user interactions (e.g., purchases on an e-commerce site).
Analyze user behavior (A) to predict outcomes (B) (e.g., product purchase).
Similar approach can be used for machine behavior (e.g., sensor data from a factory machine to predict failures).
- **Downloading Public Datasets:**
Wide variety of datasets available online (image recognition, self-driving cars, etc.).
Free and easy to access, but consider licensing and copyright restrictions.
- **Partnering with Data Providers:**
Collaborate with companies that have relevant data (e.g., factory machine data).
Leverage existing data collections for your machine learning project.

### Use-Mis use of Data
common misuses of data for machine learning
<img src="img\week1\mis use.jpg"><br>

- **Misuse 1: Waiting for Perfect Data**

- Some companies believe they need a massive, perfect dataset before using AI.
- This is wrong! Early collaboration between IT and AI teams is crucial.
- AI teams can analyze initial data and suggest improvements to data collection (e.g., frequency, type).
- This iterative approach helps refine data collection and build better AI systems.
- **Misuse 2: Assuming More Data Equals More Value**

- Simply having a lot of data doesn't guarantee success with AI.
- Don't throw data at an AI team and expect magic.
- The quality and relevance of the data matter more than just quantity.
- Similarly, acquiring data without a plan for its use can be wasteful.
- Focus on getting the right data, not just the most data. AI teams can help identify the most valuable data for your specific needs.

### Data is Messy
Messy data, also referred to as dirty data, is a common challenge in machine learning. It refers to data that is inaccurate, incomplete, inconsistent, or improperly formatted. This can significantly impact the performance of your AI system, leading to inaccurate predictions and unreliable results.
<img src="img\week1\messy data.jpg"><br>

**Types of Messy Data:**

- **Incorrect labels:** This occurs when data points are labeled inaccurately. For example, a house price listed as $0.001 is likely a typo.
- **Missing values:** Data points might be missing entirely, leaving gaps in your dataset. This could be due to faulty sensors, human error during data entry, or incomplete records.
- **Inconsistent formatting:** Data might be presented in different formats within the same dataset. For instance, house sizes could be listed in square feet and square meters without standardization.
- **Outliers:** Extreme values that deviate significantly from the rest of the data can distort the overall picture. Imagine a dataset of house prices with one mansion listed for a billion dollars, skewing the average price.
- **Duplicates:** The same data point might be present multiple times in your dataset, inflating its importance and potentially leading to biased results.

**Impacts of Messy Data:**

- **Reduced accuracy:** Training an AI system on messy data leads to inaccurate learning and unreliable predictions. For example, a system trained on incorrect house prices wouldn't be able to accurately estimate future home values.
- **Biased results:** Inconsistent data or missing values can lead to biased models that favor certain outcomes. Imagine a loan approval system trained on data with fewer entries for minorities, potentially leading to biased decisions.
- **Wasted resources:** Time and effort spent training a model on low-quality data is wasted. Cleaning the data beforehand can save resources and improve the overall efficiency of your project.
Dealing with Messy Data:

Techniques to address messy data:

- **Data Cleaning:** This involves identifying and correcting errors, filling in missing values, and standardizing formats. This can be done manually or through automated tools.
- **Data Validation:** Establishing data quality checks and validation rules can help prevent messy data from entering your system in the first place.
Data Imputation: Techniques like averaging or using statistical methods can fill in missing values with estimations.
- **Outlier Detection and Handling:** Identifying and potentially removing outliers or handling them through specific techniques can prevent them from distorting the results.
- **Data Transformation:** Transforming data into a format suitable for your AI model might involve scaling, normalization, or feature engineering.

*Data quality is paramount for successful AI projects. By understanding the types of messy data and the techniques to handle them, you can ensure your AI system is trained on clean, reliable information, leading to accurate and valuable results.*

## The Terminology of AI


## What ML can and cannot do


