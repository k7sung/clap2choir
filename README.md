# clap2choir
Easily create a virtual choir video in Google Drive and run it in Google Colab.


## Instruction for choir members
1. Start recording the video first; **(in horizontal orientation)**
2. Start playing the master track on the headphone, wait for the metronome ticks;
3. Listen for the first 4 ticks, and clap along on the 5-8th ticks. The claps should be crisp and clear. They're the markers for the script relies on to synchronize all the recordings together.
4. Sing along with the music in the master track.
5. Stop the recording when the master track is finished. 
6. The member uploads his/her video to the shared google drive folder, with the file path [Inputs / Song Name]
  1. The naming convention for the file should be: PART_FIRST NAME. (mp4/mov)
  1. For example: S_Alice.mp4 → S for Soprano, A for Alto, T for Tenor, B for Bass. More examples: A1_Alice_1.mp4, B2_Bob_2.mov
  
## Tips for recording
The video doesn’t need to be high resolution since everyone will only occupy a small box in the video. The higher the definition the longer it will take for uploading and processing. Adjust your camera/phone/laptop settings if you can.
iPhone 
Settings > Camera > Record Video > 720p HD at 30 fps (lowest res.)
Samsung
In Camera > Settings > Rear Video Size > Resolution 
If there’s a video you’d like to keep in the inputs folder (say, you have two videos and you’re not sure which one you want to keep yet), you can prefix the file name with an ‘_’. For example, “b_kyle_1.mp4” become “_b_kyle_1.mp4”. The files prefixed with underscores will not be included in the output video.
Try to have everything set up before starting the recording. Noises from adjusting the camera/microphone etc can interfere with the processing. Record the video in horizontal orientation because the python library used (moviepy) doesn't seem to like vertical orientation.

## Instruction for choirmaster
You need to create a master piano recording for everyone to follow. The beginning of the master recording should have 8 beats of metronome clicks. You can get metronome clicks here https://www.google.com/search?q=metronome. After the clicks, pause for a few seconds and then start playing the music. If you want to include the master recording video in the output video, you should name the file with an "M" at the beginning. For example, M_hallelujah.mp4
