<h1 align="center">Deep Learning–Based Inappropriate Content Detection and Classification on YouTube Videos</h1>

<p align="center">
<b>Automatic detection and classification of inappropriate (violent) and safe content in YouTube videos using deep learning models</b>
</p>

<hr>

<h2 id="table-of-contents">📑 Table of Contents</h2>

<ul>
  <li><a href="#overview">Overview</a></li>
  <li><a href="#problem-statement">Problem Statement</a></li>
  <li><a href="#dataset">Dataset</a></li>
  <li><a href="#tools-and-technologies">Tools and Technologies</a></li>
  <li><a href="#project-structure">Project Structure</a></li>
  <li><a href="#methodology">Methodology</a></li>
  <li><a href="#experimental-results">Experimental Results</a></li>
  <li><a href="#how-to-run">How to Run This Project</a></li>
  <li><a href="#applications">Applications</a></li>
  <li><a href="#future-scope">Future Scope</a></li>
  <li><a href="#author-contact">Author & Contact</a></li>
</ul>

<hr>

<h2 id="overview">📌 Overview</h2>
With the rapid growth of online video platforms like YouTube, the spread of inappropriate and violent content has become a serious concern. Manual moderation is inefficient and does not scale well with the massive volume of uploaded videos.  
This project proposes a deep learning–based approach to automatically detect and classify YouTube video content as <b>Safe</b> or <b>Inappropriate</b> by analyzing visual features extracted from video frames.

<hr>

<h2 id="problem-statement">⚠️ Problem Statement</h2>
Inappropriate and violent content on video-sharing platforms negatively affects users, especially children, and damages platform credibility. Traditional rule-based or manual moderation systems are slow, inconsistent, and expensive. There is a strong need for an automated, accurate, and intelligent content classification system that can efficiently identify inappropriate content in videos.

<hr>

<h2 id="dataset">📊 Dataset</h2>
The dataset consists of image frames categorized into two classes:
<ul>
  <li><b>Normal:</b> Safe and non-violent content</li>
  <li><b>Violence:</b> Inappropriate and violent content</li>
</ul>
These images are extracted from videos and used to train and evaluate the deep learning models. Test videos containing violent and non-violent scenes are used for final classification.

<hr>

<h2 id="tools-and-technologies">🛠️ Tools and Technologies</h2>

<ul>
  <li><b>Programming Language:</b> Python</li>
  <li><b>Deep Learning Frameworks:</b> TensorFlow, Keras</li>
  <li><b>Models Used:</b>
    <ul>
      <li>EfficientNetB7 + BI-LSTM-GRU (Proposed Model)</li>
      <li>EfficientNetB7 + SVM (Comparison Model)</li>
    </ul>
  </li>
  <li><b>Libraries:</b> NumPy, OpenCV, Matplotlib</li>
  <li><b>Development Environment:</b> VS Code</li>
  <li><b>Operating System:</b> Windows</li>
</ul>

<hr>

<h2 id="project-structure">📁 Project Structure</h2>

<pre>
youtube-inappropriate-content-detection
├── data
│   ├── normal
│   └── violence
├── models
│   ├── bilstm_weights.hdf5
│   ├── content_model.h5
│   ├── model_weights.hdf5
│   ├── x.txt.npy
│   └── y.txt.npy
├── scripts
│   ├── main.py
│   └── run.bat
├── videos
│   └── testVideos
├── results
│   └── screenshots
├── docs
│   ├── Project_Report.pdf
│   └── Project_Presentation.pptx
├── requirements.txt
├── README.md
└── .gitignore
</pre>

<hr>

<h2 id="methodology">🧠 Methodology</h2>
The system processes video data by extracting frames and performing image-based classification. The workflow includes:
<ul>
  <li>Uploading and preprocessing the dataset</li>
  <li>Feature extraction using EfficientNetB7</li>
  <li>Temporal learning using BI-LSTM-GRU</li>
  <li>Training and evaluating models</li>
  <li>Comparing performance with an SVM-based model</li>
  <li>Classifying test videos as Safe or Inappropriate</li>
</ul>

<hr>

<h2 id="experimental-results">📈 Experimental Results</h2>
The proposed EfficientNetB7 + BI-LSTM-GRU model achieved superior performance compared to the baseline model.

<ul>
  <li><b>Proposed Model Accuracy:</b> 99.04%</li>
  <li><b>EfficientNetB7 + SVM Accuracy:</b> 88%</li>
</ul>

Confusion matrix and comparison graphs confirm that the proposed deep learning model significantly reduces misclassification and improves detection accuracy.

<hr>

<h2 id="how-to-run">▶️ How to Run This Project</h2>

<ol>
  <li>Clone the repository to your local system.</li>
  <li>Navigate to the project directory.</li>
  <li>Install required dependencies using <code>requirements.txt</code>.</li>
  <li>Run the application using <code>main.py</code> or <code>run.bat</code>.</li>
  <li>Upload dataset and test videos through the interface.</li>
</ol>

<hr>

<h2 id="applications">🚀 Applications</h2>
<ul>
  <li>YouTube and social media content moderation</li>
  <li>Violence detection in surveillance videos</li>
  <li>Child safety and parental control systems</li>
  <li>Media screening and filtering platforms</li>
</ul>

<hr>

<h2 id="future-scope">🔮 Future Scope</h2>
Future improvements may include real-time video stream analysis, audio-visual content fusion, multi-class content categorization, and deployment as a cloud-based web application.

<hr>

<h2 id="author-contact">👤 Author & Contact</h2>

<b>Rishab Sakale</b><br>
Electronics and Communication Engineering Graduate<br>
Aspiring Software & Machine Learning Engineer<br>
GitHub: <a href="https://github.com/Rishab-Sakale">https://github.com/Rishab-Sakale</a><br>
Email: <a href="mailto:rishab7036@gmail.com">rishab7036@gmail.com</a>
