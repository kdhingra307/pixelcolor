## Image Colorization



- Datasets
  - https://soonminhwang.github.io/rgbt-ped-detection/data/
  - https://groups.csail.mit.edu/vision/datasets/ADE20K/ADE20K_2016_07_26.zip
- Models
  - Translation, 
    - translation.ipynb - requires kaist data, and weights from https://github.com/joehoeller/Object-Detection-on-Thermal-Images
    - Works both MSE and logistic mixture based loss (function is taken from another source, marked in github)
  - generation,
    - generation.ipynb, and generation_tf.ipynb
      - generation_tf is completely written by myself, while the gan structure from generation.ipynb is from pytorch/DCGAN.
      - switched to pytorch, because of some very minute error in the code of generator_tf. 
      - generator uses DCGAN based loss function, while generator_tf uses Wasserstein loss as it reduces the mode collapse problem.
  - pixcolor
    - pixcolor.ipynb
      - based on previous pixelcolor implementation, had new backend layer and sampling algorithm from logistic mixture loss function.
  - weights for all are shared in github assets.
- for any queries, and issues please let me know