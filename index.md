---
layout: default
---

<a name="toc"/>

<div style="text-align: center; font-size: 0.8em;">
<a href="#overview">Overview</a> &middot;
<a href="#speakers">Invited Speakers</a> &middot;
<a href="#topics">Topics</a> &middot;
<a href="#call">Call for Contributions</a> &middot;
<a href="#dates">Important Dates</a> &middot;
<a href="#schedule">Schedule</a> &middot;
<a href="#venue">Venue</a> &middot;
<a href="#organizers">Organizers</a>
</div>

----

<a name="overview"/>

Physical simulation is an important tool for robotic manipulation. Although simulation has been well-established for robotics education and integrated robot software testing, there is an ongoing debate about transferring manipulation capabilities learned in simulation to reality, a concept termed sim2real transfer.

In this workshop, we will shed light on the following questions: What is the potential impact of sim2real transfer on robotic manipulation? What methods exist and work best in the context of manipulation? To what extent can sim2real transfer reduce or avoid training on real robots altogether?

Simulation draws its appeal from the fact that it is much faster, cheaper, safer and more informative (e.g., auto-generated labels) than real-world experimentation. Recent advances have shown how to take advantage of simulation and address the sim2real transfer for tasks such as object detection, autonomous driving and grasp point detection.  However, sim2real transfer for general manipulation skills still raises significant challenges:

1. **Contact simulation**: Manipulation is about contact. However, simulating physics and in particular contact is a highly complex problem. The reason is that contact formation depends on a wide variety of physical properties such as friction, object deformability, etc. Since learning-based methods exploit any circumstance that facilitates finding a solution, they are prone to overfit to imprecise modeling and thus fail to learn transferable policies.
2. **Simulating closed-loop manipulation**: Manipulation is not a single-shot but a temporal process. Therefore, even slight errors at the beginning of a simulation sequence tend to accumulate and then lead to simulating unrealistic behavior and learning non-transferable policies.
3. **Curse of dimensionality**: Many state-of-the-art approaches to sim2real rely on sampling a large number of policies and environmental conditions. However, sampling becomes exponentially more difficult with the number of task dimensions. This raises the question whether current techniques will scale to the high-dimensionality of manipulation problems, e.g. involving high-DOF manipulators.
4. **Sensor fidelity**: Certain sensor modalities are much more difficult to simulate than others, e.g. simulating RGB or force/torque is more challenging than depth. Despite the recent advances in image synthesis and domain transfer techniques, we still do not fully understand what statistical properties of sensors need to be simulated in order to successfully learn from them.


<a name="speakers"/>

## Invited Speakers <a href="#toc" class="top-link">[Top]</a>



- Yunfei Bai (X)
- Feryal Behbahani (Latent Logic)
- Erwin Coumans (Google Brain)
- Chelsea Finn (UC Berkeley / Stanford / Google Brain)
- Kris Hauser (Duke)
- Edward Johns (Imperial College)
- Gilwoo Lee (University of Washington)
- Jean-Baptiste Mouret (INRIA)
- Fereshteh Sadeghi (University of Washington)
- Russ Tedrake (MIT)
- Josh Tobin (UC Berkeley / Open AI)
- Emo Todorov (University of Washington)

<a name="topics"/>
## Topics <a href="#toc" class="top-link">[Top]</a>

- **Learning from low-fidelity simulation**: Assuming that sensor and contact simulation will never be perfect. How can we learn in simulation despite these well-known shortcomings? How can we go beyond standard techniques such as pre-train/fine tune or residual learning to learn from simulation?
- **Manipulation-specific sensing**: Significant progress has been made in perceptual simulation, in particular using visual sensing. What is the fidelity of manipulation-specific sensors such as force/torque or tactile sensors? Which vision-related sim2real techniques can be transferred to manipulation-specific sensors?
- **Grasping**: How do we address the curse of dimensionality in simulating grasping when moving from pinch-/suction-based grippers to more complex hands?
- **Open-loop vs. closed-loop**: sim2real for manipulation shines in open-loop contexts, for example when predicting a grasp pose from a single image. How can we apply sim2real to learn high-frequency closed-loop behavior, where modeling errors can have catastrophic effects due to the accumulation of errors?
- **Interleaving learning in simulation and reality**: What are effective techniques to combine learning in simulation and reality to reduce sample complexity of pure real-world learning?
- **Real-to-sim**: To what extent can simulation benefit from real? For example, how can we learn about physical properties from real data in order to simulate better?
- **Generative modeling of sensors**: What methods are there to improve generative modeling of sensor outputs? How can we transfer across sensors and prevent overfitting to both specific sensor models and to their sensor properties?
- **Beyond domain randomization**:
  - Domain randomization enforces invariance to irrelevant aspects of the environment by simulating a vast quantity of irrelevant information. What are ways to incorporate the relevant information more directly into the learner?
  - Is domain randomization a good way forward when scaling up problems to high-dimensional robot embodiments?
- **Simulation software and datasets**: What are missing features in current simulation software required for sim2real for manipulation? Are there manipulation-specific datasets we imagine to be useful for sim2real for manipulation?
- What are **other approaches for advancing manipulation with sim2real** that are not listed here?
- What can manipulation learn from **sim2real approaches in other domains**? (Computer vision, autonomous driving, navigation, etc.)

<a name="call"/>
## Call for Contributions <a href="#toc" class="top-link">[Top]</a>

Participants are invited to submit **extended abstracts (maximum 2 pages in length)** related to the aforementioned topics.

Accepted abstracts will receive a poster presentation slot and, if equipment is available, a video presentation slot during the poster session.

Submissions must be in PDF following the IEEE style available from

[https://www.ieee.org/conferences/publishing/templates.html](https://www.ieee.org/conferences/publishing/templates.html)

**Submission website:** [https://cmt3.research.microsoft.com/SIMREALRM2019](https://cmt3.research.microsoft.com/SIMREALRM2019)

<a name="dates"/>
## Important dates <a href="#toc" class="top-link">[Top]</a>

* Submission Deadline: May 31, 2019
* Notification of Acceptance: June 11, 2019
* Camera ready submission: June 19, 2019
* Workshop: June 23, 2019 (full day)

<a name="schedule"/>
## Schedule <a href="#toc" class="top-link">[Top]</a>

*Note:* Schedule is tentative and subject to changes.

|---------------|--------------------------------------------------------------------|
| 8:15 - 8:30   | Welcome and introduction                                           |
| 8:30 - 10:30  | Invited Talks: Sim2real for Manipulation I                         |
| 10:30 - 11:00 | Posters / Coffee                                                   |
| 11:00 - 12:15 |  Invited Talks:Sim2real for Grasping                               |
|               | Lunch break                                                        |
| 14:00 - 15:15 | Invited Talks: Simulating Manipulation and Sim2real for Locomotion |
| 15:15 - 16:15 | Posters / Coffee                                                   |
| 16:15 - 17:30 | Invited Talks: Sim2real for Manipulation II                        |
| 17:30 - 18:30 | Speaker Panel                                                      |

<a name="venue"/>
## Venue <a href="#toc" class="top-link">[Top]</a>

Please check out the [RSS website](http://roboticsconference.org/attending/venue/) and [Google maps](https://goo.gl/maps/2iwdEFKUh1m) for detailed information on the workshop’s location. The room will be announced shortly.

<a name="organizers"/>
## Organizers <a href="#toc" class="top-link">[Top]</a>

| <img src="assets/images/shoefer.jpg" alt="Sebastian Höfer" width="300" /> | [Sebastian Höfer](http://www.sebastianhoefer.de) is an applied scientist at Amazon Research - Robotics AI headed by Siddhartha Srinivasa. Before joining Amazon, he received his Ph.D. with Oliver Brock at the Robotics & Biology Lab, Technische Universität Berlin.                                                                                                                                                                                                                                                                                                                                                             |
| <img src="assets/images/handa.jpg" alt="Ankur Handa" width="300" />  | [Ankur Handa](https://ankurhanda.github.io/) is a senior research scientist at the NVIDIA robotics lab run by Dieter Fox. Prior to that he was a research scientist at OpenAI. He received his Ph.D. with Dr. Andrew Davison and spent two years at University of Cambridge in Prof. Roberto Cipolla’s lab as a post-doctoral researcher.  |
| <img src="assets/images/kuzhinjedathu.jpg" alt="Kamal Kuzhinjedathu" width="300" /> | [Kamal Kuzhinjedathu](mailto:kamalkjd@amazon.com) is a senior applied scientist at Amazon Research - Robotics AI headed by Siddhartha Srinivasa. Before joining Amazon, he was a principal engineer at Microsoft working on perception for Microsoft Hololens. |
| <img src="assets/images/toussaint.jpg" alt="Marc Toussaint" width="300" /> | [Marc Toussaint](http://ipvs.informatik.uni-stuttgart.de/mlr/marc/index.html) is professor for Machine Learning and Robotics at the University of Stuttgart since 2012 and Max Planck Fellow at the MPI for Intelligent Systems since November 2018. His research aims to bridge between machine learning, control theory and AI planning, motivated by fundamental questions in robotics. Reoccurring themes in his research are appropriate representations and priors to enable efficient learning, reasoning and manipulation in the real world, combining geometry, logic and probabilities in learning and reasoning, and active learning and exploration. |
| <img src="assets/images/fox.jpg" alt="Dieter Fox" width="300" /> | [Dieter Fox](https://homes.cs.washington.edu/~fox/) is a Professor in the Department of Computer Science & Engineering at the University of Washington. He received his Ph.D. in 1998 from the Computer Science Department at the University of Bonn. He joined the UW faculty in the fall of 2000. He is currently on partial leave from UW and joined NVIDIA to start a Robotics Research Lab in Seattle. |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | |

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
