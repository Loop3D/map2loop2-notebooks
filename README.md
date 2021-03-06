**Example notebooks and test python scripts to accompany the GMD paper:**   
Automated geological map deconstruction for 3D model construction using map2loop 1.0 and map2model 1.0
Mark Jessell, Vitaliy Ogarko, Yohan de Rose, Mark Lindsay, Ranee Joshi, Agnieszka Piechocka, Lachlan Grose, Miguel de la Varga, Laurent Ailleres, Guillaume Pirot   
https://doi.org/10.5194/gmd-2020-400   
   
**Notebooks:**  
1) Example 1 - Using Loop's Sources.ipynb   
- This notebook reproduces the model described in the above paper using prededfined valeus and drawing source data from online servers.   
2) Example 2 - Draw Your Own Area.ipynb    
- This notebook allows the user to select arbitrary rectangles around Western Australia and extract the information needed to build 3D models (if sufficient data is locally available). Apart from an inline 3D model, a webgl version of the model will be saved as a timestamped file vtkleaflet*.html and a timestamped directory vtkleaflet* will be created that contains vtk and obj format versions of the trangulated surfaces, and  a voxel model will be stored in gmd-model/tmp/voxels.raw. Other formats can be saved using the codes in exporters.py   
3) Example 3 - Local Source Data.ipynb    
- This notebook allows the user to extract information and build 3D models from their own source data. This uses example data and config file found in the source_data directory. Use the **Utility 1** notebook to generate a hjson configuration file and example python script for your own data. 
4) Utility 1 - Config file generator.ipynb    
- This notebook interactively creates the hjson and python scripts needed to run models from your own data sources   
5) Utility 2 - Exporters.ipynb    
- Code snippets for converting LoopStructural surfaces and voxels into various standard formats. geoh5 and omf require additional libraries to be installed (https://github.com/gmggroup/omf) and (https://github.com/MiraGeoscience/geoh5py)
    - Triangulated surfaces supported: vtk, obj, omf, dxf, geoh5, ts, webgl 
    - Voxel formats supported: omf, geoh5
   
    
**Python scripts**    
1) GMD-testscript.py    
- This is the non-notebook equivalent of the **Example 1 notebook**.   

