# poly-GA
Python scritps for rendering and distance analysis of proteins (proteasome) and segmentations (poly-GA aggregates) in Cryo-ET

These scritps have been developed for being run in Linux 64bit platform with python 2.7.13. It also requires to have installed the next packages:
  - Additional software packages:
    + pyto (Lučić et al., 2016, PMID: 27742578 DOI: 10.1016/j.jsb.2016.10.004)
    + pyseg (https://github.com/anmartinezs/pyseg-poly-GA.git)
    
render_sub_tomo.py

    Renders template copies in a tomogram from a STAR file (poly-GA adaptation)

    Input:  - STAR file
            - Reference tomogram
            - Template pre-processing parameters
            - Rigid transformations parameters

    Output: - A set of VTK poly data for rendering the templates on the reference tomogram
    
star_seg_dst.py

    Measures distance from STAR files particles to segmentations

    Input:  - STAR files
            - Segmentation
            - Distance parameters
            - Particle template preprocessing settings

    Output: - STAR files with the distances measured
