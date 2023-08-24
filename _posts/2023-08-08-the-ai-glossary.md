---
layout: post
title:  "The AI Glossary"
date: 2023-08-08
image: assets/images/glossary_thu.png
tags: [ AI ]
---



**Animation Glossaries**
- **fps**   
<code>fps</code>, frames per second, is a key setting in animation. A very low fps makes the animation laggy. A high fps means you need to draw more frames and higher demand on hardware capacity. <code>fps</code> 12 is a good start.

- **frame rate**   
The frame rate of an animation is the number of individual images (or frames) that are being displayed over the span of the one second. Frame rate, expressed in frames per second or FPS, is typically the frequency rate at which consecutive images (frames) are captured or displayed. 

- **interpolation**   
Interpolation is inbetweening in frames between the key frames in an animation. Interpolation animation is also called keyframe animation.

- **keyframe**   
Keyframe, or key frame, refers to the starting and/or ending point of any smooth transition. Animation is broken down into individual grames. The keyframes are the most important frames that set the parameters for the other frames and indicate the changes that will occur throughout as transitions. 

- **<code>max_frames</code>**   
<code>max_frames</code> refers to the number of output images to be created for a 2D animation or a 3d animation. <code>max_frames</code> is ignored during <code>video_input</code> mode. Instead, <code>video_input</code> follows the numbers of frames pulled from the input video's length. In <code>interpolation_mode</code>, the number of output frames follows your prompt schedule. A default value of 4 yeilds four frames of interpolation between prompts.

- **<code>noise_schedule</code>**   
<code>noise_schedule</code> refers to the amount of graininess to add per frame for diffusion diversity.

- **scene**   
The term scene refers to all the shots and dialogues that take place at a particular location for a continuous block of time.

- **shot**   
The term shot refers to the images between camera edits.

- **steps**   
The term steps refers the number of the denoising stemps. Usually, Higher is better but to a certain degree. The default is 25 steps.

- **<code>strength_schedule</code>**   
<code>strength_schedule</code> refers to the amount of presence of previous frame to influence next frame. 

- **timeline**   
The timeline is the part of the animation software that represents the animation's progress over time. Depending on the software, you might use the timeline to make changes to the timing of the animations, as well as the position of the elements.

**ChatGPT**   
ChatGPT is an artificial intelligence (AI) chatbot developed by OpenAI and released in November, 2022. ChatGPT is a member of the generative pre-trained transformer (GPT) class of language models. It's a task-specific GPT that was fine-tuned to target conversational usage, and was originally built upon an improved version of OpenAI's GPT-3 model known as "GPT-3.5". OpenAI acknowledges that ChatGPT "sometimes writes plausible-sounding but incorrect or nonsensical answers". This behavior is common to large language models and is called "hallucination". The reward model of ChatGPT, designed around human oversight, can be over-optimized and thus hinder performance, in an example of an optimization pathology known as Goodhart's law. ChatGPT has limited knowledge of events that occurred after September 2021.

**ControlNet**   
ControlNet is a neural network structure which can be used to control pretrained large diffusion models such as Stable Diffusion by adding extra conditions. It provides a way to augment Stable Diffusion with conditional inputs such as scribbles, edge maps, segmentation maps, pose key points, etc during text-to-image generation. In addition, a ControlNet model can be trained with small datasets on consumer GPU; and then, the model can be augmented with any pre-trained Stable Diffusion models for text-to-image generation.

**ControlNet Naming Convention**   
<img width=700 src="/assets/images/controlnet_naming.png" class="img-fluid" alt="ControlNet Naming" />

**ControlNet Models**

ControlNet 1.1 include 14 models (11 production-ready models and 3 experimental models):
1. control_v11p_sd15_canny
2. control_v11p_sd15_mlsd
3. control_v11f1p_sd15_depth
4. control_v11p_sd15_normalbae
5. control_v11p_sd15_seg
6. control_v11p_sd15_inpaint
7. control_v11p_sd15_lineart
8. control_v11p_sd15s2_lineart_anime
9. control_v11p_sd15_openpose
10. control_v11p_sd15_scribble
11. control_v11p_sd15_softedge
12. control_v11e_sd15_shuffle
13. control_v11e_sd15_ip2p
14. control_v11f1e_sd15_tile

- **Canny**   
Canny is a model that generates a line drawing from the original image using an algorithm called Canny edge detection, and then generates a new illustration from that line drawing. Very faithfully reproduced. A Canny edge is a monochrome image with white edges on a black background.

- **M-LSD**   
M-LSD is a model for line detection. It is often used for backgrounds and compositions. M-LSD controls Stable Diffusion with M-LSD straight lines.

- **Depth**   
Depth is a model that converts an image into a depth map and generates an image based on it. It is used for images with compositions where depth is important. A depth is a grayscale image with black representing deep areas and white representing shallow areas.

- **Normal**   
Normal is a model that converts the original image to a normal map and generates an image from the normal map. 

- **OpenPose**   
OpenPose detects keypoints of the human body, face, and limbs from images. Simply put, OpenPose is a model that generates images from stick figures. Since only the pose can be reproduced, there are fewer restrictions on the original image than with line drawings, so it is possible to generate more flexible images.

-  **Scribble**   
Scribble is a model that generates illustrations from hand-drawn images.

- **Seg**
Seg is a model that classifies an original image by semantic segmentation and generates an image from it.

- **Reference**   
Reference generates images similar to the style of the reference image. "reference_only", "reference_adain", and "reference_adain+attn" were added to ControlNet v1.1 around May 13, 2023. "adain" refers to a technique called "Adaptive Instance Normalization". "reference_adain" refers to style transfer via Adaptive Intance Normalization; "reference_only" links the reference image directly to the attention layers. "reference_adain+attn" combines the two.

- **Soft Edge**   
Soft Edge retains tough sketch-like edges and includes some fine lines. Soft Edge provieds more variability during image generation. It can be used when Canny and Scribble are not suitable.

- **Shuffle**   
Shuffle randomly positions objects in the reference image. Shuffle can be used for transferring the color scheme of hte reference image. 

- **Line Art**   
Line Art converts the reference image into a line drawing or black and white sketch. 
 
- **Instruct Pix2Pix**   
Instruct Pix2Pix modifies the state of the objects in the reference image.

- **Inpaint**   
ControlNet Inpaint performs local repaint. It is useful for generating videos in m2m format.

- **Tile**   
Tile is suitable for zooming and maginificaiton purposes.

**DEFORUM**

**Deforum 2D Animation Motion Parameters**
- **angle**   
2D operator that rotates canvas closewise/counter clockwise in degrees per frame. Positive angle values rotate the canvas counter-clockwise which feels like the camera rotating clockwise. The default value is 

- **zoom**   
2D operator that scales the canvas size, multiplicatively [static = 1.0]

- **translation_x**   
2D that moves canvas left/right in pixels per frame. Positive translation_x shifts the canvas to the right which feels like the camera shifting to the left.

- **translation_y**   
2D operator that moves canvas up/down in pixels per frame. Positive translation_y shifts the canvas down the screen which feels like the camera shifting upward.

- **transform_center_x, transform_center_y**   
The term Transform Center is for changing the focal point of zoom and/or rotation. The default value is: transform_center_x: 0: (0.5), and transform_center_y: 0: (0.5), which is the center of the canvas. (X,Y) = (0,0) is the top left corner, and (1,1) is the bottom right corner.

- **noise_schedule**   
Amount of graininess to add per frame for diffusion diversity

- **strength_schedule**   
Amount of presence of previous frame to influence next frame

- **contrast_schedule**   
The term contrast_schedule adjusts the overall contrast per frame   

**Emergent behavior**   
Unexpected or unintended abilities in a large language model, enabled by the model’s learning patterns and rules from its training data. For example, models that are trained on programming and coding sites can write new code. Other examples include creative abilities like composing poetry, music and fictional stories.

**Generative AI**   
Technology that creates content — including text, images, video and computer code — by identifying patterns in large quantities of training data, and then creating original material that has similar characteristics. Examples include ChatGPT for text and DALL-E and Midjourney for images.

**Hallucination**   
A well-known phenomenon in large language models, in which the system provides an answer that is factually incorrect, irrelevant or nonsensical, because of limitations in its training data and architecture.

**Large language model (LLM)**    
A type of neural network that learns skills — including generating prose, conducting conversations and writing computer code — by analyzing vast amounts of text from across the internet. The basic function is to predict the next word in a sequence, but these models have surprised experts by learning new abilities.

**Natural language processing (NLP)**   
Techniques used by large language models to understand and generate human language, including text classification and sentiment analysis. These methods often use a combination of machine learning algorithms, statistical models and linguistic rules.

**Neural network**   
A mathematical system, modeled on the human brain, that learns skills by finding statistical patterns in data. It consists of layers of artificial neurons: The first layer receives the input data, and the last layer outputs the results. Even the experts who create neural networks don’t always understand what happens in between.

**Parameters**   
Numerical values that define a large language model’s structure and behavior, like clues that help it guess what words come next. Systems like GPT-4 are thought to have hundreds of billions of parameters.

**Reinforcement learning**   
A technique that teaches an A.I. model to find the best result by trial and error, receiving rewards or punishments from an algorithm based on its results. This system can be enhanced by humans giving feedback on its performance, in the form of ratings, corrections and suggestions.

**Transformer model**   
A neural network architecture useful for understanding language that does not have to analyze words one at a time but can look at an entire sentence at once. This was an A.I. breakthrough, because it enabled models to understand context and long-term dependencies in language. Transformers use a technique called self-attention, which allows the model to focus on the particular words that are important in understanding the meaning of a sentence.


**Stable Diffusion**      
Stable Diffusion is a latent diffusion text-to-image AI model released in 2022. Stable Diffusion was developed by the Stability AI in collaboration with a number of academic researchers and non-profit organizations. Stable Diffusion consists of 3 parts: the variational autoencoder (VAE), U-Net, and an optional text encoder. The VAE encoder compresses the image from pixel space to a smaller dimensional latent space, capturing a more fundamental semantic meaning of the image. Gaussian noise is iteratively applied to the compressed latent representation during forward diffusion. The U-Net block, composed of a ResNet backbone, denoises the output from forward diffusion backwards to obtain a latent representation. Finally, the VAE decoder generates the final image by converting the representation back into pixel space. The denoising step can be flexibly conditioned on a string of text, an image, or another modality. The encoded conditioning data is exposed to denoising U-Nets via a cross-attention mechanism. For conditioning on text, the fixed, pretrained CLIP ViT-L/14 text encoder is used to transform text prompts to an embedding space. Stable Diffusion was trained on pairs of images and captions taken from LAION-5B, a publicly available dataset derived from Common Crawl data scraped from the web, where 5 billion image-text pairs were classified based on language and filtered into separate datasets by resolution, a predicted likelihood of containing a watermark, and predicted "aesthetic" score (e.g. subjective visual quality). The dataset was created by LAION, a German non-profit which receives funding from Stability AI. The Stable Diffusion model was trained on three subsets of LAION-5B: laion2B-en, laion-high-resolution, and laion-aesthetics v2 5+. A third-party analysis of the model's training data identified that out of a smaller subset of 12 million images taken from the original wider dataset used, approximately 47% of the sample size of images came from 100 different domains, with Pinterest taking up 8.5% of the subset, followed by websites such as WordPress, Blogspot, Flickr, DeviantArt and Wikimedia Commons.

**Stable Diffusion 2**   
Stable Diffusion 2 is a text-to-image latent diffusion model built upon the work of Stable Diffusion 1. The project to train Stable Diffusion 2 was led by Robin Rombach and Katherine Crowson from Stability AI and LAION. The Stable Diffusion 2.0 release includes robust text-to-image models trained using a brand new text encoder (OpenCLIP), developed by LAION with support from Stability AI, which greatly improves the quality of the generated images compared to earlier V1 releases. The text-to-image models in this release can generate images with default resolutions of both 512x512 pixels and 768x768 pixels. These models are trained on an aesthetic subset of the LAION-5B dataset created by the DeepFloyd team at Stability AI, which is then further filtered to remove adult content using LAION’s NSFW filter.