The app is intended to help people with Autism, where their voices are hard to understand for general public, yet still recognizable to parents/siblings. To achieve such task, we use google TFLite model maker to retrain with voices of specific individual, then use Google's MediaPipe for audio classification. 
1. modelMaker uses customized voice data to generate model data
2. app uses generated model data to recognize voices of the same person.

