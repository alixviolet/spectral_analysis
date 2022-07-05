# spectral_analysis
	If using linux/macOS, install iSpec directly from the guides at https://www.blancocuaresma.com/s/iSpec/manual/installation/linux or https://www.blancocuaresma.com/s/iSpec/manual/installation/osx/anacondapython
	If using windows, then you will need to set up a virtual machine to perform analysis. I did this using https://www.virtualbox.org/ and following the guide on https://linuxconfig.org/how-to-install-ubuntu-20-04-on-virtualbox. If the window refuses to go into fullscreen mode, follow the guide on https://www.itzgeek.com/post/how-to-install-virtualbox-guest-additions-on-ubuntu-20-04/.
	To install iSpec in the virtual machine, follow the guide at https://www.blancocuaresma.com/s/iSpec/manual/installation/linux/anacondapython. Make sure all of the packages from the list at https://www.blancocuaresma.com/s/iSpec/manual/installation/linux/apt are installed. 
	(Hopefully) All functions necessary for spectral analysis are contained within the big_mega_code file, with descriptions on how to use/modify them :)
	It is important to check the format of your spectra - the code has been optimised for use with SOPHIE spectra. Depending on the instrument, you may be working with spectra of a different resolution so make sure to check this (for both HE and HR spectra if relevant). Also, some spectra may already be coadded, normalised or rv/telluric/barycentric velocity corrected - if so, the functions in the code for each step are labelled so that you can remove them.
	Only rv correction is included in the code as the others are done in the SOPHIE data reduction, however the example.py file within the iSpec directory has functions that perform the barycentric and telluric corrections if these are necessary. 
