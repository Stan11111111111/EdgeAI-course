---
layout: post
title: Edge AI MCU Capstone Projects
author: [Richard Kuo]
category: [Lecture]
tags: [jekyll, ai]
---

Edge AI MCU Capstone Projects

---
## Edge AI MCU Capstone Projects

<table>
<tr><th>AI Type </th><th>Applications</th><th>Peripherals   </th><th>AI Feature         </th><th>NN model      </th><th>required APIs/Examples</th></tr>
<tr><td>表情偵測</td><td>機器寵物 </td><td>Camera        </td><td>Image Classification  </td><td>CNN           </td><td>API for CNN       </td></tr>
<tr><td>掌紋辨識</td><td>門禁系統 </td><td>Camera        </td><td>Image Classification  </td><td>CNN           </td><td>API for CNN       </td></tr>
<tr><td>聲音互動</td><td>Stunt Car</td><td>microphone    </td><td>Audio Classification  </td><td>Audio NN      </td><td>API for Audio classifier</td></tr>
<tr><td>自動駕駛</td><td>Stunt Car</td><td>Camera+MPU9250</td><td>Object Detection      </td><td>CNN+LSTM      </td><td>API for YOLOv7    </td></tr>
<tr><td>強化學習</td><td>Stunt Car</td><td>Camera+MPU9250</td><td>Reinforcement Learning</td><td>CNN+LSTM      </td><td>RL-DQN sample code</td></tr>
<tr><td>姿態偵測</td><td>體感遊戲 </td><td>Camera        </td><td>Pose Detection        </td><td>CNN+LSTM      </td><td>API for CNN+LSTM </td></tr>
<tr><td>動作偵測</td><td>體感遊戲 </td><td>MPU9250       </td><td>Hand/Body Movement    </td><td>CNN+LSTM      </td><td>API for CNN+LSTM </td></tr>
<tr><td>生成式AI</td><td>穿戴式chatGPT</td><td>mic + 1.14" TFT</td><td>Audio recording  </td><td>N/A           </td><td>API for Audio clipping</td></tr>
<tr><td>生成式AI</td><td>Text-to-Code</td><td>none </td><td>(Over-The-Air)</td><td>N/A</td><td>N/A</td></tr>
</table>

### 專題計畫之週邊及載具
<table>
<tr><td><img width="50%" height="50%" src="https://gcs.rimg.com.tw/g1/f/b4/cd/22326084867277_915.jpg"></td></tr>
<tr><td><img width="50%" height="50%" src="https://gcs.rimg.com.tw/g4/e40/afa/jif9j8j8/f/3d/2a/22347200521514_469.jpg"></td></tr>
<tr><td><img width="50%" height="50%" src="https://gcs.rimg.com.tw/g9/3c3/78b/ff742155456/d/4e/22139378684238_637.jpg"></td></tr>
<tr><td><img width="50%" height="50%" src="https://gcs.rimg.com.tw/g5/cad/e0b/davidhadson493/f/43/3d/22347198425917_866.jpg"></td></tr>
</table>

---
## wearable chatGPT
<iframe width="505" height="284" src="https://www.youtube.com/embed/JA1CGnsKrSE" title="AI Pin 最新的AI科技有多蠢！？" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<iframe width="505" height="284" src="https://www.youtube.com/embed/ZCVDDcTL8xQ" title="World&#39;s First ChatGPT AI Smartwatch" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

*So wearableGPT device is not good enough, what do we do to design a better one ?*<br>

### ask [ChatGPT](https://chat.openai.com/)

**User:** `What advanced features should I cover in a wearable chatGPT device ?`<br>

**ChatGPT3.5**: <br>
```
To make your wearable ChatGPT device stand out and provide a rich user experience, you can consider incorporating the following advanced features:

Multimodal Input:
Support multiple input methods, such as touch, voice commands, and gestures. Users could switch between these modes based on their preferences or the context.

Real-time Language Translation:
Implement a feature that allows users to translate conversations in real-time. This can be particularly useful for international travelers or users communicating with people who speak different languages.

Contextual Awareness:
Enhance the device's ability to understand and maintain context in conversations. This could involve remembering previous interactions, allowing users to refer back to past messages, or recognizing and adapting to changes in conversation topics.

Personalization and User Profiles:
Develop a system that learns user preferences over time, tailoring responses based on individual history and preferences. Users could have profiles that store preferences, frequently used phrases, and more.

Emotion Recognition:
Implement emotion recognition to make the interactions more natural and personalized. The device could adjust its tone or responses based on the emotional context of the conversation.

Integration with Smart Home Devices:
Allow users to control and interact with their smart home devices using voice commands through the wearable. This could include adjusting lights, thermostats, or other connected devices.

Offline Mode:
Develop a mode that allows basic functionality even when the device is not connected to the internet. This could include preloaded responses or basic tasks that can be performed without an active internet connection.

Adaptive Learning:
Implement machine learning algorithms that adapt to user behavior and feedback, continuously improving the device's performance and understanding of user preferences.

Navigation Assistance:
Provide navigation assistance using GPS and augmented reality. Users could receive turn-by-turn directions or points of interest information through the wearable device.

Biometric Sensors:
Integrate biometric sensors to track health-related metrics, such as heart rate, stress levels, or activity. This data can be used to provide personalized recommendations or trigger alerts based on the user's well-being.

Collaborative Features:
Enable collaborative functionalities, allowing multiple users with compatible devices to engage in group conversations or share information seamlessly.

Voice Synthesis Customization:
Allow users to customize the voice synthesis of the device, choosing from a variety of voices or even mimicking the voices of friends or family members.

Automatic Summarization:
Implement a feature that summarizes lengthy messages or conversations, providing users with concise information.

Security and Privacy Features:
Incorporate advanced security measures, such as biometric authentication or encrypted communication, to protect user data and maintain privacy.

Third-party Integrations:
Allow integration with third-party applications or services, expanding the device's capabilities and enhancing its usefulness in various contexts.

Remember to conduct thorough user testing to ensure that these features enhance the user experience rather than overwhelming users. Regular updates and improvements based on user feedback can contribute to the long-term success of your wearable ChatGPT device.
```

### To-Do Feature List :
1. Multimodal Input: `Touch, Audio, Voice Command, Gesture, Facial...`
2. Context Awareness: `train a Context-aware LLM`
3. Personalization : `User preference profile`
4. Emotion Recognition : `integrate Emotion Detection`
5. Integration with Smart Home Devices : `activate Vaccum Robot, Air Fryer, Smart Oven, ...`
6. Offline Mode : `memory & statemachine`
7. Adaptive Learning : `ML user behavior and feedback to improve device performance`
8. Navigation Assistance : `turn-by-turn direction & point-of-interest info`
9. Biometric Sensors : `health monitoring`
10. Collaborative Features : `multi-users multi-devices collaboration`
11. Voice Synthesis Customization : `Voice Changer`
12. Automatic Summarization : `summary of a length conversation`
13. Securtiy and Privacy Features : `Edge-AI blockchain`
14. Third Party Integration : `AI-Phone, AI-PC, AI-TV`

---


<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*

