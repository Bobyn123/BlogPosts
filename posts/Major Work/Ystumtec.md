
# Ystumtec

Ystumtec is (or was depending on when you read this) a small company based in mid Wales headed up by Mark Neal, a former lecturer from Aberystwty university who as he puts it "got fed up with university paper work" and used his industry contracts to be able to focus on intresting projects.

I first came into contact with Ystumtec during my 2nd year of university when Mark put out an advertisment looking for a student to do an industrial year with Ystumtec working on a computer vision project looking at marine animals. I applied, interviewed and....didn't get the job, but Mark did say he had some part time summer work for me if I was intrested.

For the absence of doubt, I have been given permission to talk about these project in this level of detail by Mark, and the company is shutting down soon anyway.

## GPS collars

The concept for the GPS collar project was to make a low cost, low power, remote release GPS tracking collar and basestation for wildlife tracking. A few intresting features of the collar:

- It ran on an atmega328p (arduino) and then later an esp32 when the demand for flash memory exceeded the arduino. 
- User set schedules for waking and sampling GPS location.
- A remote basestation (also atmega328p) that collars would attempt to contact everytime they woke up to offload a distributed sampling of their recorded data to.
- The collar had a remote release system that could be triggered by low battery or remote communication with a basestation.

As a first project this was pretty much perfect for me, having already gotten a reasonable amount of experiance writing arduino C as part of my first year of university and my robotics work in the robotics society. I got to learn a lot about low power radio transmission with a rfm95w, custom memory flash memory management and two way coms over radio.

The radio project also involved a fair bit of fieldwork, range testing, testing the remote release, live testing on sheep which I really enjoyed.

So Mark had me work on this project piecemeal over the summer and at the end of the summer he wound up offering me an industrial year job anyway, so I continued working on the GPS collar and a few other projects for the next year.

## XY spray rig

The XY spray rig (just rolls off the tongue) was a bespoke project we made for an agricultural testing company. Its design was a fairly simple XY motion gantry with a spray nozzle, it allowed for automated testing of targeted spraying of plants via user selection from a camera placed above the work area.

I worked on this project in conjunction with the other industrial year student, she did the user interface, I did the middleware to communicate with the embedded control systems and the camera system. We wrote the project in java and the GUI in javaFX, and if I have any say in the matter I will never work with javaFX again.

In this project I found a lot of valuable experiance working as a team, specing out requirements and interfaces with my coworkers and then working on them individually, understanding (and somtimes misudnerstanding) what the client wanted and how they would use the machine.

I also learnt about openCV, camera undistortion, standarizing serial communication procedures and interacting with a GUI front end.

## Moth traps

The moth trap project was intended to produce an early warning sensor for detecting a species of swarming invasive moth in agricultural areas to reduce overuse of insecticides. The sensor was a fairly simple design, intended to be manufactured cheaply with as many off the shelf parts as possible to enable easy construction and repair. It was a standard insect trap with moth phereamones inside and some sensors to try and detect everytime an insect entered the trap, with the hope being that a significant uptick of insects would be a significant indicator of the presence of the specific swarming moth species.

For this project, I was tasked with writing the embedded C code (arduino C again), this again involved low power scheduling, to operate at sunrise and sunset (moths are Crepuscular) however instead of low power radio, and to wake and log each time the sensor flagged an insect, and communication with a GSM module, the intent being to use existing mobile phone infrastructure to communicate with a central server.

## Going full time

After my final year of university I was offered a fulltime job with Ystumtec which having had such a good time of it in my industrial year, I was excited to return to.

## FAUV

The FAUV, oh the FAUV, bane and joy of my existence.

## xArm Rig

The xArm rig 
