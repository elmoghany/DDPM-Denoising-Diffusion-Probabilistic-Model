# DDPM Denoising Diffusion Probabilistic Model Implementation

## Forward Process
𝝱 in the range [0.0001, 0.02] and set the total timesteps T = 1000

X0 is the original picture

ϵ is adding noise to the picture in the from of N(0,1)

![pic](assets/DDPM-pre-forward.png)

![pic](assets/DDPM-alpha-forward.png)

![pic](assets/DDPM-forward.png)

## Reverse Process
ϵθ​(x_t​,t) is model’s output. Network is trying to denoise and predict the image from the existing noise.

σ = √𝝱

![pic](assets/DDPM-pre-forward.png)

![pic](assets/DDPM-reverse-mean.png)

![pic](assets/DDPM-reverse-xt-1.png)

![pic](assets/DDPM-reverse-xt-1-2.png)


## Training Loss MSE "ELBO"

![pic](assets/DDPM-loss1.png)

Same as forward process => ![pic](assets/DDPM-loss2.png)

## Dataset used
[AFHQ Animals Dataset](https://huggingface.co/datasets/huggan/AFHQ)
![pic](assets/AFHQ-dataset.png)

## Results

FID Score ~= 5

![pic](assets/DDPM-output.png)

### Disclaimer:
1. All of the code is inside the Jupyter notebook file.
2. Parts of the code are copied from unsolved assignments of Prof. Minhyuk Sung @ KAIST, a graduate course about diffusion models.
3. Work is done during KAUST internship with KAUST GPUs @ Prof. Mohamed Elhoseiny Lab, as part of the learnings to create a diffusion project.
