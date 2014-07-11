#Notes on "Tracking Principles"

Kota Miura (miura@embl.de, <http://cmci.embl.de>)

# Introduction



- Vogt, W., 1925. Gestaltungsanalyse am Amphibienkeim mit örtlicher Vitalfärbung. Vorwort über Wege und Ziele. Wilhelm Roux. Arch. Entwickl. Mech. Org. 106, 542–610.
  - A classic paper on presumptive fate map.

Modern version of tracking allows the analysis both in forward and backward, in a quantitative manner. 

- Keller, P.J., Schmidt, A.D., Wittbrodt, J., Stelzer, E.H.K., 2008. Reconstruction of zebrafish early embryonic development by scanned light sheet microscopy. Science 322, 1065–9.
  -  A modern tracking version of "presumptive fate map"

**Tracking = Dot Detection (Segmentation) + Linking ** 

# Manual Tracking

Click-and-Track. Manual tracking is always a quick solution. 

- ManualTracker plugin
  - Included in Fiji. 
  - <http://rsbweb.nih.gov/ij/plugins/track/track.html>

- MtrackJ
  - Included in Fiji. 
  - <http://www.imagescience.org/meijering/software/mtrackj/>
  
# Dot Detection/ Delineation Tools

Segmentation of target objects. 

## Active Contour

- QUIMP
  - Well-designed plugin for tracking cell contour dynamics. 
  - <http://www2.warwick.ac.uk/fac/sci/systemsbiology/staff/bretschneider/quimp/ > 

## 2D Gaussian Fitting

Following are the tools using 2D Gaussian fitting.

### SpecleTrackerJ plugin

A tracker for fluorescence speckle microscopy. 

- <https://code.google.com/p/speckletrackerj/>

### PTAJ plugin

A tracker for single molecule imaging. Uses minpak for the optimization. 

- <https://github.com/arayoshipta/projectPTAj>

### The GDSC Single Molecule Light Microscopy (SMLM) plugins

For super-resolution microscopy (PALM/STORM) images, another one beside QuickPalm. It fits single molecule dots, recovers sub-pixel resolution coordinates of dots to render an super resolution image. 

- <http://www.sussex.ac.uk/gdsc/intranet/microscopy/imagej/smlm_plugins>
- Available via Fiji update site.

Similar tools are listed in the following site:

<http://bigwww.epfl.ch/smlm/software/>

##Machine Learning based Segmentation

- Weka segmentation
  - Included in Fiji.  

##Cross-Correlation, or Template Matching

### PIV 

More like a vector field analysis, based on cross-correlation analysis throughout the image field.  

<https://sites.google.com/site/qingzongtseng/piv>

![image](TFM NP_48_32 16.png)

#Linking

A short history of global optimization strategy for linking. 

- Vallotton, P., Ponti, a, Waterman-Storer, C.M., Salmon, E.D., Danuser, G., 2003. Recovery, visualization, and analysis of actin and tubulin polymer flow in live cells: a fluorescent speckle microscopy study. Biophys. J. 85, 1289–306.

- Sbalzarini, I.F., Koumoutsakos, P., 2005. Feature point tracking and trajectory analysis for video imaging in cell biology. J. Struct. Biol. 151, 182–95.

- Sbalzarini, I.F., 2006. A MATLAB toolbox for virus particle tracking ICoS Technical Report Notice of Copyright. Technology 1–16.

- Bise, R., Yin, Z., Kanade, T., 2011. Reliable cell tracking by global data association, in: 2011 IEEE International Symposium on Biomedical Imaging: From Nano to Macro. IEEE, pp. 1004–1010.
  - "tracklets"

- ParticleTracker
  - <http://mosaic.mpi-cbg.de/?q=downloads/imageJ>
















