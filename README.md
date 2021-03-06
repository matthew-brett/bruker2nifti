## Bruker2nifti

Medical image format converter: from raw Brukert ParaVision to nifti, written in Python.

### Requirements
* Python 2.7+ provided with the libraries in requirements.txt (generated with pipreqs).

### Installation
To install it as a Python library
```
pip install bruker2nifti
```

### To install in development mode:
```
cd path-to-bruker2nifti-repo
pip install -e .
```

### CLI using via pip
Create a [virtualenvironment](http://python-guide-pt-br.readthedocs.io/en/latest/dev/virtualenvs/), activate it, then type
```
pip install bruker2nifti
bruker2nifti -h
```
to open the help of the command line utility.

### CLI using it anyway without pip:
* `PYTHONPATH="${PYTHONPATH}:path-to-bruker2nifti-repository"`
* `python parsers/bruker2nii.py -h`
* `python parsers/bruker2nii.py -i path/to/a/bruker/study -o path/to/output/folder`
Where python is a distribution proivided with the required libraries.

### Open the GUI via pip
Create a [virtualenvironment](http://python-guide-pt-br.readthedocs.io/en/latest/dev/virtualenvs/), activate it, then type
```
pip install bruker2nifti
bruker2nifti_gui
```

### Open the GUI and convert data without any programming
Download the repository as a .zip with button **clone or download** in the [repository home page](https://github.com/SebastianoF/bruker2nifti).
Unzip the donwloaded file and double click on the file `run_setupper_MAC` in the `GUI` folder.

After the automatic installation of a virtualenvironment with the required libraries, if everything worked, you should see a new file called 'OpenGUIbru2nii' in the code structure. 

This is a launcher. Double click on it: the following window should appear:  

![gui_example](https://github.com/SebastianoF/bruker2nifti/blob/master/screenshots/gui_example.jpg)

Keep the terminal open while doing the conversion, as there you will see the steps and the output of the different
conversion steps.
The launcher can be moved around in the user system. If you need to move the folder where you donwloaded the code.

If something went wrong please raise an issue in the [issue page of the repository](https://github.com/SebastianoF/bruker2nifti/issues).

### Testing
Unit testing with [nosetest](http://pythontesting.net/framework/nose/nose-introduction/):
* `nosetests`
Tests are based on an open dataset Bruker images downloadable with the repo, in the folder 
[test_data](https://github.com/SebastianoF/bruker2nifti/tree/master/test_data)

### API documentation, further notes and examples <a name="up"></a>
Essential API documentation can be found [here](bruker2nifti.rtfd.io).
Additional documentation and examples can be found in the [bruker2nifti wiki pages](https://github.com/SebastianoF/bruker2nifti/wiki).

### Useful links and related software <a name="utilities"></a>
+ [nifti format](https://nifti.nimh.nih.gov/nifti-1): official documentation.
+ [nifti format](https://brainder.org/2012/09/23/the-nifti-file-format/): unofficial documentation.
+ [nibabel](http://nipy.org/nibabel/): neuroimaging python library. 
+ [bruker format info](http://imaging.mrc-cbu.cam.ac.uk/imaging/FormatBruker): one of the few places where to find 
information about Bruker format, other than the official documentation stored under 
<PvInstDir>/prog/docu/english/pvman/D/Docs/D02_PvParams.pdf of the ParaVision installation. 
+ [pvconv](https://github.com/matthew-brett/pvconv): from Bruker to Analyze, Perl.
+ [Bru2Nii](https://github.com/neurolabusc/Bru2Nii): from Bruker to Nifti, written in Pascal. 
+ [mpi](https://github.com/francopestilli/mpi): from Bruker to Vistasoft or Analyze in Matlab. Conversion is based on the parameters contained in the **reco** parameter file. This
parameter file exists only if the image was created using ParaVision reconstruction.
+ [Bruker2nifti](https://github.com/CristinaChavarrias/Bruker2nifti): from Bruker to Nifti, Matlab (not maintained anymore?).


### Copyright and Licence 
Copyright (c) 2017, Sebastiano Ferraris.
Bruker2nifti is available as free open-source software under [MIT License](https://github.com/SebastianoF/bruker2nifti/blob/master/LICENCE.txt).

### Thanks <a name="thanks"></a>
Thanks to 
Bernard Siow (Centre for Advanced Biomedical Imaging, University College London), 
Chris Rorden (McCausland Center for Brain Imaging, University of South Carolina) 
and 
Mattew Brett (Berkeley Brain Imaging Center).
