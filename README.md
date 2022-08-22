# astroscholars22_anand
Optics, Lenses, and Telescopes 2022 JHU.  
Advisor: Dr. Anand Sivaramakrishnan   (Dr. Anand works too!)

Material to support Anand's "Telescopes and Optic" lab.  Assumes astroconda is the python environment being used.  

**Navigate to**. the github AS22 for the section: [repo](https://github.com/anand0xff/astroscholars22_anand)   
**Download** a zip on Windows or clone from this location on UNIX), and expand it.   

you might have all the modules already loaded, with the lossible exception of imageio... I created this envirinment from the "base" anaconda environment.  

**If needed**, install the all these, otherwise try to run the script in the next section
 
		(base) bash$ conda create -n py39 python=3.9
		(base) bash$ conda deactivate
		(base) bash$ conda activate py39
		(py39) bash$ conda install astropy
		(py39) bash$ conda install scipy
		(py39) bash$ conda install matplotlib
		(py39) bash$ conda install imageio

Now run the python script to create R, G, B fits files out of a sample jpg file...  this enables us to look at just the numerical values in a viewer like DS9.

		(py39) bash$ python jpg_rgbfits.py 
		(py39) bash$python jpg_rgbfits.py ../jpg_rgb/Gigi_in_Central_Park.jpg		
		
	

- Examine RGB channels of jpg images, write separate FITS files for each channel. 

- On a **Unix** or **Windows** terminal command line, deconstruct a jpg image into R, G, B:

		(astroconda) bash$ cd astroscholars22_anand/code/ImageExamples
		(astroconda) bash$ python jpg_rgbfits.py anyfile.jpg

	Pinhole camera predictions

		(astroconda) bash$ cd astroscholars_anand/code
		(astroconda) bash$ python photo_pinhole.py
		