---
layout: post
title: Experimenting With Visualization
category: posts
---

![UCSD Undergraduate Department Sizes Spring 2012][ucsd_dept_bubblesspr12]

I've been spending some time here and there playing with [Processing][processing], a graphic generating programming language.  This is a visualization I made showing the sizes of the the different academic departments at the University of California, San Diego using <a href="http://blink.ucsd.edu/instructors/courses/enrollment/week3.html">information from the Registrar's Office</a>. Even though this is a pretty pedestrian visualization, it's pretty cool to give those enrollment numbers geometric meaning. That's a lot of biology majors...

##How It's Done

The program bundles together the department code with the number of undergraduates enrolled in it, then generates a circle with a random color with size proportional to the number of students.  The scale factor that controls the circle size is  constant within each rendering, but varies between renderings. Students in double (and triple) majors are counted in each department he/she is enrolled in.

##The 6 College Breakdown

The breakdown for the <a href="http://admissions.ucsd.edu/colleges/about/index.html">6 undergraduate colleges</a> that form UCSD:

####Revelle College
![Revelle][revelle]

####Muir College
![Muir][muir]

####Marshall College
![Marshall][marshall]

####Warren College
![Warren][warren]

####Eleanor Roosevelt College
![ERC][erc]

####Sixth College
![6th][6th]

###Department Codes

- ANTH.....Anthropology

- BENG.....Bioengineering

- BIOL ......Biology

- CENG......Chemical Engineering

- CGS.........Critical Gender Studies

- CHEM.....Chemistry

- CHIN.......Chinese Studies

- COGS.......Cognitive Science

- COMM.....Communications

- CSE..........Computer Science and Engineering

- ECE..........Electrical and Computer Engineering

- ECON.......Economics

- ESYS.........Environmental Systems

- ETHN.......Ethnic Studies

- GMST........German Studies

- HDP..........Human Development

- HIST.........History

- INTD.........Interdisciplinary?

- INTL.........International Studies

- ITAL.........Italian Studies

- JAPN........Japanese Studies

- JUDA.......Judaic Studies

- LATI.........Latino Studies

- LING.........Linguistics

- LIT............Literature

- MAE..........Mechanical and Aersospace Engineering

- MATH.......Mathematics

- MUS..........Music

- NENG........Nanoengineering

- PHIL.........Philosophy

- PHYS.........Physics

- POLI..........Political Science

- PSYC..........Psychology

- RELI..........Religion

- RUSS.........Russian Studies

- SE.............Structural Engineering

- SIO............Scripps Institute of Oceanography (think Earth Science)

- SOC...........Sociology

- THEA........Theater and Dance

- TWS..........Third-world Studies

- UNAF........Undeclared

- USP...........Urban Studies and Planning

- VIS............Visual Arts



[ucsd_dept_bubblesspr12]: /images/ucsd-vis/UCSD_Dept_BubblesSPR12.gif
[marshall]: /images/ucsd-vis/Marshall_Dept_BubblesSPR12.gif
[muir]: /images/ucsd-vis/Muir_Dept_BubblesSPR12.gif
[revelle]: /images/ucsd-vis/Revelle_Dept_BubblesSPR12.gif
[6th]: /images/ucsd-vis/Sixth_Dept_BubblesSPR12.gif
[erc]: /images/ucsd-vis/ERC_Dept_BubblesSPR12.gif
[warren]: /images/ucsd-vis/Warren_Dept_BubblesSPR12.gif

[processing]: http://processing.org
