
# [ONGOING] **Multimodal Mental Health Monitoring with LLM Explanations**

**Objective:** Develop a multimodal AI system that predicts mental health states (e.g., stress, anxiety, depression) in college students by integrating high-frequency physiological time-series data from wearables with contextual features (e.g., activity, location). The system should not only make accurate predictions but also provide human-readable natural language explanations of the physiological and contextual patterns driving each prediction using a Large Language Model (LLM).

**Challenges:**

  * Temporal Dynamics: Modeling per-second wearable sensor data to capture short-term and long-term physiological trends.

  * Multimodal Fusion: Combining numeric time-series embeddings with categorical contextual information in a form suitable for reasoning by an LLM.

  * Natural Language Reasoning: Translating sensor signals and context into interpretable textual explanations for mental health states.

  * Noise & Missing Data: Handling artifacts, missing seconds, and irregular sensor readings without degrading prediction or explanation quality.

  * Evaluation of Explanations: Measuring both prediction accuracy and the relevance/clarity of the LLM-generated reasoning.


**Solution Approach:**

* Aggregate per-second sensor readings to manageable windows (e.g., per minute) and encode as temporal embeddings.

* Convert categorical context/activity features into textual tokens for the LLM (e.g., “Student is in the library”) or embeddings.

* Fuse temporal embeddings and textual embeddings via cross-attention layers so the LLM can jointly reason over physiology and context.

* Train the model to output both:

* Predicted mental health state per window, and

* A natural language explanation summarizing which physiological trends and contextual factors contributed to the prediction.

* Evaluate using classification metrics (accuracy, F1-score) for predictions and human/automatic metrics (BLEU, ROUGE, clinical interpretability) for explanations.
