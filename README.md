# brain-worm

## Who

The team is formed of people coming from significatly different areas of arts, engineering, and psychology:

* [**Krystof Kaplan**](http://artalk.cz/tag/krystof-kaplan/) is an artist and also the author of kinetic worm designed for BCI, neuro-feedback, and for exploring new ways of movement.
* [**Vlastimil Koudelka**](http://www.nudz.cz/en/employee/?id=497) is an engineer and researcher in neuro-imaging, machine learning, and optimization
* [**Dmitri Berzon**](http://www.lunchmeat.cz/en/events/lunchmeat-festival-2014-173/artists/dimitri-berzon--ru---frances-sander--uk--visual--211.html) is a Concept developer / Light designer, Programmer, Conceptual artist specializing in interactive installations
* [**Cyril Kaplan**](https://www.researchgate.net/publication/300082527_Personal_Conceptions_of_Death_in_Young_Czech_Adults) is a psychologist specializing on EEG correlates of mental and emotional activity, music producer, openVibe and PD programmer. 

Many thanks go to **Martin Zrzek** who programmed a VVVV sequencer to record, read, and play the worm movements.

## What

![alt text](https://github.com/HackTheBrain/brain-worm/blob/master/worm_pics/P1070909.JPG "A kinetic worm")

A kinetic worm needs your attention! Once it realizes you are concentrated it will use pneumatic muscles and move. If you are not focused enough the worm stops moving and starts breathe frequently. The level of your concentration is measured via electrical brain waves (EEG). 

## Why

**A sculpturer**

A couple years ago I started creating a toy for my recently born daughter. Generally, I was interested in objects addressing rather the abstract form of the world. Thus, I designed a wooden puppet consisting of several various pieces which also made sounds when it was moved. This really changed my approach to the sculpturing and it has been influencing me even now. One of such abstract objets is also a brain worm designed for hackathon event. The brain worm consists of many segments exhibiting slow movements which look like a micro-organism or a big whale if looking from a different perspective.

**An engineer**

Slow and big pneumatic kinetic worm which would move in accordance to very fast and noisy changes in human EEG signal seemed to me an impossible goal with unclear outcomes. This challanging idea driven me to join in the project. A couple years ago I studied automation so that I could formulate the brain worm as a soft-robot. I was really interested in what is possible to do with the worm, how it can move, and which parameters from EEG would correspond to the worm dynamics. The process of making the worm alive began form the physical layer (basic muscle patterns) and then more and more abstract layers could be added. This resulted in rather a specific set of EEG parameters which could be used. 

## How

The kinetic worm can move and breathe using its pneumatic muscles made of 24 tires. Extra eight tires are constantly inflated and form a sculpture skeleton. 

Solenoid valves are connected to a computer interface such that synchronous patterns of movements can be created within [VVVV](https://vvvv.org/) environtment. The IDE can also receive UDP messages from real-time EEG analysis tools. [OpenVibe](http://openvibe.inria.fr/) and [PureData](https://puredata.info/) are used and tested in our project.

OpenVibe is connected to NeuroSky Mindwave mobile device and further analyzes the eeg stream to obtain a robust eeg marker of participants concentration. Relative frontal alpha power was chosen to measure a level of concentration. 

Once the participant reach some threshold of the EEG parameter VVVV drives the worm in a sequence of movements. If the concentration drops below the threshold VVVV drives the worm to simulate fast breathing.


## Ethical considerations
The brainworm informed audience (via its movements) about participants state of consciousness. This could cause a hypothetical social issue during or after the performance. On the other hand, we could inform participants before the beginning of their trial.
