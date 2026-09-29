https://teachablemachine.withgoogle.com/

![Week 5 Assignment-01](https://raw.githubusercontent.com/al3xxli/TDF-Weekly-Journals/main/embeds/Week%205%20Assignment-01.png)

Trained Object Classifier: Focus Timer
This one works by identifying two simple hand gestures, peace✌️ and thumbs up👍. I would pose peace for the focus timer to start, and it's always set at 45-minute intervals (it's what works best for me). Thumbs up would stop the focus timer, marking the end of the session.
Link: 
Training Files: [Link](https://drive.google.com/drive/folders/1x2B8TfECzNnFM97mm2SBs9ecmqVcszMw?usp=sharing)

Trained Pose Classifier: Shrimper (extra credit project)
The Shrimper is a posture detector that is trained specifically for me at my workstation since the webcam will always be mounted in a constant position.
Link: 
Training Files: [Link](https://drive.google.com/drive/folders/1PIsjDu4sH4eh_EtTp1mup7L88GemcjUE?usp=sharing)

Journal Entry: The datasets were pretty easy to set up, since the functions were dependant on either a specific object (in the first case, numbers) or the camera is mounted to a fixed position, making it easier for the classifiers to detect changes. For the Shrimper, I put on different t-shirts and took videos (using FFmpeg for frames) to hopefully provide a robust level of data. (write more here about a data key)