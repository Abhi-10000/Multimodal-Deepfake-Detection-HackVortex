# 🛡️ VeritasGuard: Multimodal Deepfake Authenticator 🎥🔊
# HackVortex 2025 Submission | AI/ML & Open Innovation Domain

✨ Introduction: The New Frontier of Deception
In an era increasingly defined by digital content, the authenticity of what we see and hear online is paramount. The recent unveiling of advanced generative AI models like Google's Veo 3 at I/O 2025 marks a pivotal moment: AI can now create hyper-realistic videos complete with perfectly synchronized, authentic-sounding dialogue and environmental audio.

This capability fundamentally changes the landscape of digital misinformation. Traditional deepfake detectors, often reliant on visual-only or audio-only analysis, are critically unprepared to combat these sophisticated multimodal deepfakes. The ability to easily fabricate compelling audio-visual narratives poses unprecedented risks to trust in media, individual reputations, and democratic processes.

VeritasGuard is our urgent response to this escalating threat.

🎯 Problem Statement: The Multimodal Misinformation Gap
The proliferation of AI-generated content, especially with the advent of tools capable of producing high-fidelity video with integrated audio, creates a significant vulnerability. Existing deepfake detection systems, while effective against older generations of visual-only or audio-only fakes, are blind to the subtle, yet critical, inconsistencies that arise when AI attempts to synthesize complex, synchronized human behavior across both visual and auditory streams.

This gap leads to:

Rapid Spread of Misinformation: Fabricated news, political propaganda, and misleading narratives can spread unchecked.

Enhanced Fraud & Impersonation: Malicious actors can create highly convincing impersonations for financial fraud or identity theft.

Erosion of Trust: The public's ability to discern truth from falsehood in digital media is severely compromised.

There is an immediate and critical need for accessible tools that can analyze both the visual and auditory components of media in conjunction to accurately identify these next-generation multimodal deepfakes.

💡 Our Solution: VeritasGuard - Multimodal Deepfake Authenticator
VeritasGuard is a proof-of-concept web-based application designed to provide an initial, rapid assessment of video authenticity by analyzing both its visual and audio components. Our approach focuses on identifying the subtle "tells" that even advanced generative AIs struggle to perfect when synthesizing synchronized human behavior.

Unique Value Proposition:
Bridging the Modality Gap: We directly address the challenge posed by new multimodal AI generators like Veo 3 by analyzing both video and audio streams for inconsistencies, providing a more comprehensive authenticity check.

Focus on Subtle A/V Inconsistencies: Our system targets the nuanced, synchronized discrepancies (e.g., imperceptible lip-sync errors, uncanny generated voice characteristics) that are harder to perfect across an entire clip.

Accessible Initial Assessment: VeritasGuard offers a quick, easy-to-use first line of defense for journalists, fact-checkers, and concerned individuals, providing a probabilistic assessment to guide further investigation.

🚀 Core Features (Minimum Viable Product - MVP)
Our functional prototype demonstrates the core multimodal detection capability:

Video Upload Interface: A simple web UI DESIGN for users to upload a short video file (e.g., MP4).

Simplified Lip-Sync Inconsistency Detector: Analyzes the video frames and audio track to identify potential misalignments or unnaturalness in lip movements relative to the speech.

Basic Synthetic Voice Detection: Extracts audio features to identify characteristics commonly found in artificially generated voices.

Overall Suspicion Score: Combines the findings from both visual and audio analyses to generate a single, interpretable "Deepfake Suspicion Score" (0-100%).

Brief Anomaly Indication: Provides a short textual message if a specific anomaly (e.g., "Potential lip-sync mismatch," "Synthetic voice characteristics detected") is identified.

🛠️ Tech Stack
Frontend: HTML5, CSS3 (Tailwind CSS for responsive design), JavaScript (Vanilla for UI interactions and API calls).

Backend & AI/ML Core:

Python: The powerhouse for all AI/ML processing.

OpenCV-Python: For video frame extraction, face detection, and facial landmark analysis.

Librosa / Pydub: For robust audio loading, processing, and feature extraction.

SciPy / NumPy: For numerical operations and signal processing.

Pre-trained Models/Simplified Classifiers: Leveraging existing models (e.g., for facial landmarks) or training very basic, lightweight classifiers (e.g., scikit-learn) on minimal datasets for specific anomaly detection.

⚙️ How It Works (High-Level Flow)
User Uploads Video: A user uploads a video file through the web interface.

Backend Processing: The Python backend receives the video.

Video & Audio Extraction: The video is split into individual frames and its audio track is extracted.

Multimodal Analysis:

Visual Analysis: Facial landmarks are detected, and lip movements are analyzed for consistency with speech.

Audio Analysis: Acoustic features are extracted from the audio to detect synthetic voice characteristics.

Score Calculation: The results from both analyses are combined into an overall Deepfake Suspicion Score.

Results Display: The score and any detected anomalies are sent back to the frontend and displayed to the user.

🎬 Screenshots UI DESIGN


Screenshot 1: Upload Interface
![image](https://github.com/user-attachments/assets/e688860c-7b09-4773-81ab-5303e7ef5b13)


Screenshot 2: Analysis in Progress 
![image](https://github.com/user-attachments/assets/5ecaea4a-0680-47e6-98b0-efe2d34ec6b3)


Screenshot 3: Results Displaying Score and Anomaly
![image](https://github.com/user-attachments/assets/004fe482-afab-4723-9282-bbc09e705528)


🛣️ Future Enhancements
Integration with a more robust, larger-scale deepfake dataset for improved accuracy.

Real-time video stream analysis from webcams.

Visual heatmaps indicating manipulated regions in the video.

Detailed forensic reports on detected anomalies.

Integration with content provenance standards (e.g., C2PA) for digital watermarking verification.

API for seamless integration into social media platforms or news verification tools.

Support for more video and audio codecs.

🤝 Team Members
Naga Abhilash V

Shaik Imran

Deveeswara Sarma N

🙏 Acknowledgments
A huge thank you to the HackVortex 2025 organizers for this incredible opportunity!
