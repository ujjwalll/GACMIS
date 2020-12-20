# GACMIS

Indian Songs Classification Datasets and Machine learning models. GACMIS stands for: (Genre Automated Classification using Machine Learning of Indian Songs). Our main goal through this project is to handle the mis classification problem Indian music genre on popular streaming applications. There is lots of work done for western music classification but very little for Indian music.

## Dataset Details.

This dataset contains 7 major Genres of Indian music, and contains around 100 songs (6 Hr in duration approx.) in each genre.

Genres are classified as shown below:

- <b>Bhajan</b>: Bhajan refers to any devotional song with religious theme or spiritual ideas, specifically among Indian religions, in any of the languages from the Indian subcontinent.
- <b>Bhojpuri</b>: Bhojpuri music includes a broad array of Bhojpuri language performances in distinct style, both traditional and modern. This from of music is mostly created in Indian states of Bihar, Uttar Pradesh and Jharkhand and other countries like Nepal, Suriname, Guyana, Netherlands, Mauritius and other Caribbean Islands.
- <b>Sufi</b>: Sufi music is the devotional music of the Sufis, inspired by the works of Sufi poets, like Rumi, Hafiz, Bulleh Shah, Amir Khusrow and Khwaja Ghulam Farid. Qawwali is the best-known form of Sufi music, and is most commonly found in the Sufi culture in South Asia
- <b>Raga</b>: A raga or raag is a melodic framework for improvisation akin to a melodic mode in Indian classical music. While the rāga is a remarkable and central feature of the classical music tradition, it has no direct translation to concepts in the classical European music tradition.
- <b>Ghazal</b>: The ghazal is a form of amatory poem or ode, originating in Arabic poetry. A ghazal may be understood as a poetic expression of both the pain of loss or separation and the beauty of love in spite of that pain. The ghazal form is ancient, tracing its origins to 7th-century Arabic poetry
- <b>Bollywood (Romantic)</b>: Bollywood pictures and albums romantic songs.
- <b>Bollywood (Rap)</b>: New kind of Bollywood music, inspired from west. 


## Data modeling and feature ectraction.

We have curated a list of features that needs to be extracted for our Model.

- Zero Cross Rate
- Energy
- Entropy of Energy
- Spectral Centroid
- Spectral Spread
- Spectral Entropy
- Spectral Flux
- Spectral Roll off
- MFCC
- Chroma Vector
- Chroma Deviation
- pitch

Description of these features cn be found on our manuscipt. Manuscript is present in manuscript folder.

## Data Preparation

We have done deep data analysis of the songs that we got. As we have created our dataset from scratch, We tried to make sure that our data integrity is strong. We have created list of songs, cross verified them from several sources, then incluced them. We also tried to make sure that classes are not very much imbalanced. We have extracted features with the help of Librosa and pyaudio libraries. We also make sure that our dataset is free of 30 sec anamoly, hence included whole song instead of small fragments.

## Models we trained

We have trained several models on our dataset, here we are presenting Top 5 classifiers which gives us best results.

- SVM (Support Vector Machine)
- Gradient Boost
- Light GBM 
- Neural Network
- kNN (k nearest neighbours)

We have taken Logistic regression as our baseline model which gives us 69.09 % accuracy after hyperparameter tuning.

## Weights

All the weights are saved under weights model, as we have also applied many permutations to find best features, we haven't uploaded all the models weight, just the best model weights of each model.


## Literature Review.

If you want to learn more about this problem, we have curated few good papers to read to get a start, you can find them in Literature Review Folder.

Disclaimer: Data and Songs scrapped only and only for research purposes. Any mal distribution/commercial distribution of this content is illegal. Please make sure you are not using any data or song for any non research purpose.
