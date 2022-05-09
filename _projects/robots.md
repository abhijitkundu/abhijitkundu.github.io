---
layout: page
title: Robots
description: A few of my old amateur robots.
img: assets/img/robots/irat0.gif
importance: 3
category: hobby
---

## iRAT

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
    	<p>
        iRAT is a micromouse development kit developed at <a href="https://www.crunchbase.com/organization/thinklabs-in/">Thinklabs</a>, a robotics startup in India. I worked on this project as an intern at Thinklabs in 2007 along with Anand Ramaswami of Thinklabs. iRAT is a modular micromouse development platform; it has both top-down and sidewall sensors so the user can choose any sensor approach he likes.
    	</p>
    	<p> iRAT is based on the <a href="http://www.atmel.com/dyn/products/product_card.asp?part_id=2014">AVR ATmega32</a> RISC controller running at 16MIPS. It has two high-torque stepper motors, which can be over driven with the on-board current chopper circuitry. The board also has LEDs, buzzer, LCD, and UART port for easy debugging. A simulator along with some sample code has also been developed.
    	</p>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="../../assets/img/robots/irat0.gif" title="irat image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Indur

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
    	<p>
        Indur was my entry at the international <a href="http://en.wikipedia.org/wiki/Micromouse">micromouse</a> event at <a href="http://www.techfest.org/">Techfest 2008</a>, which is held every year at <a href="http://www.iitb.ac.in/">IIT Bombay</a>. This was my first micromouse entry for a competition.
        </p>
		<p>
		<i>Indur</i> means mouse in Bengali. This robot was developed rather very quickly, in just a month. As a result, I didn't have time to optimize the PID routines to acheive perfectly straight runs, and Indur didn't perform to my expectation. Despite this, Indur still made to the finals in Techfest 2008 micromouse event, and was among very few robots to reach the centre of the maze. 
		</p>
<!-- 		<p>
		Specification:
		Motors: 2 x Stepper motors
		Battery: 6x li-ion
		DC-DC converter: PTN78000W (free sample from TI)
		CPU: AVR ATmega 32
		Motor driver: Allegro A3982 (free samples from Allegro)
		IR transmitter : OPE5594 (sourced from RS components)
		IR receiver : TSL262R (same as above)
		StraightSpeed: 1.9 m/s
		Acceleration:2.4 m/s/s
		Software: Flood-fill algorithm, In-place turns
		</p> -->
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="../../assets/img/robots/indur0.jpg" title="Indur image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


## Robots at the IIIT Hyderabad Robotics Lab

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
    	<p>
        During my time at <a href="http://robotics.iiit.ac.in/">Robotics Research Lab</a> of <a href="http://iiit.ac.in/">IIIT Hyderabad</a>, I worked on several (professional) robot platforms. I predominantly made use of the <a href="http://www.mobilerobots.com/researchrobots/researchrobots/pioneerp3dx.aspx">Pioneer P3DX</a> and the new (at the time) <a href="http://www.mobilerobots.com/researchrobots/researchrobots/P3AT.aspx">P3AT</a> robot. With this platform, we implemented and developed various vision algorithms to develop a mobile robot that can interact and assist people in a home/office environment. I also worked heavily with stereo and monocular cameras and SICK laser scanners mounted on the poineer robots. We also used these robots for a mobile robotics course at <a href="http://iiit.ac.in/">IIIT Hyderabad</a> for which I was both a student and teaching assistant.
    	</p>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="../../assets/img/robots/iiith_robots.jpg" title="IIIT Robots image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


## MERP

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
    	<p>
        MERP is a mobile robot platform that I designed and developed as a testbed for robotics learning and research. The objective was to create a cheap, modular, easy to debug robot platform, both at the hardware and software level. With this platform, I implemented and developed various vision algorithms to create a mobile robot that can interact and assist people in a home/office environment. Some of the abilities of the robot are:
		<ol>
		  <li>Speech based interaction and command execution.</li>
		  <li>Face detection and face/person tracking.</li>
		  <li>Vision based person following.</li>
		  <li>Ability to read text messages and symbols.</li>
		</ol>
		This platform was built with economical off-the-shelf equipments, which should be accessible to hobbyists and home users. The main components of the platform include an onboard laptop, three AVR ATmega uc, a webcam, two dc-geared motors, pan and tilt mechanism for webcam mounting, and dc-dc converters for power management.
		</p>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="../../assets/img/robots/merp1.jpg" title="merp image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


## MousEye

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
    	<p>
        This small robot can move around and scan the surface underneath it. The idea of building this robot came after coming across <a href="http://spritesmods.com/?art=mouseeye">this article</a> on mouse scanners. Optical Mice generally use tiny CCD sensors. The mouse I hacked has an <a href="http://www.avagotech.com/products/optical_navigation_sensors/led-based_sensors/adns-2610/">ADNS-2610</a> chip. It has a 18x18 CCD matrix. It is programmable and gives it's output serially (SPI interface).
        </p>
        <p>
		Though the images produced are not very visually appealing, it can be used like poor man's document scanner. I interfaced the ADNS-2610 with my PC parallel port and made a simple GUI to show the scanned picture. I also attached two small DC motors to the mouse, so you can just sit back in your chair and just click few buttons to move the 'MousEye' robot and scan all the parts of the document you need.
		</p>
		<p>
		The sensor chips in the optical mice like the ADNS-2610 give displacement readings, and thus can be used as alternative to conventional wheel encoders.
		</p>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="../../assets/img/robots/mouseye3_2.jpg" title="MousEye image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


## Maze Solver

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
    	<p>
        Maze Solver is an autonomous robot that attempts to solve a maze with the help of an overhead camera using image processing principles. I built this robot for a robotics competition at <a href="http://www.iitg.ernet.in/">IIT Guwahati's</a> annual techfest, <a href="http://www.techniche.in/">Techniche'06</a>.
    	</p>
    	<p>
		The objective was to build a robot that could solve a maze in the shortest time possible by avoiding the color-coded obstacles (white unmovable, red: movable) with help of a overhead camera. The images from the overhead webcam were processed on a desktop computer, which then sent movement commands to the robot.
		</p>
		<p>
		In solving the maze, the first task is to localize the robot in the arena using the overhead camera. A simple pattern on the robot is used to track it and find its orientation. Then it needs to differentiate between movable path and obstacles. Next it has to find the circular landmark and calculate the shortest route to it. Finally it drives the bot along this route to its target.
		</p>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="../../assets/img/robots/mazesolver0.jpg" title="Maze Solver image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


## Apocalypse

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
    	<p>
        Apocalypse is a line following robot; it also has obstacle detection sensors. It won 1st prize at 3 robot competitions. Apocalypse clocked the fastest time of 15 seconds at a line following event in Edge at Techno India, Kolkata. The 2nd fastest time at the event was 26 seconds. Apocalypse also won the <a href="http://www.youtube.com/watch?v=AXHqOU20SOg/">Sliding Door</a> event (a maze solving contest), crossing the whole grid in 22 seconds.
        </p>
        <p>
		Apocalypse uses an Atmel AVR <a href="http://www.atmel.com/dyn/resources/prod_documents/2486S.pdf">ATmega8</a> microcontroller as its "brain". <a href="http://www.st.com/stonline/books/pdf/docs/1330.pdf">L293D</a> is used as motor driver for two geared dc motors. LDRs are used as the sensors. The sensor board is replaceable and it can use other sensors (such as IR LED + IR phototransistor) with ease. Apocalypse is highly configurable; we configured it according to our needs and it served as a formidable base for many events.
		</p>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="../../assets/img/robots/apocalypse0.jpg" title="Apocalypse image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>





