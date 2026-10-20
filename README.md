# Cytoskeleton Analysis (BBBC018)

**Student ID:** 202303489  
**Image Field ID:** 15961  
**Phenotype Classified:** Large spread  
- **Actin filename:** 15961-actin.DIB 
- **DNA filename:** 15961-DNA.DIB  

  ## Dataset
This activity uses the BBBC018 fluorescence image dataset of human cells (Ljosa et al., Nature Methods, 2012).  The fluorescence images (`15961-actin.DIB` for F-actin and `15961-DNA.DIB` for nuclei) were used to observe cellular morphology, specifically analyzing the Large spread phenotype. Measuring the cell area, circularity, aspect ratio, and mean actin intensity across five representative cells to quantify cytoskeletal structure and cell shape variations.
- **License:** CC BY-NC-SA 3.0
- **Download link:** https://bbbc.broadinstitute.org/BBBC018

## Fiji Steps
1. Go to the Official Download Page:
     <img width="1361" height="682" alt="image" src="https://github.com/user-attachments/assets/eeb1aced-146a-470c-a821-5a21520fe528" />

  *Figure 1.* The official Fiji download site was accessed to obtain the application package. The Windows x86-64 version was selected for installation 

2. Extract the Compressed Folder:
  <img width="810" height="715" alt="Screenshot (250)" src="https://github.com/user-attachments/assets/788196d0-82a3-456d-a69f-a2e3c43fe27b" />

   *Figure 2.* The downloaded zip file was extracted to "fiji-latest-win64-jdk".

3. Launch Fiji:
   <img width="1125" height="619" alt="Screenshot (253)" src="https://github.com/user-attachments/assets/1c6c8408-d896-4c1a-b460-f8c1bd817458" />

   *Figure 3.* The new unzipped fiji-latest-win64-jdk folder was opened and Fiji was launched.

4. Set Measurements:
  <img width="312" height="488" alt="Screenshot (254)" src="https://github.com/user-attachments/assets/9efc9286-aa39-414b-9628-7b6f26c25d16" />

   *Figure 4.* Measurements were configured in Fiji by checking Area, Mean gray value, Min & max gray value, Shape descriptors, and Display label.

5. Open ROI Manager:
  <img width="192" height="289" alt="image" src="https://github.com/user-attachments/assets/7e3bfe60-7c4a-4f2c-a945-e741a47b2f55" />

   *Figure 5.* The ROI Manager was opened by navigating to Analyze > Tools > ROI Manager.

6. Import Bio-Formats:
  <img width="450" height="562" alt="Screenshot (263 1)" src="https://github.com/user-attachments/assets/8eb45e92-315f-423c-a87f-e25374b9950a" />  <img width="246" height="288" alt="Screenshot (263)" src="https://github.com/user-attachments/assets/7dd00dec-61d8-4bf0-ac87-0bfc44daf1fe" />

   *Figure 6.* File > Import > Bio-Formats was selected to import microscopy images for analysis.

7. Open Image Files:
  <img width="1366" height="610" alt="Screenshot (266)" src="https://github.com/user-attachments/assets/520af047-55f2-42e9-a72d-6b596b07521b" />

   *Figure 7.* The 15961-actin and 15961-DNA image fields were uploaded and opened.

8. Trace Cells and Record Measurements:
   <img width="522" height="623" alt="Screenshot (267)" src="https://github.com/user-attachments/assets/10ab2fb1-5d07-4e50-a842-765d04c8c6b3" />

   *Figure 8.* Individual actin cells were selected and traced using the freehand tool, followed by pressing T and M to save the regions to ROI Manager and measure all 5 cells.

9. Complete Results:
  <img width="1366" height="768" alt="Screenshot (275)" src="https://github.com/user-attachments/assets/6752d0fe-71ac-47fe-8d9a-ce5d8070d980" />  

   *Figure 9*. The complete results were displayed, showing the DNA image, measured cells, ROI Manager, and the final measurements table in Fiji.

## Plot
<img width="900" height="650" alt="actin_intensity" src="https://github.com/user-attachments/assets/4f468f20-37c9-4552-9bc3-2d3523e4609e" />

*Figure 10.* Actin Signal Intensity of Large Spread Cells. The graph shows the mean actin fluorescence intensity of five cells. Cell 4 and Cell 2 show the highest intensity values, while Cell 1 shows the lowest, demonstrating variation in actin concentration across the spread cells.

<img width="900" height="650" alt="area_vs_circularity" src="https://github.com/user-attachments/assets/f0ea1917-73ae-41a2-9efd-037657bb3409" />

*Figure 11.* Relationship Between Cell Area and Circularity During Large Spread. The graph shows the relationship between cell area and circularity across the five cells. Cell 3 exhibits a smaller area with high circularity (~0.93), whereas Cell 5 exhibits a much larger area (~905 px²) with lower circularity (~0.63). This reflects morphological diversity in the spread phenotype.

## Discussion Questions

1. Which specific phenotype did you choose, and what visible features support that choice?
- I selected the Large spread phenotype using image field 15961. Looking at the image, you can clearly see that the cells are wide and flat across the surface rather than rounded or clumped, with visible actin fibers spreading out over a large area.

2. Were your five cells mostly round or elongated? Refer to your circularity and aspect-ratio results.
- The five cells were mostly round to irregularly spread out, not elongated. Cell 3 was the roundest with a high circularity of 0.928 but a small area of 330 px², while Cell 5 was the largest at 904 px² with a lower circularity of 0.625. With circularity values between 0.535 and 0.931, none of the cells showed the long, thin shape of elongated cells.
  
3. What role does actin play in maintaining cell shape and in cell movement (Karp Chapter 9)?
- Actin microfilaments form a supporting network right under the cell membrane to hold the cell's shape. For movement, actin grows at the front edge to push the membrane forward (forming lamellipodia), while contractions at the back pull the rest of the cell forward.

4. Why can a single fixed fluorescence image NOT show how fast a cell moves?
- A fixed fluorescence image is just a single frozen snapshot, showing only where the cell and its actin are at one moment. To measure speed, you need to track how far the cell moves over time, which requires live-cell video rather than a single fixed picture.
