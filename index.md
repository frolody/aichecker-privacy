# Privacy Policy & Terms of Service
**AIChecker: AI Detector (for Video & Image)**  
*Last updated: November 2026*

This Privacy Policy explains how **AIChecker: AI Detector** ("AIChecker", "we", "our", or "the App") handles information when you use our mobile application. We are committed to protecting your privacy and ensuring transparency regarding our technical architecture and data processing.

---

## 1. Summary — Privacy by Design
- **No User Account Required:** We do not collect names, email addresses, phone numbers, or passwords.
- **Privacy-Centric Advertising:** We use Google AdMob to display banner and interstitial ads to support free service. We do not sell your personal data or maintain tracking profiles.
- **Local Storage:** Your scan history, analysis logs, and thumbnails are stored exclusively on your device.
- **Ephemeral Media Processing:** Selected videos and images are processed in volatile memory (RAM) solely for the duration of the AI analysis and are not retained on our servers.

---

## 2. Information Handled & How It Is Used

### A. Media Files (Photos and Video Frames)
When you choose to analyze an image or video:
1. The App samples visual frames locally on your device.
2. The sampled frames are transmitted over an encrypted HTTPS/TLS connection to our cloud AI inference server (hosted on Hugging Face Spaces).
3. The AI model (Swin Transformer-B) analyzes visual artifacts (e.g., diffusion noise patterns, frequency anomalies, perspective consistency).
4. As soon as the detection score and forensic breakdown are generated, the frames are immediately purged from server memory.
5. **We never store, log, share, or sell your photos or videos.**

### B. Device Permissions
The App requests only permissions essential for its core functionality:
- **Media / Photo Access:** Required only when you explicitly select a file from your gallery or file manager.
- **Display Over Other Apps (`SYSTEM_ALERT_WINDOW`):** Enables the optional floating overlay button so you can trigger real-time inspection while on video calls.
- **Screen Capture / Media Projection (`FOREGROUND_SERVICE_MEDIA_PROJECTION`):** Used solely when you enable the Overlay Detector to capture on-screen frames for live analysis. It operates only under explicit user activation with a visible foreground notification and can be turned off at any moment.

### C. Local History Storage
The App saves your previous analysis scores, timestamps, and thumbnails locally within the app's sandboxed private storage. You can delete all history records at any time with a single tap using the **"Clear History"** button in the Scan History menu.

### D. Third-Party Advertising (Google AdMob)
To keep the application free for all users, we display advertisements provided by Google AdMob (Google LLC):
- Google Mobile Ads SDK may collect and process pseudonymous identifiers (such as the Android Advertising ID, IP address, and device diagnostic information) to deliver ads, prevent fraudulent clicks, and measure performance.
- We do not share your media files, scan scores, or personal identifiers with Google AdMob.
- You can manage or reset your advertising ID and opt out of personalized ads at any time via Android device settings (**Settings > Google > Ads**).
- For more information on how Google collects and uses advertising data, visit [Google's Privacy & Terms](https://policies.google.com/technologies/ads).

---

## 3. Data Security
All communication between the App and the AI inference backend is protected using industry-standard **HTTPS (TLS 1.2/1.3)** encryption. No plain-text or cleartext network traffic is allowed.

---

## 4. Children’s Privacy
The App does not target or knowingly collect data from children under 13 years of age. Because no personal data is collected or stored, the App complies with global privacy standards, including COPPA and GDPR.

---

## 5. Terms of Service & Disclaimer of Accuracy

### A. Informative and Educational Purpose
AIChecker uses deep learning models (Swin Transformer-B) to evaluate whether media exhibits visual characteristics common in synthetic AI generation (such as Midjourney, DALL-E, Stable Diffusion, Flux, Sora, Kling, Runway).

### B. Probabilistic Output & Limitation of Liability
1. **Probabilistic Estimation:** Detection scores (e.g., "86% Likely AI-Generated" or "Appears Real") represent statistical likelihoods derived from neural network patterns. They do not constitute absolute, certified, or infallible certainty.
2. **Not Legal Evidence:** The outputs of this App are provided for personal verification, awareness, and educational purposes only. They must not be used as the sole basis for legal accusations, judicial proceedings, criminal investigations, or disciplinary actions.
3. **No Warranty:** The App is provided on an "AS IS" and "AS AVAILABLE" basis without warranties of any kind. Under no circumstances shall the developers be liable for any direct, indirect, incidental, or consequential damages resulting from reliance on the detection results.

---

## 6. Updates to This Policy
We may update this Privacy Policy from time to time. Any changes will be reflected in this document with an updated revision date.

---

## 7. Contact Us
If you have questions or feedback regarding this Privacy Policy or the App, please reach out via our project repository or support channel:
- **Project Repository:** https://github.com/frolody/deepfake_analyzer
- **Inference Infrastructure:** Hugging Face Spaces (https://huggingface.co/spaces)
