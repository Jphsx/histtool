

This script reads a ttree and generates a class similar to make class, this class contains TH1D objects of all the root data. The script then generates another script to link and fill all the histograms in the histogram class which then creates a rootfile of histograms.
(note all filenames are currently hardcoded)
run with (in root interpreter) 


.x generateTreeClass.cpp++

this creates two files

OutputClass.cpp which contains all histograms, this is an intermediate file for rebinning and labeling histograms

also created is 

Loop.cpp which fills the histograms in the OutputClass, to fill them run

.x Loop.cpp++

the output is a .root file
