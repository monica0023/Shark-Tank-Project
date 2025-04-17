🧠 MemoTag – Speech Intelligence for Early Cognitive Risk Detection

This project analyzes anonymized voice clips from the Mozilla Common Voice dataset to detect potential early signs of cognitive impairment such as memory issues, slowed speech, or reduced fluency.

📍 Goal: Build a lightweight, explainable, and scalable pipeline to extract voice features and detect anomalies using unsupervised machine learning.

📁 Dataset

Source: Mozilla Common Voice (English)

Samples Used: 10 audio clips (e.g., common_voice_en_42693855.mp3)

Format: .mp3 files, ~5–10 sec each

🛠️ Features Extracted

Feature	Description

🗣️ speech_rate	- Words per second (wpm estimate)

😶 hesitation_count - 	Filler words like “uh”, “um”, “er”

🎵 pitch_mean	 - Average voice pitch (from librosa)

🎶 pitch_std - 	Pitch variation (standard deviation)

🧾 word_count - Total words spoken

⏸️ pauses - 	Silence duration between words

📊 similarity_score	Optional: match spoken vs. expected sentence

🤖 ML Approach

✅ Isolation Forest

Unsupervised anomaly detection

Flags “at-risk” speech patterns without labeled data

Visualized using pitch vs speech rate

📈 Sample Output

bash
Copy code
Filename: common_voice_en_42693856.mp3
Speech Rate: 1.2 wps
Hesitations: 4
Pitch Mean: 250 Hz
Pitch Std: 200
--> Risk Level: ⚠️ At Risk

📌 Key Highlights

📦 Uses OpenAI Whisper for transcription

📊 Feature Engineering with librosa, difflib, and basic NLP

📉 IsolationForest from scikit-learn for anomaly detection

📍 Interpretable results for future clinical applications

💡 Credits

Dataset by Mozilla Common Voice

Model: OpenAI Whisper, Librosa, Scikit-learn

Project by Monica for MemoTag's Speech Intelligence Module

📬 Contact

For collaboration, reach out via https://www.linkedin.com/in/monica-r-tech-innovator/ or monica.r.041002@gmail.com.
