---
layout: default
---

*The workshop proposal is currently under review at R:SS 2019. More info coming soon.*

## Abstract

Physical simulation is an important tool for robotic manipulation. Although simulation has been well-established for robotics education and integrated robot software testing, there is an ongoing debate about transferring manipulation capabilities learned in simulation to reality, a concept termed sim-to-real transfer.

In this workshop, we will shed light on the following questions: What is the potential impact of sim-to-real transfer on robotic manipulation? What methods exist and work best in the context of manipulation? To what extent can sim-to-real transfer reduce or avoid training on real robots altogether?

Simulation draws its appeal from the fact that it is much faster, cheaper, safer and more informative (e.g., auto-generated labels) than real-world experimentation. Recent advances have shown how to take advantage of simulation and address the sim-to-real transfer for tasks such as object detection, autonomous driving and grasp point detection. However, sim-to-real transfer for general manipulation skills still raises significant challenges:

1. Contact simulation: Manipulation is about contact. However, simulating physics and in particular contact is a highly complex problem. The reason is that contact formation depends on a wide variety of physical properties such as friction, object deformability, etc. Since learning-based methods exploit any circumstance that facilitates finding a solution, they are prone to overfit to imprecise modeling and thus fail to learn transferable policies.
2. Simulating closed-loop manipulation: Manipulation is not a single-shot but a temporal process. Therefore, even slight errors at the beginning of a simulation sequence tend to accumulate and then lead to simulating unrealistic behavior and learning non-transferable policies.
3. Curse of dimensionality: Many state-of-the-art approaches to sim-to-real rely
on sampling a large number of policies and environmental conditions. However, sampling becomes exponentially more difficult with the number of task dimensions. This raises the question whether current techniques will scale to the high- dimensionality of manipulation problems, e.g. involving high-DOF manipulators. (iv) Sensor fidelity: Certain sensor modalities are much more difficult to simulate than others, e.g. simulating RGB or force/torque is more challenging than depth. Despite the recent advances in image synthesis and domain transfer techniques, we still do not fully understand what statistical properties of sensors need to be simulated in order to successfully learn from them.

<!--
We encourage researchers to submit their contributions, addressing, but not limited to the following questions:

* Learning from low-fidelity simulation: Assuming that sensor and contact simulation will never be perfect. How can we learn in simulation despite these well-known shortcomings? How can we go beyond standard techniques such as pre-train/fine tune or residual learning to learn from simulation?
* Manipulation-specific sensing: Significant progress has been made in perceptual simulation, in particular using visual sensing. What is the fidelity of manipulation-specific sensors such as force/torque or tactile sensors? Which vision-related sim-to-real techniques can be transferred to manipulation-specific sensors?
* Grasping: How do we address the curse of dimensionality in simulating grasping when moving from pinch-/suction-based grippers to more complex hands?
* Open-loop vs. closed-loop: Sim-to-real for manipulation shines in open-loop contexts, for example when predicting a grasp pose from a single image. How can we apply sim-to-real to learn high-frequency closed-loop behavior, where modeling errors can have catastrophic effects due to the accumulation of errors?
* Interleaving learning in simulation and reality: What are effective techniques to combine learning in simulation and reality to reduce sample complexity of pure real-world learning?
* Real-to-sim: To what extent can simulation benefit from real? For example, how can we learn about physical properties from real data in order to simulate better?
* Generative modeling of sensors: What methods are there to improve generative modeling of sensor outputs? How can we transfer across sensors and prevent overfitting to both specific sensor models and to their sensor properties?
* Beyond domain randomization:
    * Domain randomization enforces invariance to irrelevant aspects of
the environment by simulating a vast quantity of irrelevant information. What are ways to incorporate the relevant information more directly into the learner?
    * Is domain randomization a good way forward when scaling up problems to high-dimensional robot embodiments?
* Simulation software and datasets: What are missing features in current simulation software required for sim-to-real for manipulation? Are there manipulation-specific datasets we imagine to be useful for sim-to-real for manipulation?
* What are other approaches for advancing manipulation with sim-to-real that are not listed here?

-->

<!--
---
-->

<!-- ## News -->
<!-- {% for post in site.posts %}
  <article>
    <h3 id="news-{{ forloop.index }}">
       {{ post.title }}
    </h3>
    <p>
    <small>posted at <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time> &middot; by {{ post.user }}</small>
    </p>
    {{ post.content }}
  </article>
{% endfor %} -->
