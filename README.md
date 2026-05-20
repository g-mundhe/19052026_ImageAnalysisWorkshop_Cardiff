# 19052026_ImageAnalysisWorkshop_Cardiff
## subtitle
### Repository created during IA workshop in Cardiff


#### Write an environment.yml file for python=3.10 for this: conda activate introIA-env to activate introIA-env environment conda install pip to install pip pip install jupyterlab to install Jupyter-lab pip install scikit-image to install scikit-image pip install matplotlib to install matplotlib pip install pandas to install pandas pip install numpy to install numpy pip install imagecodecs to install imagecodecs pip install openpyxl to install openpyxl conda install -c conda-forge pyqt napari==0.6.6 to install napari pip install napari-skimage to install the napari-skimage plugin

name: introIA-env
channels:
  - conda-forge
  - defaults

dependencies:
  - python=3.10
  - pip
  - pyqt
  - napari=0.6.6
  - pip:
      - jupyterlab
      - scikit-image
      - matplotlib
      - pandas
      - numpy
      - imagecodecs
      - openpyxl
      - napari-skimage
        
conda env create -f environment.yml
conda activate introIA-env


##### If you want maximum compatibility, you could also install numpy, pandas, matplotlib, and scikit-image through Conda instead of pip:
name: introIA-env
channels:
  - conda-forge
  - defaults

dependencies:
  - python=3.10
  - pip
  - numpy
  - pandas
  - matplotlib
  - scikit-image
  - imagecodecs
  - openpyxl
  - pyqt
  - napari=0.6.6
  - pip:
      - jupyterlab
      - napari-skimage
