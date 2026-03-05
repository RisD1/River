## Stage 1 Requirements 

Smart Login with role-based dashboards + Face Recognition (OpenCV)
Task Assignment & Monitoring — Kanban board (To-Do → In-Progress → Completed)
"Black Box" Recorder — History log of every action, who did it, when
Clean responsive interface for phones & PCs

## Aproach
### 1. Smart Login with role-based dashboards + Face Recognition (OpenCV)
Within any organization, a single individual may be a part of several projects with varying roles. Hence, the "role-based dashboard" 
will also be different from project-to-project. These configurations may be set by the "project lead"/admin. Hence, right now, I will 
only include a basic login system. The role-logic will be handled later on in development.

Facial Recognition.
This is the most challenging part of the login implementation. Traditional methods ((like Haar Cascades and Eigenfaces/LBPH) are easily 
confused. OpenCV’s DNN is safer because it uses "Deep Learning"  to recognize complex facial geometry. 
(Live Detection is also necessary to prevent spoofing.)

I'm thinking YuNet + SFace because it is a lightweight, industry-standard DNN pair used in professional security systems.

Also, I'll make facial recognition an opt-in feature. Doesn't really seem necessary in most "project management" contexts. 

