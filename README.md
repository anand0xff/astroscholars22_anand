# astroscholars22_anand
Optics, Lenses, and Telescopes 2022 JHU.  
Advisor: Dr. Anand Sivaramakrishnan   (Dr. Anand works too!)

Material to support Anand's "Telescopes and Optic" lab.  Assumes astroconda is the python environment being used.  

**Navigate to**. the github AS22 for the section: [repo](https://github.com/anand0xff/astroscholars22_anand)   
**Download** a zip on Windows or clone from this location on UNIX), and expand it.   

you might have all the modules already loaded, with the lossible exception of imageio... I created this envirinment from the "base" anaconda environment.  

**If needed**, install the all these, otherwise try to run the script in the next section
 
		If you don't have the 'as22' conda env on your machine:
		'(base) bash$'   is your prompt  
		conda create -n py39 python=3.9
		conda deactivate
		conda activate py39. # makes '(py39) bash$' your prompt
		conda install astropy
		conda install scipy
		conda install matplotlib
		
		Otherwise only use this if you have activated 'as22' conda env:
		conda install imageio
		


Now run the python script to create R, G, B fits files out of a sample jpg file...  this enables us to look at just the numerical values in a viewer like DS9.

		python jpg_rgbfits.py  # gives you syntax used like this
		python jpg_rgbfits.py ../jpg_rgb/Gigi_in_Central_Park.jpg
		# change file name including path name to convert another file.
		
	 
		
		
#### Monday's class (added reminders)

- Light: wave description - wavefronts (constant phase -> wave speed)
- Interference of wave amplitudes (principle of superposition)
- Light interference almost always 'single photon' interference: think monochromatically, add intensities for polychromatic images.
- What is a radian
- What determines [resolution](https://image1.slideserve.com/1553225/resolving-power-airy-disk-l.jpg)?
- From [raytracing](https://image1.slideserve.com/3006816/thin-lenses-ray-tracing1-l.jpg) to image formation
- [Thin lens equation](https://en.wikipedia.org/wiki/Thin_lens) in "Image Formation" related object distance, image distance, and lens focal length 
- Larger pinholes produce larger [circle of confusion](https://en.wikipedia.org/wiki/Circle_of_confusion) blur - ray optics
- Smaller pinholes crate larger diffraction blur: the Point-Spread function is an [Airy pattern](https://en.wikipedia.org/wiki/Airy_disk) - wave optics

#### Tuesday's class - today

Think of your class project - Tue Wed Thu remain

* Topic(s)
* Explorations (Tue Wed Thu) 
* Sections/assignments (Tue Wed)
* Results amd slide creationTue Wed Thu
* Edting & refining
* Presenting

Experiments.  

* Pinhole setup: Olympus E-PL5 (2012)
* Olympus E-PL5, sensor 17.3mm x 13 mm, 4627 x 3479 eff. pixels
* Pinholes 100, 200, 300, 400, 600 (?) um
* Laser stable setup to illuminate pinholes, take data
* Crop of full res images made with 5 pinholes (native pixel size)
* Fits files of RGB "slices" of above
* JPGs of full frame, but smaller resolution (rebinned)
* R & B laser illumination of pinholes
* Crop of full res images made with 5 pinholes (native pixel size)
* Fits files of RGB "slices" of above
* JPGs of full frame, but smaller resolution (rebinned)
  
Fraunhofer diffraction.  

* Fresnel to Fraunhofer (i.e. far field) transition: [Fresnel length](https://en.wikipedia.org/wiki/Fresnel_diffraction#/media/File:Comparison_Sommerfled-Fresnel-Fraunhofer.gif)
* Lens in focus: same as far field (in angular image space)
* [Airy pattern animation](https://en.wikipedia.org/wiki/Fraunhofer_diffraction).  
* [Airy pattern derivation & equation](https://en.wikipedia.org/wiki/Fraunhofer_diffraction_equation#Circular_aperture)
* PSFs and the [convolution integral](https://phiresky.github.io/convolution-demo/)
* Planetary orbits:  Earth 1 AU, Jupiter 12 AU. *(1 AU = 1.5e11 m)*. 
* Telescope diameter 10 m, wavelength 1.0e-6 m = 1 micron   
* Resolution = lambda/D = 1e-7 rad = 0.02 arcsec *(2e5 arcsec = 1 rad)*.  
* At what stellar distance can we resolve an Earth and a Jupiter from its host star?  (Use small angle approximationn - no need for sines & cosines)


#### Wednesday's class




#### Thursday's class




#### Friday's class

	