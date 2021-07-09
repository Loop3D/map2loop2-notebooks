**Example notebooks and test python scripts to accompany the GMD paper:**   
Automated geological map deconstruction for 3D model construction using map2loop 1.0 and map2model 1.0
Mark Jessell, Vitaliy Ogarko, Yohan de Rose, Mark Lindsay, Ranee Joshi, Agnieszka Piechocka, Lachlan Grose, Miguel de la Varga, Laurent Ailleres, Guillaume Pirot   
https://doi.org/10.5194/gmd-2020-400   
   
Notebooks:  
1) Example 1 - Using Loop's Sources.ipynb   
- This notebook reproduces the model described in the above paper using prededfined valeus and drawing source data from online servers.   
2) Example 2 - Draw Your Own Area.ipynb    
- This notebook allows the user to select arbitrary reactangles around Western Australia and extract the information needed to build 3D models (if sufficient data is locally available)   
3) Example 3 - Local Source Data.ipynb    
- This notebook alls the user to extract informationa nd build 3D mdoels from their own source data. If the Example 1 notebook has been run, all the necessary shapefiles to build a model will be available in the gmd-model/tmp directory   
4) Utility 1 - Config file generator.ipynb    
- This notebook interactively creates the hjson and python scripts needed to run models from your own data sources   
    
Python scripts    
1) GMD-testscript.py    
- This is the non-notebook equivalent of Example 1
2) exporters.py   
- Code snippets for converting LoopStructural surfaces and voxels into various standard formats. geohy and omf require additional libraries to be installed (https://github.com/gmggroup/omf) and (https://github.com/MiraGeoscience/geoh5py)
- Triangulated surfaces supported: vtk, obj, omf, dxf, geoh5, ts
- Voxel formats supported: omf, geoh5

