# reMind.ai

### Microsoft Imagine Cup 2024 Qualifier 


https://github.com/user-attachments/assets/9a41d2a6-92bc-4f52-85ae-71b194d119da


Demo Video:  [https://drive.google.com/file/d/1y3BqHG6NisGqMY5_vk6v9wgHm5YMdr20/view?usp=sharing]( https://drive.google.com/file/d/1y3BqHG6NisGqMY5_vk6v9wgHm5YMdr20/view?usp=sharing)

Website Hosted On: https://salmon-sea-0f4b21710.4.azurestaticapps.net/

reMind.ai creates mindmaps from user-inputted .txt, .mp3, .mp4, or .wav files. The original use case for this app is intended for meetings where easy recall of important topics and concepts is necessary. reMind will display a mindmap of the main topic (that encapsulates said meeting) and its respective sub-topics where you can view a "Summary" and "Quotes" of each topic through pop-up interactivity.

## Overview
There are 3 main components to reMind
- A React/Vite frontend using React Flow to render the interactive mindmap
- WhisperAI to convert audio/video (.mp3, mp4, .wav) files to a .txt file
- GPT-3 to convert .txt files (transcripts of meetings) into mindmap format

## Setup
You can replicate this app by running:
```
git clone git@github.com:jhnkim23/reMind.git
cd reMind
docker-compose build
docker-compose up
```
Additionally you can run this code without docker by replacing docker commands by running frontend (react+vite) and backend (django):
```
npm run dev
python manage.py runserver
```
