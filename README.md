# SACC_mlsp
Speech Accent Classification and Conversion based on deep learning technique and etc.


STEPS (** subject to change **)
Audio signal preprocessing
1. Data loading
    1) download the data and save as a matrix according to the label
    2) separate training and testing dataset
2. Fourier transform
3. Quality inspection - Check the spectrum and delete low-quality data
4. Denoising - Clean the background white noises
5. Transcription - Transcribe the audio signal into words

Accent classification
1. Feature extraction
    2.1 PCA analysis on the whole dataset 
    2.2 Represent all the accent with regard to the eigenvectors
    2.3  Use ICA, LDA and t-SNE to extract features as well 
    2.4 Wording embedding of the transcribed words
2. Modeling
    Classification algorithm: Adaboost, CNN, RNN, LSTM

Accent reconstruction
1. Feature extraction
    Multiple feature-extraction algorithm (e.g. PCA/ICA analysis) tested on each group of accent to extract the main features of that specific accent
2. Reconstruction 
    Use the feature of one accent to reconstruct the audio/vocabulary
