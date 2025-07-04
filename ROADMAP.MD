# Python package that has one purpose: Combining any intravascular image modality with CCTA meshes.
# Base module (aligning frames withing IVUS/OCT)
- [] Bind all Rust structs to python objects
- [] Single mesh alignment (ignoring systole and diastole (for OCT))
- [] Functions should return obj, as python objects

# Centerline alignment module
- [] Centerline resampling based on geometry
- [] 3-Point alignment versus Hausdorff-alignment versus manual (degree/centerline point)
(- [] Create Centerline directly from mesh)

# Mesh combination
- [] Read in CCTA mesh (STL/Obj)
- [] Assign regions based on Centerlines (RCA, LCA, Aorta)
- [] Shrink/Expand CCTA to best match Aortic wall and shrink/expand coronary to match iv images
- [] ensure works for IVUS and OCT