
Our first goal was to investigate how the whole brain response relates to stimulus complexity. To do this, we applied PCA to trial-averaged functional EEG data in response to different classes of visual stimuli. We found that the PCs for familiar, unfamiliar, and scrambled faces shared some overlap. Overall this suggests that cortex wide processing of visual information is capable of expressing a finite repertoire of principal components and that a subset of those components is employed for any given stimulus. We note that even though the EEG responses to different stimuli occupy some similar dimensions, this does not imply that the responses activate the same regions of the PC subspace. The activity we measure may covary along the same dimensions but be centered at different locations in the functional EEG space. Future work can look into whether this activity is centered in the brain. 

Our second goal was to understand the frequency patterns that V1 uses to process images of varying complexities. We performed this analysis by separating frequencies into smaller bands rather than individual components or features to create a simple and interpretable model. From our band-level analysis, we found little overlap between the frequency pattern components of different stimuli responses. However, in comparison to the trends seen in Fig. 3c, the dimensions for image combinations increased similarly to the combinations of the responses they invoke. Perhaps the number of frequency components used to explain an image scale up with image complexity. In the future, this could be further studied by decomposing the signal into more basic frequency components using a wavelet transform method.  
From our model and ranked features we noted that the top 20 channels needed for feature classification come from V1. This suggests the stimulus-driven patterns are best discerned in V1 and not in other areas along the visual pathway. For future work, it would be interesting to connect the results from the whole-brain PCA to see what specific regions are similar/different for the varying stimuli. 


The basic LSTM model, though a basic version, then ran for 4 folds over the 16 subjects in the datasets, gives an overall accuracy of  34.7%. On the other hand, the MALSTM-FCN model which improves on the basic LSTM module achieves an overall performance of 69.4% over the same dataset


1. Add NPA to the directory: https://github.com/crocodoyle/npa
2. Create a directory called ds00017 in the root and keep the data in the ds00017 folder
3. Create and activate the virtual environment: 
            a. conda env create -f environment.yml -n ee6790
            b. conda activate ece6790
            c. conda install -c conda-forge shap
4. Run the classifier.py as follows:
            python3 classifier.py
