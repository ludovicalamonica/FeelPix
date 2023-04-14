# FeelPix
Database of labeled data for facial expression recognition based on landmarks coordinates.

---

The FeelPix database is a labeled database extracted during the validation process of the Facial Expression Recognition (FER) algorithm implemented in the Javascript library face-api.js. 

The validation process involved presenting high emotional stimuli, extracted from the NAPS BE database of images, to elicit an emotional response. During the viewing of the images, the subjects' expressions were recorded using the algorithm under investigation. Subsequently, subjects were asked to report the emotions evoked by images to compare their choices with the expressions recognized by the algorithm. 

During the facial recognition, the two-dimensional coordinates of the 68 facial landmarks were extracted to construct the labeled database presented here.
The users' choices represent the ground-truth associated with the data, allowing for the utilization of this database for the training of any Facial Expression Algorithm that uses landmark coordinates to recognize users' expressions.

This open-source database will be useful for researchers and developers working on facial expression recognition algorithms based on landmarks. The objective is to develop a tool that can reduce the problem of generalization in the application of FER algorithms. The data was collected in a multi-contextual setting with a heterogeneous population of subjects who differed in various characteristics, such as age, sex, gender, ethnicity, and culture.

---

The repository is organized as follows:
- High emotional stimuli: contains the data of all the stimuli used to elicit an emotional response in the subjects during landmarks recording.
- Subject data: contains the main characteristics of the subjects participating in the test associated with the identification code that is also reported in the data file.
- Raw data: contains the data collected without any elaboration. The data are listed with the user identification number, the name of the images presented to the users, their choices, and the raw coordinates of the 68 landmarks extracted.
- Processed data: contains the data that have been elaborated using a normalization procedure of the coordinates and an extraction of 22 points identified as informative points based on the FACS manual. This data are listed with the user identification number, the label of the images used to elicit the emotional response, the users' choices of emotions, and the coordinates of the 22 informative points.
