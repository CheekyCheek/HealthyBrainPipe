# HealthyBrainPipe

This repository houses the scripts necessary to analyze brain imaging genetic data. For this project, we identify significant genetic SNPs associated with brain imaging locations that are highly associated with specific reading disability (dyslexia, as quanitified via behavioral assessment scores).

We will be testing three relevant regularized regression approaches (Ridge, lasso, and elastic net) on brain imaging genetic data to determine the best approach for extracting significant genetic SNPs. 

We will be using three different data types: whole genome data, MRI brain scans, and two clinical reading scores. 

First, we ensure the data is formatted correctly according to the additive genetic model.

Once formatted, we will begin by performing some data reduction.

First, we reduce the number of imaging data points. We do this by regressing the imaging points with the behavioral scores to find the ROI that are significant. We then include these ROI in the regularized regressions with the genetic data. 

We can then select the significant SNPs and analyze them for their importance in the SRD. 
