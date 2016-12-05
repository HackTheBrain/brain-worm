# brain-worm

## Who

The team is formed of people coming from significatly different areas of arts, engineering, and psychology:

* **Krystof Kaplan** is an artist and author of kinetic sculpture designed for BCI, neuro-feedback, and for exploring new ways of movement.
* **Vlastimil Koudelka** is an engineer and researcher in neuro-imaging, machine learning, and optimization
* **Dmitri Berzon** is a Concept developer / Light designer, Programmer, Conceptual artist specializing in interactive installations
* **Cyril Kaplan** is a psychologist specializing on EEG correlates of mental and emotional activity, music producer, openVibe and PD programmer. 

## What

![alt text](https://github.com/HackTheBrain/brain-worm/blob/master/worm_pics/P1070909.JPG "A kinetic worm")

A kinetic worm needs your attention! Once it realizes you are concentrated it will use pneumatic muscles and move. If you are not focused enought the worm stops moving and starts breathe frequently. The level of your concentration is measured via electrical brain waves (EEG). 

## Why

**A sculpturer**

A couple years ago I started creating a toy for my recently born daughter. Generally, I was interested in objects addressing rather the abstract form of the world. Thus, I designed a wooden puppet consisting of several various pieces which also made sound when it was moved. This really changed my approach to the sculpturing and it has been influencing me even now. A particular example of my object is the brain worm designed for hackathon event. The brain worm consists of many segments exhibiting slow movements which look like a micro-organism or a big whale if you look at it from a different perspectives.

**A engineer**



## How

The kinetic worm can move and breathe using its pneumatic mussels made of 24 tires. Extra eight tires are constantly inflated and form a sculpture skeleton. 

Solenoid valves are connected to a computer interface such that a synchronous patterns of movements can be created within [VVVV](https://vvvv.org/) environtment. The IDE can alse recieve UDP messages from realtime EEG analysis tools. OpenVibe and PureData are used and tested in our project.

OpenVibe is connected to NeuroSky Mindwave mobile device and further alyzes the eeg stream to obtain a robust eeg marker of participants concentration. Relative frontal alpha power was chosen to measure a level of concentration. 

Once the participant acceeds same treshold of the parameter VVVV drives the worm in a sequence of movements.


## Ethical considerations
*please share the insights about ethical matters surrounding your work. Some "ethical cards" have been distributed to support the discussion about this subject.*
