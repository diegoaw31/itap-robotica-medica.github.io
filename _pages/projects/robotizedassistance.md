---
title: "ITAP Medical Robotics"
layout: textlay
excerpt: "ITAP Medical Robotics"
sitemap: false
permalink: /projects/robotizedassistance
---

<br>
### Robotized System for the Regulation of Assistance in Rehabilitation Tasks of Higher Members, Using Physiological Signs of the Autonomous Patient Nervous System

<b>Funding Entity:</b> Ministry of Science and Innovation.  
<b>Reference:</b> DPI2009-10658  
<b>Participating entity:</b> CARTIF  
<b>Duration:</b> 01-December-2009 - 30-November-2010  

---

The robotic platform for rehabilitation tasks of the upper limbs that was developed consists of a white room robot Stäubli RX90 of 6 degrees of freedom, equipped with a force / torque sensor JR3, mounted on the end effector of the robot. This sensor provides us with information about the haptic interaction between the robot and the patient.

In order to use the robotic rehabilitation platform with patients suffering from spasticity, a hand-forearm antispastic orthosis has been designed, coupled to the robot's force / torque sensor by means of a quick coupling mechanism, using electromagnets. The coupling / uncoupling of this antispastic orthosis can be carried out in manual mode, using manual control of the physiotherapist, or in automatic mode, through the control signal coming from a Beckhoff BK5200 DeviceNet device, which interfaces with the controller of the robot. By means of a control signal coming from the safety chain, or from the speed / force observer, it is possible to uncouple the patient from the orthosis, in a fast and safe way. It is also regulated, by means of a potentiometer, a force threshold, above which the orthosis will uncouple safely, preventing the robot from causing harm to the patient.

<img src="{{ site.url }}{{ site.baseurl }}/images/assistance_proj.png" class="img-responsive" width="100%" />

The Biopac MP 150 system measures and records different physiological signals of the patient "on-line", and allows the registration of them on an external PC through a UDP / IP link. Using a series of amplifiers and filters specially designed for each type of signal, we can take Electrocardiogram (ECG) records, - from which the heart rate (HR - Heart Rate) and other parameters of the signal are obtained -, galvanic response of the skin (GSR - Galvanic Skin Response) and skin temperature (SKT). These signals are captured at 100hz, filtered, processed "on-line", and finally stored in a SQL database, in such a way that they are easily accessible for further analysis.

To the security software that the robot owns by default, two layers of software have been added that increase the security of the robotic rehabilitation platform. The first layer is at the haptic level. These are virtual walls that exert an infinite impedance outside the working plane of the robot, defined as "safe plane". This prevents the robot from entering a configuration close to its singular points, and its joints moving at high speeds. The second layer of security software is formed by a speed / force observer, which in case of recording a dangerous situation (speed or force above a preset maximum value), provides a control signal that frees the patient from the orthosis , and dampens the movement of the robot.

---

<div class="col-md-4">
<a href="https://www.cartif.es/">
<img src="{{ site.url }}{{ site.baseurl }}/images/CARTIF.png"  class=" img-responsive" />
</a>
</div>

<div class="col-md-4">
<a href="https://ec.europa.eu/regional_policy/es/funding/erdf/">
<img src="{{ site.url }}{{ site.baseurl }}/images/feder.jpg"  class=" img-responsive" />
</a>
</div>

<div class="col-md-4">
<a href="https://www.ciencia.gob.es/">
<img src="{{ site.url }}{{ site.baseurl }}/images/logo_ciencia.png"  class=" img-responsive" />
</a>
</div>