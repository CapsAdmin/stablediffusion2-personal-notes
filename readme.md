# various personal notes on stable diffusion 2.0 in automatic1111

- famous people exist, but tend to cause baked images

  - to fix, be more specific about style

- https://laion-aesthetic.datasette.io/ can be a good source for prompt inspiration

  - searchable dataset of training data with an aesthetic score of 6 or higher (out of 10)

- https://huggingface.co/spaces/pharma/CLIP-Interrogator based on the new clip model can give you an idea of what prompts to use, unsure if it's what sd2 uses though

# prompts

- prompts further to the left affect the overall composition of the image and prompts further to the right affect the details of the image

  - for instance `anime` on the left will make the entire image anime, but `anime` on the right will try to retrofit anime details into the image

- unsure if the above applies can be used for negative prompts? never tried

## negative prompts that seem to work well:

- ((((ugly)))), (((duplicate))), ((morbid)), ((mutilated)), [out of frame], extra fingers, mutated hands, ((poorly drawn hands)), ((poorly drawn face)), (((mutation))), (((deformed))), ((ugly)), blurry, ((bad anatomy)), (((bad proportions))), ((extra limbs)), cloned face, (((disfigured))). out of frame, ugly, extra limbs, (bad anatomy), gross proportions, (malformed limbs), ((missing arms)), ((missing legs)), (((extra arms))), (((extra legs))), mutated hands, (fused fingers), (too many fingers), (((long neck)))

- stock image, istock, yayimages, gettyimages, watermark, tiling, poorly drawn hands, poorly drawn feet, poorly drawn face, out of frame, body out of frame, blurry, bad art, blurred, text, grainy

- photoshop, video game, ugly, tiling, poorly drawn, poorly drawn feet, poorly drawn face, out of frame, mutation, mutated, extra limbs, extra legs, extra arms, disfigured, deformed, cross-eye, body out of frame, blurry, bad art, bad anatomy, 3d render, photograph

# embeddings

- https://www.reddit.com/r/StableDiffusion/comments/z622mp/trained_midjourney_embedding_on_stable_diffusion/
  - midjourney and greg rutkowski embeddings. works really well with little effort, maybe a bit overtrained
  - would be fun to try and figure out what kind of prompts lead to those embeddings
