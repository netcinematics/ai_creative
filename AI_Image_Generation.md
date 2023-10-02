# ai image generation
- diffustion models
- inspired by physics
<hr></hr>
## THEORY of DIFFUSION MODELS
- Train & Deploy on Vertex AI
### Many MODEL FAMILIES
1. VARIATIONAL Auto Encoders (VAEs)
- encode image to compresser,
- decode back, learning distribution of the data
2. GENERATIVE Adversarieal Models (GANs)
- two opposing Neural Networks
- GENERATOR creates images
- DISCRIMINATOR guesses fakes
- both get better over time real fakes (deep fakes)
3. Auto Regressive Models
- image is sequence of pixels
- inspiration from LLMs
4. DIFFUSION MODELS.
- inspiration from physics (thermo dynamics)
- research space and industry space
- state of art image generation systems
- promise many usecases
## UNCONDITIONED and CONDITIONED
### UNCONDITIONED_GENERATION
- no additional instruction or input data
- trained on image of specific thing
- generate new images of thing
1. Human face synthesis
2. SUPER-RESOLUTION:
- enhancing low quality images.
### CONDITIONED_GENERATION
- additional conditioning... input/ instruction.
1. Text_to_image
2. Image_in_Painting
3. Text_guided Image_to_image
- remove / add / edit
## How it works DDPM
- systematicaly and slowly distroy, 
- structure in data distribution, by 
- iterative FORWARD_DIFFUSION process
- learn REVERSE_DIFFUSION
- restores structure in data,
yields highly flexible and tractable generative model of image data.
- add noise, and train model - to denoise images.
- DENOISING from pure noise, 
Synthgesize - until unique image is generated.
GAUSSIAN NOISE added. (BLUR)
- BLUR into NOVEL IMAGE
- LARGE DATA SET OF IMAGES
- Forward Diffusion Process (little bit of noise.
- iteratively add more and more noise.
- only depends on previous step. How many blur steps? 1000.
- reach a state of pure noise. (easy part)
### Challenging part REVERSE DIFFUSION PROCESS
- learn from the noise add
- input is noisy image, predicts noise that was added. 
- SAMPLE at TIMESTAMP - to denoising model. GOAL predict noise.
- COMPARE predicted noise and noise we added.
- ML trained to minimize difference 
(gets very good at removing noise) FUN PART.
### AFTER TRAIN MODEL (how to remove noise) 3.
ITERATIVELY:
1. start pure noise
2. send through trained ML model
3. output, subtracted from noise
GOAL: generated image.
- model learn data distribution, from what its seen,
then SAMPLE from LEARN DISTRIBUTION for Novel Images.
DDPM Generation.
## ADVANCEMENTS
- fast, conditioned, CLIPs
- text_to_image is combined power of LLM + Diffusion Model.
- text embedding
- TEXT_to_IMAGE_DIFFUSION_MODEL
- SUPER-RESOLUTION_DIFFUSION MODEL 64x, 256x, 1024x.
COMBINED DIFFUSION and LLM.
Photo Realistic from Text prompt.
Context Aware.
IMAGEN from google research.
composition of LLM and a few diffusion based models.
VERTEX AI
