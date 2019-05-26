---
title: "Steven M Day's Retirement Symposium"
layout: gridlay
excerpt: "Steven M Day's Retirement Symposium"
permalink: /symposium/
---

# Steven M. Day Retirement Symposium 
#### <span style="color:red">*Sep 13th, 2019 @ San Diego State University*</span>
--------------------
<br/>
![]({{ site.url }}{{ site.baseurl }}/images/symposium/steveday.jpg){: style="width: 500px; float: left; border: 100px"}

Prof. Steven M. Day is a world-renowned computational seismologist and great teacher whose research and expertise has shaped the fields of dynamic rupture and physics-based ground motion simulation. He received B.S. of Geology from University of Southern California in 1971. Then he moved to San Diego and obtained Ph.D. of Geophysics from Institute of Geophysics and Planetary Physics, University of California, San Diego in 1977. After graduation, he worked as a Research Geophysicist (1977-1983) and Program Manager for Theoretical Geophysics (1983-1987) in S-Cubed, Inc and Maxwell Laboratories, Inc, respectively. Since 1988, he had been serving as Rollin and Caroline Eckis Professor of Seismology in Department of Geological Sciences of San Diego State University. During his academic years, he was Member of Board of Directors, Southern California Earthquake Center (2002-2015), Member in Committee on Seismology of the National Research Council (1990-1996), Member of Earthquake Ground Motion Review Panel of Nuclear Regulatory Commission (1985-1991) ,etc. He honorably became an Emeritus Professor in 2016. 
[Steve's gallery]({{ site.url }}{{ site.baseurl }}/stevegallery)

## <span style="color:red">*Congratulations to Steve!*</span>
--------------------
<br/>

### Topics and aspects

##### <span style="color:blue">*Earthquake Rupture Dynamics, Strong Ground Motion and Nuclear Explosion Seismology*</span>

### Organizing committee
- Dr. Yongfei Wang (SCEC)
- Dr. Kim Olsen (SDSU)
- Dr. Allen Gontz (SDSU)
- Dr. Thomas Rockwell (SDSU)

### Location
#### Scripps Cottage, San Diego State University

![]({{ site.url }}{{ site.baseurl }}/images/symposium/sc.jpg){: style="height: 220px; float: left; border: 100px"}
![]({{ site.url }}{{ site.baseurl }}/images/symposium/sdsu.jpg){: style="height: 220px; float: left; border: 100px"}

<br/>
[Interative Map](http://www.myatlascms.com/map/index.php?id=801#!ce/12160,17006?ct/17006?m/152641)


## Participant list 
##### (Alphabetical ranking):
--------------------
{% assign number_printed = 0 %}
{% for member in site.data.participants %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}


<div class="col-sm-3 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/symposium/{{ member.photo }}" class="img-responsive" width="200px" style="float: center" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 3 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 3 %}
</div>
{% endif %}
