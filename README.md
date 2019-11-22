# talking-head-stylegan

This project is based on ![StyleGAN-Encoder](https://github.com/pbaylies/stylegan-encoder)

# What's the idea?
Let's find latent representations for the face images corresponding to different phonemes and make this face say what we want :)  

# How to do it?
1. Use ![Gentle](https://github.com/lowerquality/gentle) to extract phonemes corresponding to their timestamps in the source audio 
2. Extract frames from the video, which corresponds to their phonemes
3. Find latent representations (LR) for these frames
4. Extract phonemes for target audio
5. Put phonemes in the right order according to the target audio. Find intermediate LRs to make output video smooth. Save resulting frames to output video 
5. Merge output video and target audio

All code in ![talking_head.ipynb](talking_head.ipynb). You only need to put your source video in `./input` directory

# Results
Output video 

[![Watch output video](https://i.ibb.co/3cpd9BK/image.png)](https://www.youtube.com/watch?v=73aUnd0na04)
