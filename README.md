# stable-k-4d

jupyter/colab implementation of [Stable Diffusion](https://github.com/CompVis/stable-diffusion) and Katherine Crowson's [k-diffusion wrapper](https://github.com/crowsonkb/k-diffusion) in order to use the k_lms sampler  by [karan4d](https://twitter.com/karan4d) aka [DamascusGit](https://github.com/DamascusGit). The notebook utilizes CPU draw manual seeding with k_lms and has a weird quantize.py adjustment in an attempt to best replicate the results from Simulacra/Dreambot using the stable-diffusion weights.

## Using The Notebook
Provided you have the weights, store them in 
```
/stable-diffusion/models/ldm/stable-diffusion-v1/
```
Change your desired model's name to model.ckpt.

Replace ```quantize.py``` in  ```/usr/local/lib/python3.7/site-packages/taming/modules/vqvae/quantize.py``` with

```/stable-diffusion/quantize.py```.

Run the cells in order except for "DEBUG SHIT IGNORE THIS".

## Comments
implemented with the help of [Katherine Crowson](https://https://twitter.com/rivershavewings), palp, wbrown, and litexev. 

This would not exist without the good folks over at [EleutherAI](https://eleuther.ai) + [StabilityAI](https://stability.ai).

Inspired by the very special work of the [SimulacraBot Team](https://github.com/JD-P/simulacrabot).
