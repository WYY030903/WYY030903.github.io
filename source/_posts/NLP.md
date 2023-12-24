---
## Project 1 of **Advanced natural language Processing**

													                                         –12111641 魏悦阳

### Q1 Paper reading and answering

![image-20231025162203208](assets\image-20231025162203208.png)

#### 1. What is the problem addressed in the paper?

This article discusses the application of the **Transformer** architecture in the field of **computer vision** and introduces a novel model known as the **Vision Transformer (ViT)**. The primary focus of this article is on **image classification**.

The ViT model was meticulously designed to closely follow the original Transformer architecture. It involves breaking down the input image into numerous patches, reshaping these 2D patches into a 1D sequence, and subsequently employing the **Transformer** to process these sequences. In addition to this, the model incorporates **extra learnable embeddings** and **position embeddings**. Ultimately, the **MLP Head** is employed to complete the image classification task.

![image-20231025162234698](assets/image-20231025162234698.png)

#### 2. Is this a new problem?

This isn't an entirely new problem but rather a novel approach that leverages the **Transformer** architecture in the domain of **Computer Vision (CV)**, which is originally developed for **Natural Language Processing (NLP)**, .

This method disrupts the dominant roles that **Convolutional Neural Networks (CNNs)** and **Recurrent Neural Networks (RNNs)** have traditionally held in the field of CV, and it has yielded remarkable performance results.

#### 3. What is the scientific hypothesis that the paper is trying to verify?

This article aims to demonstrate the feasibility of utilizing the **Transformer** architecture for **image classification** and underscores its excellence, particularly when applied to large-scale datasets.

#### 4. What are the key related works and who are the key people working on this topic?

Basic works: **Transformer**(*Attention is all you need*), **BERT** model(*BERT: Pre-training of deep bidirectional transformers for language understanding*)

Most similar work: 2×2 patches(**On the relationship between self-attention and convolutional layers**)

Important people: **Alexey Dosovitskiy**, **Thomas Kipf**, **Ilya Sutskever**, etc.

#### 5. What is the key of the proposed solution in the paper?

Change 2D images into 1D sequences and just "copy" transfomer.

#### 6. How are the experiments designed?

It compare with state of the art on popular image classification benchmarks, which using mean and standard deviation of accuracies together with days trained by TPUv3.

![image-20231024225625023](assets/image-20231024225625023.png)

It also show performance versus pre-training compute for VIT, ResNet and Hybrid.

![image-20231024225857600](assets/image-20231024225857600.png)



#### 7. What datasets are built/used for the quantitative evaluation? Is the code open sourced?

It used public datasets wit 14M-300M images, including **ImageNet**, **JFT**, **CIFAR-100** and **VTAB**.

The code is available at *https://github.com/google-research/vision_transformer*

#### 8. Is the scientific hypothesis well supported by evidence in the experiments?

Yes! The experiments well supported that Transformer can be use in CV especially in large-scale datasets.

#### 9. What are the contributions of the paper?

This marks a milestone in the utilization of the Transformer in **computer vision (CV)**, starting off significant advancements in various **CV** research areas and making multimodal analysis possible.

#### 10. What should/could be done next?

Enhancing ViT and Extending the Use of ViT and Transformers in Other Computer Vision Domains.

Over the past two years, a plethora of improved models have emerged, including **PVT** (reducing computational requirements), **DeiT** (optimizing training data usage), **DeepViT** (increasing network depth), **DETR** (handling positional encoding differently), **DVT** (reducing model parameters), and so on.

### Q2 LLM using and improving

#### 1. Help writing

Task description：生成一篇辩论赛的一辩稿。

<img src="assets/image-20231025162324252.png" alt="image-20231025162324252" style="zoom:33%;" />

Prompt: Role

It helps AI understanding question.

<img src="assets/image-20231025162357044.png" alt="image-20231025162357044" style="zoom:33%;" />

 Prompt: demand

It helps AI get accurate demand. 

<img src="assets/image-20231025162408370.png" alt="image-20231025162408370" style="zoom:33%;" />

Expect answer: 一篇可以直接上场的一辩稿，其中有数据、学理、案例的支撑，并且有着严密的逻辑。

#### 2. Code writing

*This part has video, which can't show in .pdf file while can show in .md file.*

Task description: 用python中的3b1b动画引擎包生成关于VIT中reshape过程的动画代码。

<img src="assets/image-20231025162428457.png" alt="image-20231025162428457" style="zoom: 33%;" />

<video src="assets\Test@2023-10-25@13-44-02.mp4"></video>

Prompt: describe in details. 

<img src="assets/image-20231025162545636.png" alt="image-20231025162545636" style="zoom:33%;" />

<video src="assets\Test@2023-10-25@14-06-52.mp4"></video>

Prompt: describe the movie one by one 

*In this part, I adjust the code by myself in order to get good result*

<img src="assets/image-20231025162606417.png" alt="image-20231025162606417" style="zoom:50%;" />

<video src="assets\Test@2023-10-25@15-46-28.mp4"></video>

Expect answer: I want to show the process of VIT clearly, and try to use the GPT to generate.

*It seems not a good choice.*

#### 3. Question asking

Task description: 帮我决定今天晚上吃什么。

<img src="assets/image-20231025162631462.png" alt="image-20231025162631462" style="zoom:50%;" />

Prompt: 描述我的状况

<img src="assets/image-20231025162638952.png" alt="image-20231025162638952" style="zoom:50%;" />

Prompt: 请他给我结果

<img src="assets/image-20231025162645896.png" alt="image-20231025162645896" style="zoom:50%;" />

Exception answer: Tell me eat what! 

*Today's dinner is sushi🍣!*
---

|      |      |      |
| ---- | ---- | ---- |
|      |      |      |
