# astroscholars24_anand
Optics, Lenses, and Telescopes 2022 JHU.  
Advisor: Dr. Anand Sivaramakrishnan   (Dr. Anand works too!)

Material to support Anand's "Telescopes and Optic" lab.  Assumes anaconda is the python environment being used.  

Day by day I'll update the next class.  This file's future classes are develoiped for the 2022 class.  You might steer us differently...


	
#### Monday's class (added reminders)

- Light: wave description - wavefronts (constant phase -> wave speed)
- Interference of wave amplitudes (principle of superposition)
- Light interference almost always 'single photon' interference: think monochromatically, add intensities for polychromatic images.
- What is a radian
- What determines [resolution](https://image1.slideserve.com/1553225/resolving-power-airy-disk-l.jpg)?
- From [raytracing](https://image1.slideserve.com/3006816/thin-lenses-ray-tracing1-l.jpg) to image formation
- 100um to 1/16th inch pinhole imaging sequence (day 1 data, jpg_rgb/Day1_pinholes
- [Thin lens equation](https://en.wikipedia.org/wiki/Thin_lens) in "Image Formation" related object distance, image distance, and lens focal length 
- Larger pinholes produce larger [circle of confusion](https://en.wikipedia.org/wiki/Circle_of_confusion) blur - ray optics
- Smaller pinholes crate larger diffraction blur: the Point-Spread function is an [Airy pattern](https://en.wikipedia.org/wiki/Airy_disk) - wave optics

#### Not Tuesday's class- actually Wednesday's class!

Class project - Tue Wed Thu remain

* Define first 
* Explorations (Wed Thu) 
* Sections/assignments (Tue Wed)
* Results and slide creation Wed Thu, refine Fri
* Presenting Fri



Existing data in this repo:  

* Pinholes 100, 200, 300, 400 um, 1/16th inch
* Crop of full res images made with 5 pinholes (native pixel size)
* Fits files of RGB "slices" of above
* R & B laser illumination of pinholes
  
  
Class topics  

* From pupil to focus - and beyond movie (Emiel Por) [here](https://docs.hcipy.org/0.5.1/tutorials/NearFarFieldDiffraction/NearFarFieldDiffraction.html#)
* Lensmaker's equation from [wikipedia](https://en.wikipedia.org/wiki/Focal_length)
* [Refraction](https://en.wikipedia.org/wiki/Refraction) of light at a boundary (nice animation)
* In-focus image properties: [pixel or plate scale](https://github.com/anand0xff/astroscholars22_anand/blob/main/PLSCL.pdf), beam focal ratio (f-number) [angular resolution](https://en.wikipedia.org/wiki/Angular_resolution) "lambda/D"
* (optional) Far-field or in-focus Point Source Function using Fourier transforms, and the [Airy pattern derivation & equation](https://en.wikipedia.org/wiki/Fraunhofer_diffraction_equation#Circular_aperture)  
* PSFs and the [convolution integral](https://phiresky.github.io/convolution-demo/) - use Square (object), Gaussian (PSF) to see telescope image  

Miscellaneous

* Earth 1 AU, Jupiter 12 AU. *(1 AU = 1.5e11 m)*. Earth diameter = ? 
* JWST diameter 10 m, Hubble diameter 2.4 m, wavelength 1.0e-6 m = 1 micron.  Angular resolution? Detector pixels?   
* Resolution = lambda/D *(2e5 arcsec = 1 rad)*.  



#### Thursday's class
Results and slide creation

######Feedback to Anand:  Tentative responses from Anand - we'll work through & refine today:

*They would like an example of how to introduce the project*

The talk **could**  go like this:

- Start with title  
- Then state the "Science Requirement" driving the investigation, and the quantities (distance of telescope from Earth) that satisfy the Science Requirement.  Conceptual, very very short.
- Segue into a brief list of key topics you had to figure out to get your answer: eg Camera creates image, what determines image sharpness, size of image on detector, pixel size of detector (physical, and angular on-sky size), ...
- Slide-by-slide explain the key arguments, with formulae & numbers for the two cases, derivations, etc. ... 
- The "answer" to the driving question



*Explain arcseconds*. 

360 degrees in a circle (2 pi radians), 60 arcminutes (aka minutes of arc) in a degree, 60 arcseconds in an arcminute (aka minute of arc).  Moon is about 1/2 degree angular size to us on Earth, so 30 arcmin angular (apparent) diameter for us, which is 1800 arcsec.  [Planet sizes](https://www.timeanddate.com/astronomy/planets/distance) (select "Size in Sky").

*Is it acceptable for them to perform and show their calculations using google sheets?*

You should write the formulae out and give results numerically to each step as you explain your work.  That presents it in a sequence for the audience to absorb, one step at a time.  If you want you can add a link in your references to the google sheet for the detailed calculations all together.

*Lastly, what should the students use for simulations in the presentations?*

Let's see if we get there.  

#### Thursday's class
Results and slide creation

Our session today is two hours, 2:50p - 4:50p.

Content definition and slide creation/definition, with rough first draft by the session end. 

--
--

2022 material for future reference if you are interested:

##### What have we done?

[Slide 13](http://nicadd.niu.edu/~piot/phys_630/Lesson7.pdf)  Ojo: Slide 13  might be interesting to you
 
		
---
		
	




#### Friday's class

* Presentation!

	