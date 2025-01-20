# DDPM Denoising Diffusion Probabilistic Model Implementation

## Forward Process
𝝱 in the range [0.0001, 0.02] and set the total timesteps T = 1000

X0 is the original picture

ϵ is adding noise to the picture in the from of N(0,1)

![pic](assets/DDPM-pre-forward.png)

![pic](assets/DDPM-alpha-forward.png)

![pic](assets/DDPM-forward.png)

## Reverse Process
ϵθ​(x_t​,t) is model’s output, predicted noise

![pic](assets/DDPM-pre-forward.png)

![pic](assets/DDPM-reverse-mean.png)

![pic](assets/DDPM-reverse-xt-1.png)



## Training Loss MSE "ELBO"
