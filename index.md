---
layout: default
---

<!--<div align="center">
<h3 style="font-color: darkgreen;">NEWS: Camera-ready of accepted papers & speakers slides are online</h3>
</div>

----
-->
<a name="toc"/>

<div style="text-align: center; font-size: 0.8em;">
<a href="#overview">Overview</a> &middot;
<a href="#debaters">Invited Debaters</a> &middot;
<a href="#topics">Topics</a> &middot;
<a href="#call">Call for Contributions</a> &middot;
<a href="#dates">Important Dates</a> &middot;
<!--<a href="#papers">Accepted Papers</a> &middot;-->
<a href="#schedule">Schedule</a> &middot;
<!--<a href="#venue">Venue</a> &middot;-->
<a href="#organizers">Organizers</a>
</div>

----

<a name="toc"/>

<div style="text-align: center; font-size: 0.8em;">
Previous Workshops:
<a href="./rss2019">RSS 2019</a>
</div>

----

<a name="overview"/>

Physical simulation is an important tool for robotic manipulation. While simulation has been well-established for robotics education and integrated robot software testing for a long time, only recently the robotics community has made significant progress in transferring manipulation capabilities learned in simulation to reality, a concept termed Sim2Real transfer.

Sim2Real draws its appeal from the fact that it is much faster, cheaper, safer and more informative to perform experiments in simulation than in the real world. Recent advances in Sim2Real have shown how to make advances in solving difficult robotic problems, such as autonomous driving, grasping or in-hand manipulation using Sim2Real techniques. However, Sim2Real still faces significant challenges, and it remains an open question whether Sim2Real techniques will ever reach the sample efficiency and accuracy of techniques based on real-world experimentation, and whether they will scale to realistic problem domains.

In this workshop we invite well-known researchers to debate the state of the art and the impact of Sim2Real on robotics. The workshop will primarily consist of debates focussed on controversial key topics with a few spotlight presentations.

<!--
1. **Contact simulation**: Manipulation is about contact. However, simulating physics and in particular contact is a highly complex problem. The reason is that contact formation depends on a wide variety of physical properties such as friction, object deformability, etc. Since learning-based methods exploit any circumstance that facilitates finding a solution, they are prone to overfit to imprecise modeling and thus fail to learn transferable policies.
2. **Simulating closed-loop manipulation**: Manipulation is not a single-shot but a temporal process. Therefore, even slight errors at the beginning of a simulation sequence tend to accumulate and then lead to simulating unrealistic behavior and learning non-transferable policies.
3. **Curse of dimensionality**: Many state-of-the-art approaches to sim2real rely on sampling a large number of policies and environmental conditions. However, sampling becomes exponentially more difficult with the number of task dimensions. This raises the question whether current techniques will scale to the high-dimensionality of manipulation problems, e.g. involving high-DOF manipulators.
4. **Sensor fidelity**: Certain sensor modalities are much more difficult to simulate than others, e.g. simulating RGB or force/torque is more challenging than depth. Despite the recent advances in image synthesis and domain transfer techniques, we still do not fully understand what statistical properties of sensors need to be simulated in order to successfully learn from them.
-->

The goal of this workshop is to debate the state of the art and the impact of Sim2Real for robotics. Here, Sim2Real refers to a concept of transferring robot skills acquired in simulation to the real robotic system. Sim2Real draws its appeal from the fact that it is cheaper, safer and more informative to perform experiments in simulation than in the real world. Yet, Sim2Real faces significant challenges. 

The proposed workshop is the second edition of a <a href="./rss2019">workshop held at R:SS 2019</a>. The R:SS 2019 had the goal of surveying the state of the art in Sim2Real for robotics, with a focus on robotic manipulation, and featured invited talks from top researchers in the field of Sim2Real. In this year’s edition, we aim to review the actual progress in Sim2Real more critically by changing the workshop format: inspired by the ICRA 2019 robotic debates workshop, for this workshop we will invite top-researchers to participate in debates focussed on controversial key topics with a few spotlight presentations.


<a name="debaters"/>
## Invited Debaters <a href="#toc" class="top-link">[Top]</a>

- **Dieter Fox** (University of Washington and Nvidia Research)
- **Chris Atkeson** (Robotics Institute, Carnegie Mellon University)
- **John Leonard** (MIT) 
- **Ken Goldberg** (UC Berkeley and UCSF)
- **Abhinav Gupta** (Robotics Institute, Carnegie Mellon University)
- **Jan Peters** (Technische Universität Darmstadt, MPI for Intelligent Systems)
- **Karen Liu** (Georgia Tech)
- **Anca Dragan** (UC Berkeley)
- **Peter Welinder** (OpenAI)
- **Shuran Song** (Columbia University)
- **Martha White** (University of Alberta)


<a name="topics"/>
## Topics <a href="#toc" class="top-link">[Top]</a>

In contrast to the R:SS 2019 edition, we changed the format from invited talks to **debates**. Each debate will focus on a key - rather controversial - statement regarding Sim2Real, and will be discussed by two proponents and two opponents of that statement. Each debate consists of short introductory pitches by the two sides, providing an opportunity to presenters to also highlight their work, followed by a moderated discussion. An example list of statements includes: 

> "Sim2Real will never work for complex robotic tasks";

> "Sim2Real is able to successfully leverage inaccurate simulations - accurate physics-based simulation and photo-realistic rendering is not required"; 

> "Sim2Sim performance is sufficient to indicate progress in Sim2Real"; 

> "Sim2Real is nothing more than system identification / model-based RL". 

We will coordinate with panelists regarding the phrasing and the selection of the statements as well as the assignment of panelists upon the acceptance of the workshop


<a name="call"/>
## Call for Contributions <a href="#toc" class="top-link">[Top]</a>

Please stand by. This information will be published if the workshop gets accepted. 
We will be accepting 2 page extended abstracts.

<!--
Participants are invited to submit **extended abstracts (maximum 2 pages in length, excluding references)** related to the aforementioned topics.

Accepted abstracts will receive a poster presentation slot and, if equipment is available, a video presentation slot during the poster session.

* Submissions must not exceed *2 pages in length, excluding references*.
* Submissions must be in PDF following the IEEE style available from<br/>
  [https://www.ieee.org/conferences/publishing/templates.html](https://www.ieee.org/conferences/publishing/templates.html)
* Submissions must include a short abstract. The *extended abstract* should go in the main section of the template and the *short abstract* in the abstract section.

**Submission website:** [https://cmt3.research.microsoft.com/SIMREALRM2019](https://cmt3.research.microsoft.com/SIMREALRM2019)
-->


<a name="dates"/>
## Important dates <a href="#toc" class="top-link">[Top]</a>

- Workshop Acceptance Notification: March 6, 2020
- Potential Workshop Dates: July 12/13, 2020

<!--
* Submission Deadline: June 3, 2019 <s>May 31, 2019</s>
* Notification of Acceptance: **June 17, 2019** <s>June 14, 2019</s>
* Camera ready submission: June 21, 2019 <s>June 19, 2019</s>
* Workshop: June 23, 2019 (full day)
-->

<!--
<a name="papers"/>
## Accepted Papers <a href="#toc" class="top-link">[Top]</a>

* Adam Allevato, Elaine Short, Mitch Pryor, Andrea Thomaz - TuneNet: One-Shot Simulation Tuning for Physics Prediction and Robot Task Planning [<a href="assets/papers/allevato.pdf">pdf</a>]
* Brayan S. Zapata-Impata, Pablo Gil, Fernando Torres  - vision2tactile: Feeling Touch by Sight [<a href="assets/papers/zapata.pdf">pdf</a>]
* Diego Ferigo, Silvio Traversaro, Daniele Pucci  - Gym-Ignition: Reproducible Robotic Simulations for Reinforcement Learning [<a href="assets/papers/ferigo.pdf">pdf</a>]
* Eric Heiden, David R Millard, Gaurav Sukhatme  - Real2Sim Transfer using Differentiable Physics [<a href="assets/papers/heiden.pdf">pdf</a>]
* Jakob Hollenstein, Justus Piater  - Evaluating Planning for Policy Search [<a href="assets/papers/hollenstein.pdf">pdf</a>]
* Jonas Kiemel - PaintRL: Coverage Path Planning for Industrial Spray Painting with Reinforcement Learning [<a href="assets/papers/kiemel.pdf">pdf</a>]
* Joshua P. Powers, Dylan Shah  - Sim2real of soft-bodied, shape-changing robots [<a href="assets/papers/powers.pdf">pdf</a>]
* Kent A. Rosser - Sim2real transfer degrades non-monotonically with morphological complexity for flapping wing design [<a href="assets/papers/rosser.pdf">pdf</a>]
* Manuel Kaspar, Jürgen Bock - Reinforcement Learning with Cartesian Commands andSim to Real Transfer for Peg in Hole Tasks [<a href="assets/papers/kaspar.pdf">pdf</a>]
* Max K. Nielsen - Data Driven Inverse Kinematics of Soft Robots created using Geometrical Constraints ensuring Safe Manufacturing [<a href="assets/papers/nielsen.pdf">pdf</a>]

-->

<a name="schedule"/>
## Schedule <a href="#toc" class="top-link">[Top]</a>

Taking inspiration from the ICRA 2019 Debates on the Future of Robotics Research, the workshop will consist of three debates. Every debates focuses on a single key question and is structured as follows:
Poster teasers related to debate topic (3-5 minutes each depending on number)
Pitch by proponents (2 researchers), 15 minutes 
Pitch by opponents (2 researchers), 15 minutes
Debate, 45 minutes

We will be soliciting poster submissions for the workshop. We will review the contributions by putting together a program committee with experts in the field. We will have two poster sessions during the coffee breaks along with teaser presentations.

We will conclude the workshop with a panel discussion focusing on the question on how Sim2Real and real-world experimentation can be combined in the best way to achieve the best of both worlds.


<iframe class="cal" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRK0fRQC4gP6nuXUvxKSfwrl-bJhn3SSMJrqArG1JrdnO1siDzuKBipDb20h8A4MirZ7PPppbY_NcLm/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

<!--
<a name="venue"/>
## Venue <a href="#toc" class="top-link">[Top]</a>

The workshop takes place in **Building 101, Room 00 026**.

The poster sessions takes place in **Building 101, Room 00 019**.

Please check out the [RSS website](http://roboticsconference.org/attending/venue/) and [Google maps](https://goo.gl/maps/2iwdEFKUh1m) for more detailed information on the workshop’s location.
-->

<a name="organizers"/>
## Organizers <a href="#toc" class="top-link">[Top]</a>


| <img src="assets/images/shoefer.jpg" alt="Sebastian Höfer" width="300" /> | [Sebastian Höfer](http://www.sebastianhoefer.de) is an applied scientist at Amazon Robotics AI headed by Siddhartha Srinivasa. Before joining Amazon, he received his Ph.D. with Oliver Brock at Technische Universität Berlin. 

| <img src="assets/images/kostas.jpg" alt="Kostas Bekris" width="300" />  | [Kostas Bekris](https://robotics.cs.rutgers.edu/pracsys/members/kostas-bekris/) is an Associate Professor at the Computer Science department of Rutgers University and an Amazon Scholar at the Amazon Robotics AI team headed by Siddhartha Srinivasa. He received his PhD with Lydia Kavraki at Rice University.  |

| <img src="assets/images/ankur.jpg" alt="Ankur Handa" width="300" />  | [Ankur Handa](https://ankurhanda.github.io/) is a senior research scientist at NVIDIA robotics lab run by Dieter Fox. Prior to that he was a research scientist at OpenAI. He received his Ph.D. with Dr. Andrew Davison and spent two years at University of Cambridge in Prof. Roberto Cipolla’s lab as a post-doctoral researcher.  |

| <img src="assets/images/juan.jpg" alt="Juan Camilo Gamboa Higuera" width="300" />  | [Juan Camilo Gamboa](https://cim.mcgill.ca/~gmaboa ) is a PhD Candidate at the School of Computer Science at McGill University. His research focuses on model-based RL for control and navigation of underwater vehicles.  |

| <img src="assets/images/florian.jpg" alt="Florian Golemo" width="300" />  | [Florian Golemo](https://fgolemo.github.io/) is a postdoctoral fellow at Mila and ElementAI, working with Liam Paull, Aaron Courville, and Chris Pal on Sim2Real and 3D perception problems. He received his PhD from INRIA Bordeaux under supervision of Pierre-Yves Oudeyer.  |

| <img src="assets/images/melissa.jpg" alt="Melissa Mozifian" width="300" />  | [Melissa Mozifian](https://melfm.github.io/about.html) is a PhD Candidate at the School of Computer Science at McGill University. Her research focuses on deep reinforcement learning and transfer for control of robot manipulation tasks.  |
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
