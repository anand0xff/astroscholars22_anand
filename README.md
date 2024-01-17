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

#### Tuesday's class

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

--
--
#### Wednesday's class

* Topic(s)
* Explorations (Start today) 
* Results and slide creation Wed Thu

 Discussion of topics/sub-topics (10 min at start, again mid-session)   
 *	Already brought up: astronomical science interest/target.  
 * Choice of telescope and wavelength
 * suggestion: two possible images: present simulated telescope images to determine telescope diameter (convolution)

 Use R & B laser illumination of pinholes and new fits files. to
 determine diffraction dependence on wavelength, with R, B light sources
 and 100, 300, 400 um pinhole data.

## Thursday's class

Our session today is two hours, 2:50p - 4:50p.

Content definition and slide creation/definition, with rough first draft by the session end. 

I'm also available tomorrow am if you want. 

##### What have we done?

As a starter we looked at describing a **wavefront** mathematically, and its **phase**.  And also at what interference of waves is, including lack of interaction between different photons.  If you want a slide showing this, we could take a jpg image with the red & blue laser pinhole images landing on almost the same spot in the camera.  

The main work we did was to truly understand the resolution of an optical system.  And why lenses or mirrors improved early pinhole imaging in a bedroom (camera in Italian).  You called out a sweet spot of pinhole sharpness - that's a cool result!  That transition involved the Fresnel length, given the pinhole or aperture size, distance from pinhole, and the light's wavelength.  Lenses near focus are equivalent to **far field** diffraction.  [Slide 13](http://nicadd.niu.edu/~piot/phys_630/Lesson7.pdf) shows the near-aperture to In Focus progression of the light pattern (\N_\f in this slide is the Fresnel length / how far the screen is from the aperture - 0.1 is 10 Fresnel lengths away).  
####Ojo: the above Slide 13  might be interesting to you
 
How does a lens work to create a focus?  We did not cover that in detail.  It tilts incident parallel bundles of light rays from a distant point source so they come together at one point, and delays each ray's phase so they have the same phase when they reach this focal point.  The delay is carefully matched to the "prism angle" of that slice of the lens, which imparts the tilt. Light travels slower through glass than air, so the thick middle of a convex lens delays light more than the thinner edge of the lens. Constructive interference happens for all the light paths reaching the focal point, so brightness is high** there.  That spot is an in-focus PSF of the lens, created by the point source.

We also worked on quantifying resolution by looking at the response of our optics to illumination by a point source.

Every point in the scene in front of a camera or telescope produces its own point spread function response at the appropriate location on your detector.  These individual PSF **intensities** all add to crate the "picture" you get when you press the shutter button.

##### My thoughts on what we've discussed: 

* In the Day3 files the Point Spread Function (that Robel mentioned in his presentation yesterday!) - the image of a pint source through the optical system - is not as deeply exposed as in Day2's data, which burned out the core but showed the extended ringy structure far from the "(laser) star" we were "observing" with the simple system.
* You calculated the angular size of the resolution - this angle is pretty much the smallest scale we can distinguish in an image we obtain with the optical system under consideration.  The core of the PSF (of a circular telescope) has a radius **1.22 lambda/D** (the Airy Disk radius). 
* Think of an astronomical science case you might want to optimize your telescope for.  At what distance (**D\_target**) from us is your object, and what is the minimum physical feature length (L\_feature) you want to see? The feature could be a planet's distance from its host star, the size of a protoplanetary gas-and-dust disk, the length of a jet from an Active Galactic Nucleus (AGN) galaxy, ...
* With that in mind, what angle (A) would that feature subtend to us observers at or near our home planet, the Earth?  If you've  put your target even at the nearest star, it's distance from the Sun is a good enough approximation!  (**A = L\_feature/D_target** radians).
* So you need a telescope whose angular resolution lambda/D_telescope is at least as small as A.  Maybe half the size of A, just to be sure.
* What wavelength do you want to observe this target in?  That sets lambda.
* All these considerations fix the telescope primary mirror diameter.  Work out the number (in meters)

Once you know how large a telescope you want, for extra fun you could estimate a cost estimate for a ground-based telescope, either a 'giant segmented mirror' (GSM) or a single dish 'monolithic' primary mirror design.  The graph [here](http://www2.lowell.edu/users/gerard/publications/van_belle_meinel2_2004.pdf) on page 7.  An informed guess is fine after a quick glance at the graph!




---
### Startup
**Navigate to** the github AS22 for the section: [repo](https://github.com/anand0xff/astroscholars22_anand)   
**Download** a zip on Windows or clone from this location on UNIX), and expand it.   

You might have all the modules already loaded as part of your as22 set-up, with the possible exception of imageio.

I created this environment from scratch, the "base" anaconda environment...

**If you don't have "as22" conda env ready**, install all these modules:
 
		'(base) bash$' is your prompt  
		conda create -n py39 python=3.9
		conda deactivate
		conda activate py39. # makes '(py39) bash$' your prompt
		conda install astropy
		conda install scipy
		conda install matplotlib
		
		
**If you have an activated 'as22' conda env**, only do this :

		'(as22) bash$' is your prompt
		conda install imageio
		


Now run the python script to create R, G, B fits files out of a sample jpg file...  this enables us to look at just the numerical values in a viewer like DS9.

		python jpg_rgbfits.py  # called like this it'll remind you of usage
		python jpg_rgbfits.py ../jpg_rgb/Gigi_in_Central_Park.jpg
		# change file name including path name to convert another jpg file into fits files.
		
---
		
	




#### Friday's class

* Presentation!

	