---
layout: post
title:  "Using Stable Diffusion WebUI on Google Colab"
date: 2023-08-08
image: assets/images/webui.png
tags: [ AI, resources ]
---

**How to run Stable Diffusion WebUI on Google Colab**
1. Enable GPU. 
2. Download Stable Diffusion WebUI:   
    <code>!git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui</code>
3. Go to the Stable Diffusion WebUI directory:   
    <code>%cd /content/stable-diffusion-webui</code>
4. Launch the Stable Diffusion WebUI:   
    <code>!python ./launch.py --share --xformers --enable-insecure-extension-access</code>

    Parameters:     
    <code>--share</code>: to publish to gradio.app   
    <code>--xformers</code>: to improve image generation speed   
    <code>--enable-insecure-extensions-access</code>: to install extensions

**More resources**
1. Here's where you can find more about GIT:    
    [https://git-scm.com/docs/git](https://git-scm.com/docs/git){:target="_blank"}
2. Here's where you can find Automatic 1111's Stable Diffusion WebUI Github page:   
    [https://github.com/AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui){:target="_blank"}
3. Here's where you can find Automatic 1111's Stable Diffusion WebUI wiki:   
    [https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki){:target="_blank"}
4. Heres' where you can find more about how to use Google Colab:   
    [https://research.google.com/colaboratory/faq.html](https://research.google.com/colaboratory/faq.html){:target="_blank"}
5. Here's where you can find more about how to use shell commands in Google Colab:   
    [https://jakevdp.github.io/PythonDataScienceHandbook/01.05-ipython-and-shell-commands.html](https://jakevdp.github.io/PythonDataScienceHandbook/01.05-ipython-and-shell-commands.html){:target="_blank"}


