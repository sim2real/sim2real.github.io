---
layout: default
---

<div align="center">
<h3 style="font-color: darkgreen;">NEWS: Final schedule is online</h3>
</div>

----

<a name="toc"/>

<div style="text-align: center; font-size: 0.8em;">
<a href="#overview">Overview</a> &middot;
<a href="#speakers">Invited Speakers</a> &middot;
<a href="#topics">Topics</a> &middot;
<a href="#call">Call for Contributions</a> &middot;
<a href="#dates">Important Dates</a> &middot;
<a href="#papers">Accepted Papers</a> &middot;
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

Participants are invited to submit **extended abstracts (maximum 2 pages in length, excluding references)** related to the aforementioned topics.

Accepted abstracts will receive a poster presentation slot and, if equipment is available, a video presentation slot during the poster session.

* Submissions must not exceed *2 pages in length, excluding references*.
* Submissions must be in PDF following the IEEE style available from<br/>
  [https://www.ieee.org/conferences/publishing/templates.html](https://www.ieee.org/conferences/publishing/templates.html)
* Submissions must include a short abstract. The *extended abstract* should go in the main section of the template and the *short abstract* in the abstract section.

**Submission website:** [https://cmt3.research.microsoft.com/SIMREALRM2019](https://cmt3.research.microsoft.com/SIMREALRM2019)

<a name="dates"/>
## Important dates <a href="#toc" class="top-link">[Top]</a>

* Submission Deadline: June 3, 2019 <s>May 31, 2019</s>
* Notification of Acceptance: **June 17, 2019** <s>June 14, 2019</s>
* Camera ready submission: June 21, 2019 <s>June 19, 2019</s>
* Workshop: June 23, 2019 (full day)


<a name="papers"/>
## Accepted Papers <a href="#toc" class="top-link">[Top]</a>

* Adam Allevato, Elaine Short, Mitch Pryor, Andrea Thomaz - TuneNet: One-Shot Simulation Tuning for Physics Prediction and Robot Task Planning [<a href="allevato.pdf">pdf</a>]
* Brayan S. Zapata-Impata, Pablo Gil, Fernando Torres  - vision2tactile: Feeling Touch by Sight [<a href="zapata.pdf">pdf</a>]
* Diego Ferigo, Silvio Traversaro, Daniele Pucci  - Gym-Ignition: Reproducible Robotic Simulations for Reinforcement Learning [<a href="ferigo.pdf">pdf</a>]
* Eric Heiden, David R Millard, Gaurav Sukhatme  - Real2Sim Transfer using Differentiable Physics [<a href="heiden.pdf">pdf</a>]
* Jakob Hollenstein, Justus Piater  - Evaluating Planning for Policy Search [<a href="hollenstein.pdf">pdf</a>]
* Jonas Kiemel - PaintRL: Coverage Path Planning for Industrial Spray Painting with Reinforcement Learning [<a href="kiemel.pdf">pdf</a>]
* Joshua P. Powers, Dylan Shah  - Sim2real of soft-bodied, shape-changing robots [<a href="powers.pdf">pdf</a>]
* Kent A. Rosser - Sim2real transfer degrades non-monotonically with morphological complexity for flapping wing design [<a href="rosser.pdf">pdf</a>]
* Manuel Kaspar, Jürgen Bock - Reinforcement Learning with Cartesian Commands andSim to Real Transfer for Peg in Hole Tasks [<a href="kaspar.pdf">pdf</a>]
* Max K. Nielsen - Data Driven Inverse Kinematics of Soft Robots created using Geometrical Constraints ensuring Safe Manufacturing [<a href="nielsen.pdf">pdf</a>]


<a name="schedule"/>
## Schedule <a href="#toc" class="top-link">[Top]</a>

**The most up-to-date schedule can be found on our *Google calendar***:
 [*[View](https://calendar.google.com/calendar/embed?src=cd5ddd82tddp4hjs0p8kacem9k%40group.calendar.google.com&ctz=Europe%2FBerlin&mode=AGENDA)*]
 [*[Subscribe](https://calendar.google.com/calendar?cid=Y2Q1ZGRkODJ0ZGRwNGhqczBwOGthY2VtOWtAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ)*]

|---------------|--------------------------------------------------------------------|
| 09:00 - 09:15 | *Welcome and introduction*                                           |
|---------------|--------------------------------------------------------------------|
|  | Session 1: Sim2real for Manipulation I  |
| 09:15 - 09:40 | **Kris Hauser**: *Real2sim: generalizable learning to simulate complex contact phenomena*                         |
| 09:40 - 10:05 | **Gilwoo Lee**: *Bayes-optimal reinforcement learning for sim2real adaptation*                                                    |
| 10:05 - 10:30 | **Chelsea Finn**: *Learning and Adapting in Diverse, Dynamic Environments* |                                         |
|---------------|--------------------------------------------------------------------|
| 10:30 - 10:45 | *Poster Teasers*                                                   |
|---------------|--------------------------------------------------------------------|
| 10:45 - 11:30 | Posters Session I / Coffee Break                                                   |
|---------------|--------------------------------------------------------------------|
|  | Session 2: Sim2real for Grasping |
| 11:35 - 12:00 | **Edward Johns**: *Zero-shot sim-to-real transfer for robotic grasping* |
| 12:00 - 12:25 | **Josh Tobin**: *Beyond Domain Randomization.*                               |
| 12:25 - 12:45 | **Yunfei Bai**: *Learning to grasp using simulation and deep learning* |
|---------------|--------------------------------------------------------------------|
| 12:45 - 13:30 | Lunch break                                                        |
|---------------|--------------------------------------------------------------------|
|  | Session 3: Sim2real for Locomotion |
| 13:35 - 14:00 | **Erwin Coumans**: *Sim-to-real for quadruped locomotion* |
| 14:00 - 14:25 | **Jean-Baptiste Mouret**: *Data-efficient Adaptation to Damage is a Reality Gap Problem* |
|---------------|--------------------------------------------------------------------|
| 14:30 - 15:15 | Posters Session II / Coffee Break                                                   |
|---------------|--------------------------------------------------------------------|
|  | Session 4: Sim2real for Manipulation I  |
| 15:20 - 15:45 | **Fereshteh Sadeghi**: *Domain Invariant Semantic Robot Navigation* |
| 15:45 - 16:10 | **Emo Todorov**: *Robustness of model-based control* |
| 16:10 - 16:35 | **Russ Tedrake**: *Robust full-stack manipulation (perception, planning, <br/>and control)  via simulation-based design and verification* |
|---------------|--------------------------------------------------------------------|
| 16:45 - 17:30 | *Speaker Panel Discussion*   |
|---------------|--------------------------------------------------------------------|

<a name="venue"/>
## Venue <a href="#toc" class="top-link">[Top]</a>

The workshop takes place in **Building 101, Room 00 026**.

The poster sessions takes place in **Building 101, Room 00 019**.

Please check out the [RSS website](http://roboticsconference.org/attending/venue/) and [Google maps](https://goo.gl/maps/2iwdEFKUh1m) for more detailed information on the workshop’s location.

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
