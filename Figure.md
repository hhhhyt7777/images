<figure>
  <p align="center">
  <img src="Figure 1.jpg" alt="" width="1000">
  </p>
  <figcaption>Figure 1: Step-wise branch discrepancy under baseline, shared guidance, and decoupled guidance. The left y-axis plots the baseline discrepancy <span>&#8741;&Delta;<sub>t</sub>&#8741;</span>, and the right y-axis plots the guidance branch discrepancy &#8741;&epsilon;<sub>+</sub> - &epsilon;<sub>-</sub>&#8741. In the baseline, after the extremely noisy initial stage, the positive and counterfactual branches quickly collapse into a shared coarse semantic trajectory, and <span>&#8741;&Delta;<sub>t</sub>&#8741;</span> remains relatively small during early denoising, which reflects the lagged suppression effect. Compared with shared guidance, decoupled guidance consistently preserves a much larger branch discrepancy, showing that shared trajectories suppress the counterfactual signal and that trajectory decoupling can better maintain an independent guidance direction. The shaded region denotes the early denoising stage where coarse semantic structure is established.</figcaption>
</figure>

<figure>
  <p align="center">
  <img src="Figure 2.png" alt="" width="700" >
  </p>
  <figcaption>Figure 2: Cosine similarity between the positive branch &epsilon;<sup>+</sup> and the counterfactual branch &epsilon;<sup>-</sup> throughout denoising. In the baseline, the similarity remains almost exactly 1, showing that previous negative prompting produces a counterfactual signal that is nearly fully aligned with the positive direction. Under shared guidance, the similarity is reduced but still remains high, indicating that the shared latent trajectory continues to constrain the counterfactual branch. Under decoupled guidance, the similarity is consistently much lower, which means that the counterfactual branch can evolve along a more independent direction. These results directly support the existence of trajectory bias under shared trajectories and show that decoupling is necessary to preserve a distinct counterfactual guidance direction.</figcaption>
</figure>
