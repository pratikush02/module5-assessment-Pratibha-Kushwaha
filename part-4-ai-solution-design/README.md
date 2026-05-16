Part 4: AI Solution Design for a Business Problem



**Task 1: Choose a Business Domain**

Selected Domain - Healthcare 



\---------------------------------------------------



**Task 2: Define the Business Problem**



* What problem is being solved?

  * Doctors get too many medical images like chest X-rays and it takes a lot of time to check all of the images. AI can help sort which ones look urgent



* Who are the users or stakeholders?

  * Doctors, radiologists, patients are the users or the stakeholders



* What is the current manual or traditional process?

  * Doctors manually review every image which is very time consuming.



* What are the limitations of the current process?

  * The current process is very Slow, risk of missing urgent cases, delays in treatment.



\---------------------------------------------------



Task 3: Identify the AI Task Type

**Answer:**

This is an Image classification problem because the AI looks at an image and decides: “Normal” or “Abnormal.”

Example: AI sees an X-ray → predicts if there’s congested chest or not.



\---------------------------------------------------



Task 4: Data Requirement Plan

**Answer:**

* Type of data: X-ray or CT scan images.
* Structured or unstructured: Unstructured (images).
* Input features: Pixel values of the image.
* Target variable: Label (e.g., “healthy” or “disease”).
* Data collection: Hospital imaging systems.
* Data quality risks: Blurry scans, mislabeled data, privacy concerns.



\-----------------------------------------------------



Task 5: Model Recommendation

**Answer:**

The model recommendation in this case study, we will use Convolutional Neural Network (CNN).



CNNs are great at spotting patterns in images (like edges, shapes, textures). Transfer learning (using a pre-trained model like ResNet) can help in speeding the findings with improved accuracy.



\-----------------------------------------------------

Task 6: Evaluation Plan

**Answer**:

Technical metrics: Recall, sensitivity, accuracy.

Business metrics: Faster review time, fewer missed diagnoses, improved patient outcomes.

Failure cases: AI misses rare diseases, or flags too many false alarms.

Human review: Doctors always double-check AI suggestions.



\-----------------------------------------------------



Task 7: Responsible AI Considerations

**Answer:**

Bias in data: If training data is mostly from one region, AI may not be able to generalize the findings.

Incorrect predictions: It could harm patients if remained unchecked.

Privacy concerns: Medical images must be stored securely.

Over-reliance: Doctors should use AI as support, not as a replacement.

Human oversight: AI highlights urgent cases, but doctors make the final call.



\-----------------------------------------------------

Task 8: Final Solution Summary

Problem: Doctors spend too much time reviewing medical images, risking delays.

Proposed AI solution: Use CNN-based image classification to triage urgent cases.

Required data: X-ray/scan images with disease labels.

Model recommendation: CNN with transfer learning.

Expected business impact: Faster diagnosis, reduced workload, better patient care.

Risks \& mitigation: Bias, privacy, misdiagnosis → solved by diverse training data, secure storage, and mandatory doctor review.

