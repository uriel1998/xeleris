xeleris
=======

A series of scripts to work with the Xeleris Molecular Imaging System and other files for a nuclear medicine clinic.

This work is licensed under the Creative Commons Attribution-ShareAlike 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/3.0/.

##DISCLAIMER  
These scripts are used in a real hospital on real patients. However, I am "just" a technologist, and have never been officially" trained in Aladdin.  That said, I have made every attempt to ensure that they are correct in all ways.  I make no guarantee or warantee, express or implied.  I am not responsible for any outcome on your system. You must have a basic understanding of the Aladdin script language (or virtual basic) to make these work correctly! 

##WHAT YOU GET  
Uncompiled Aladdin scripts (and review templates and SOPs, when applicable) so that you can modify these scripts to work properly on your own Aladdin system, contained in a ZIP archive. Click on the thumbnails for larger images. These scripts are written specifically for my site; your acquisition protocols almost certainly differ and will require that you modify these scripts. There are also selected SOP (standard operating procedures or protocols) for various studies. While site-specific, they are written with processing using the Xeleris (and these scripts) in mind. 

##LEGALITY  
Read the disclaimer again! I am not responsible for your systems or patients! These are all released under a Creative Commons Attribution-ShareAlike license. I ask that you email me any modifications and improvements so that I can place them here. We are allowed to share these scripts;  I checked (see legality.gif for a screenshot). 

#Patient Rename  
This script allows you to conveniently rename most aspects of any study in the Xeleris database.  It automagically forces you to add an accession number, and then using "Mass Rename" will walk you through renaming up to sixteen images... while you're able to see what you're renaming!  It also has defaults for renal renaming and gastric emptying (two of the pickier default Xeleris scripts).  You can also, on the second page, rename the study, patient name, and more with ease. 

#Whole Body Scan    
This script displays anterior and posterior whole body images, along with up to eight spot films, on one screen.  The whole body displays have one set of images that are of higher intensity displayed alongside the original whole body images.  It can be used with bone scans and other whole body (I-131, Ga67, In-111) scans.  There is also a built in dynamic section, which accepts a two-stage dynamic image (a flow, then an eight frame 60 second/frame phase dynamic for a blood pool).  Both the flow and blood pool are composited and displayed next to the appropriate delay image.  You can see our SOP for Whole Body Bone Scans and SPECT Bone Scans (PDF format).  It has been updated to include automatic labeling of most routine images and setting the Institution ID for ACR accreditation; Institution ID is a HARDCODED VARIABLE and REQUIRES editing lines 206 & 210 of the script to put in your instition's name.

#Brain Flow (Brain Death)  
This script takes three dynamic acquisitions (90sec, 1.5s/fr) and compresses/composites them into a flow and blood pool for the determination of brain death.  This methodology was necessary due to software incompatibilities between our old ADAC Transcam camera and the Xeleris software;  if you acquire your brain flows differently it should be relatively easy to modify the script.  You can see the SOP for Brain Death Studies as well.  (PDF format).  It has been updated to include automatic labeling of most routine images and setting the Institution ID for ACR accreditation; Institution ID is a HARDCODED VARIABLE and REQUIRES editing lines 110 & 114 of the script to put in your instition's name.

#Hida   
Dynamic filling of GB. 1 min frame per frame for 60 min, two acquisitions

#Lung Scan (Xe133/Tc99m/Co57)  
At our facility, we acquire lung scans with a ventilation (Xe-133) and six perfusion images (Tc-99m MAA).  We also perform a Co57 transmission image to assess lung size/shape instead of a CXR.  The "first breath" section of the image is extracted by the script from the acquisition.  Here is our SOP for a V/Q Lung Scan (PDF format).  It has been updated to include automatic labeling of most routine images and setting the Institution ID for ACR accreditation; Institution ID is a HARDCODED VARIABLE and REQUIRES editing lines 136 & 140 of the script to put in your instition's name.  Can also handle eight view perfusion only, or 8 view perfusion with ventilation.

#Renal Analysis (ERPF)  
I modified the Renal Analysis program to allow the calculation of an ERPF.  The second modification allows the addition of an accession number.  These are written up as "modification" files - follow the directions to modify your own files in place.  It may make more sense when you see our SOP for Renal Scans.

#Gastrointestinal Bleed  
At our facility we moved to acquiring two 45-minute serial dynamic scans for gastrointestinal bleed studies.  This script compresses them to 5min/fr to allow displaying each 45 minute segment at a time, then also allowing all 90 minutes to be viewed on the same screen.  At the bottom right of that screen is a location where the whole study can be displayed in 1min/fr cine mode.  Up to two delayed images can also be displayed on the main review screen.  It has been updated to include automatic labeling of most routine images and setting the Institution ID for ACR accreditation; Institution ID is a HARDCODED VARIABLE and REQUIRES editing lines 115 & 119 of the script to put in your instition's name. 

#Blood Volume  
This archive is two Excel sheets to aid in the calculation of red blood cell volumes using Cr51.  It includes the DuBois method of determining BSA.  You may also see our SOP for Red Cell Volumes (without RISA) in PDF format. 

#History Template  
A one-page template our facility uses to convieniently record history, dosages, technologist involvement, and other pertenient data. 

#Myocardial Perfusion Information  
A two-page information sheet (intended as a front/back single sheet) information sheet for patients at our facility for a same-day Cardiolite myocardial perfusion study.  PDF format.  You can also see our SOP for myocardial perfusions, a guide to using Xeleris' motion correction, and how to ensure QGS/QPS has drawn accurate countours.  (Yes, we use both ECToolbox and Cedars.) 

#Gastric Emptying Excel Sheets  
Two Excel sheets to calculate gastric emptying.  The first is a straightforward Tc solid gastric emptying;  the second is a more complex one that includes In-111 spilldown for solid/liquid combined studies.  Both include radioactive decay in calculating the T1/2.  You can see our SOPs for Solid Gastric Emptying, Liquid Gastric Emptying, and Combined (Liquid/Solid) Gastric Emptying (PDF format).  Please see the research I did that led our facility to stop doing combined liquid/solid gastric emptying studies.  (PDF format). 

#Fix Modality  
A small modification script to fix the Xeleris system's habit of (incorrectly) marking results series as OT modality instead of NM.
