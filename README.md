<div align="center">

# Arsh Mann

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=C4B89A&center=true&vCenter=true&width=620&lines=Computer+Science+%40+Simon+Fraser+University;Data+%C2%B7+Software+%C2%B7+Cloud;Seeking+a+January+2027+co-op" alt="Computer Science at SFU · Data, Software, Cloud · Seeking a January 2027 co-op" />

<br/>

[![Email](https://img.shields.io/badge/asm32%40sfu.ca-1a1a1a?style=for-the-badge&logo=gmail&logoColor=C4B89A)](mailto:asm32@sfu.ca)
![AWS Certified](https://img.shields.io/badge/AWS_Certified_Cloud_Practitioner-1a1a1a?style=for-the-badge&logo=amazonwebservices&logoColor=C4B89A)
![Location](https://img.shields.io/badge/New_Westminster,_BC-1a1a1a?style=for-the-badge&logo=googlemaps&logoColor=C4B89A)

</div>

---

### About me

I'm a fourth-year Computer Science student at SFU who likes finding out whether a result can actually be trusted. Most of my work turns messy data into something a person can use: models that are evaluated honestly, packaged into tested code, and shipped as apps anyone can try.

- **Focus:** data analysis, machine learning, and the software around it
- **Also into:** systems programming, cloud infrastructure, and competitive programming
- **Off the keyboard:** competitive ice hockey since 2015

---

### Featured project

<table>
<tr>
<td>

#### Heart Disease Risk Screener

[![Live demo](https://img.shields.io/badge/Live_Demo-C4B89A?style=for-the-badge&logo=streamlit&logoColor=1a1a1a)](https://heart-risk-screener.streamlit.app/)
[![Source](https://img.shields.io/badge/Source-1a1a1a?style=for-the-badge&logo=github&logoColor=white)](https://github.com/arshmann2003/HeartDiseaseClassifier)

A web app that estimates heart-disease risk from 21 health-survey answers and explains which answers drive each person's estimate. It is trained on 253,680 CDC survey records.

The most important part was a bug that didn't crash anything: threshold tuning was leaking test data and making results look better than they were. I found it, rebuilt the evaluation with separate training, validation, and test sets, and added tests so it can't quietly return.

| Result | Value |
|:--|:--|
| Cases caught at the screening threshold | **81%** |
| Precision vs. base rate | **2.6×** |
| ROC-AUC (tuned gradient boosting) | **0.85** |
| High-risk subgroup found with K-Means | **5×** the overall rate |

`Python` `scikit-learn` `pandas` `Streamlit` `GitHub Actions`

</td>
</tr>
</table>

---

### Projects

<table>
<tr>
<td width="50%" valign="top">

#### Student Performance Predictor
[![Live demo](https://img.shields.io/badge/Live_Demo-C4B89A?style=flat-square&logo=streamlit&logoColor=1a1a1a)](https://gpa-predictor-amann.streamlit.app/)
[![Source](https://img.shields.io/badge/Source-1a1a1a?style=flat-square&logo=github&logoColor=white)](https://github.com/arshmann2003/student-performance-prediction)

Predicts GPA and exam scores from 9,000 student records across three public datasets. Every model was benchmarked against a simple baseline. The GPA model reached **R² 0.90**, within 0.23 GPA points on average. Absences predicted GPA far more strongly than study time.

`Python` `scikit-learn` `pandas` `Streamlit`

</td>
<td width="50%" valign="top">

#### Spring Maze
[![Source](https://img.shields.io/badge/Source-1a1a1a?style=flat-square&logo=github&logoColor=white)](https://github.com/arshmann2003/mazeApp)

A browser maze game with a JavaScript frontend and a Spring Boot REST API that creates mazes, stores game state, and takes every move. Most of the work was in the seam between the two: fixing integration bugs and documenting the API.

`Java` `Spring Boot` `JavaScript` `REST`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### Group Chat Server

A chat server in C that handles many clients at once over sockets, relaying messages in order and using non-blocking I/O to accept new connections without stalling.

`C` `Sockets` `Networking`

</td>
<td width="50%" valign="top">

#### QuickSum

A Chrome extension that summarizes web pages with the OpenAI GPT API, streaming the response so text appears right away instead of after a wait.

`JavaScript` `OpenAI API` `Chrome Extensions`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### Library Management System

A Python app on a SQLite schema I designed for members, loans, events, and staff tasks, with SQL for create, read, and update, and checks that records stay consistent after every action.

`Python` `SQL` `SQLite`

</td>
<td width="50%" valign="top">

#### Candy Factory Simulation

A multi-threaded producer–consumer simulation in C that uses semaphores to coordinate shared resources and reports production-to-consumption delays.

`C` `Threads` `Synchronization`

</td>
</tr>
</table>

---

### Currently building

- **Airlock Drop:** a private file-drop service on AWS. Uploads stay in a private S3 bucket until a Lambda check clears them, then get a short-lived download link. Built with `S3` `Lambda` `IAM`.
- **A relational database in C++:** a term-long course project using threads and manual memory management.

---

### Tech stack

<p align="left">
  <img src="https://skillicons.dev/icons?i=python,java,js,ts,c,cpp,r&theme=dark" alt="Python, Java, JavaScript, TypeScript, C, C++, R" />
  <br/>
  <img src="https://skillicons.dev/icons?i=sklearn,spring,sqlite,aws,git,githubactions,linux&theme=dark" alt="scikit-learn, Spring, SQLite, AWS, Git, GitHub Actions, Linux" />
</p>

`pandas` `NumPy` `matplotlib` `Streamlit` `SQL` `REST APIs`

---

### Certifications

![AWS](https://img.shields.io/badge/AWS_Certified_Cloud_Practitioner-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Google](https://img.shields.io/badge/Google_IT_Support_Professional_Certificate-4285F4?style=flat-square&logo=google&logoColor=white)

---

<div align="center">

**B.Sc. Computer Science, Simon Fraser University**

<sub>Algorithms · Systems Programming · Database Systems · Cybersecurity · Web Development · Computational Data Science</sub>

</div>
