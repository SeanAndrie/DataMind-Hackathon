# RecognAIze-Hackathon

"In secure workplaces and restricted environments, surveillance systems play a critical role in ensuring that only authorized personnel are present. This competition invites participants to develop intelligent computer vision models and pipeline that can detect and identify employees in CCTV frames using provided reference photos.

Your mission is to build an AI solution capable of:

Face Identification – Match each detected face to a known employee from a gallery of reference photos, or flag it as "unknown" if no match exists.

Participants will work with real-world CCTV imagery that presents natural challenges like varied lighting, camera angles, occlusions, and crowded environments—making this a realistic testbed for surveillance and access verification AI system"

This our team's machine learning pipeline for the **RecognAIze Hackathon** hosted by DataMind at 42 Abu Dhabi.

Our solution puts great emphasis on *efficiency* and *simplicity* as the reidentifcation process is mainly done by a linear classifier.

It was able to achieve performance comparable to that of more complex implementations (particularly neural networks) due to:

- smart feature extraction and engineering;
- a efficient cross-validation strategy; as well as
- hyperparameter tuning.
