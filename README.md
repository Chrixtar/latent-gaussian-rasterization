# Latent Gaussian Rasterizer
This is a modified version of the differentiable 3D Gaussian rasterizer from "3D Gaussian Splatting for Real-Time Rendering of Radiance Fields" (Kerbl et al.), adapted for the implementation of <a href="https://geometric-rl.mpi-inf.mpg.de/latentsplat/">latentSplat: Autoencoding Variational Gaussians for Fast Generalizable 3D Reconstruction</a> (Wewer et al.).

## Modifications

- Spherical harmonics match e3nn now.
- Return alpha mask and depth, and allow gradients through them
- Optional rasterization of high-dimensional features and stop gradient through features to all structural Gaussian parameters

## Citation

This modified rasterizer is used for the paper "latentSplat: Autoencoding Variational Gaussians for Fast Generalizable 3D Reconstruction". If you can make use of it in your own research, please be so kind to cite us (first BibTex item).
Moreover, please consider citing the paper "3D Gaussian Splatting for Real-Time Rendering of Radiance Fields" (second BibTex item), which provided the implementation of the original rasterization engine.

<section class="section" id="BibTeX">
  <div class="container is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>@inproceedings{wewer24latentsplat,
    title     = {latentSplat: Autoencoding Variational Gaussians for Fast Generalizable 3D Reconstruction},
    author    = {Wewer, Christopher and Raj, Kevin and Ilg, Eddy and Schiele, Bernt and Lenssen, Jan Eric},
    booktitle = {arXiv},
    year      = {2024},
}</code></pre>

  <pre><code>@Article{kerbl3Dgaussians,
      author       = {Kerbl, Bernhard and Kopanas, Georgios and Leimk{\"u}hler, Thomas and Drettakis, George},
      title        = {3D Gaussian Splatting for Real-Time Radiance Field Rendering},
      journal      = {ACM Transactions on Graphics},
      number       = {4},
      volume       = {42},
      month        = {July},
      year         = {2023},
      url          = {https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/}
  }</code></pre>
  </div>
  
</section>
