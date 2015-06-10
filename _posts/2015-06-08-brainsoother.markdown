---
layout: post
title:  "B C I"
date:   2015-03-13
link:	
excerpt: discovering stress in the human brain and inducing calmness
color:  "#000000"
bgimage: "./assets/bci_cover2.jpg"
---

In June 2015, I attended [Angel Hacks](http://angelhack.com/hackathon/montreal-2015// "Title") in Montreal. My team (Philippe Castonguay, Yusaira Khan, Maksim Sen) and I built a BCI application called 'Brain Soother'. 

## Brain Computer Interface (BCI)

A brain-computer interface is a direct communication pathway between the brain and an external device with the purpose of assisting, augmenting, or repairing cognitive and/or motor functions.  The computer measures electrical activity in the brain by means of an electroencephalogram (EEG) and interprets the signals for display.

As brain and other biometric measures are obtained, rapid analysis of the information is converted into graphical displays of the individual’s cognitive, emotional, and stress states. Cloud-based computing allows for near real-time display and analysis of the results. This system allows doctors to quickly measure the brain and then safely modulate certain regions using various techniques.

One approach is the use of transcranial direct current stimulation (tDCS), a form of neuro-stimulation using constant, low current delivered directly to a specific area of the brain via small electrodes. However, the approach we chose instead uses visual stimualtion to generate electrical activity at the same frequency, thus imitating the stimuli.

In neurology, Steady State Visually Evoked Potentials (SSVEP) are signals that are natural responses to visual stimulation at specific frequencies. When the retina is excited by a visual stimulus ranging from 3.5 Hz to 75 Hz, the brain generates electrical activity at the same (or multiples of) frequency of the visual stimulus.

We used the science behind SSVEP in order to evoke signals to test our goal of reducing stress and inducing calmness in users. In addtion to a visual stimuli, we used auditory stimuli at the same frequency to test our hypothesis. In the future we would like to explore stimulating the human brain using more senses such as haptics in order to work towards a healthier brain.


![Hackathon](/assets/bci_devices.jpg)


##Motivation

More than [20 percent of Americans regularly consume prescribed drugs related to mental health issues](http://www.newyorker.com/tech/elements/the-psychiatric-drug-crisis // "Title"), earning contemporary America the nickname, “the Prozac Generation.”  However, developing safe, targeted, and effective drugs for mental illnesses has increasingly become a struggle for the pharmaceutical industry.

Due to the complexity of brain networks, these pharmaceutical compounds may work to alleviate some symptoms, but they may exacerbate others. The diagnosis of many conditions is a highly subjective process based on patient self-reporting and thus identifying the appropriate course of treatment is frequently trial and error.

We believe we are moving into a post-pharmaceutical age in the treatment of neurological and psychiatric illness. With the flurry of wearable sensors, brain-computer interfaces, and non-invasive brain stimulation research we see a new type of treatement related to cognition, behavior, and emotion. Thus, we see potential for patients with insomnia, paralysis, ADHD and MS.


![SSVEP](/assets/SSVEP.jpg)
- [Architecture of a typical brain–display interactive system. SSVEP: Steady-state visual evoked potential.](http://spie.org/x113409.xml// "Title")

##Tinkering


In order to achieve this we used an [openBCI](http://www.openbci.com// "Title"), scraped the data, analysed it, ran a Fast Fourier Transform (FFT) on it and used this frequency to create a visual and auditory stimulus on a web app. 

In terms of hardware, openBCI was easy to set up, had a great GUI, a helpful developer community (Thanks [Conor](https://twitter.com/russomanno15 // "Title")!), was fleixble in terms of use cases and I would totally recommend it to makers and tinkerers in the human-computer interaction domain! 

We used flickering red lights to create an imperceptible flickering visual stimulus that can elicit a strong SSVEP. 

##Prototype

Although you wouldn't be able to hear the audio and feel it in real time, here's what the visual looked like at one point.

![GIF](http://i.imgur.com/UuubiLp.gif)

##Team

![Team](/assets/teambci.jpg)

