# Creating and Inputing a subtitle for Youtube video
### Overview
This Jupyter Notebook provides a comprehensive workflow for downloading a YouTube video, extracting its audio, transcribing and translating the audio into subtitles, overlaying these subtitles onto the original video, and finally uploading the subtitled video for public access and display.

### Features
- **YouTube Video Download:** Downloads a specified YouTube video.
- **Audio Extraction:** Extracts the audio track from the downloaded video.
- **Transcription and Translation:** Utilizes the Whisper model to transcribe the audio and translate it into German.
- **Subtitle Generation:** Generates SRT subtitles from the transcribed text.
- **Subtitle Overlay:** Adds the generated subtitles onto the original video.
- **Video Upload:** Uploads the final video with subtitles to a public server.
- **Video Display:** Displays the uploaded video within the notebook.

### Dependencies
- `pytube`: For downloading videos from YouTube.
- `whisper`: For audio transcription and translation.
- `srt`: For handling SRT subtitle files.
- `datetime`: For managing time-related data in subtitles.
- `moviepy`: For video editing tasks, including audio extraction and subtitle overlay.
- `kora`: Specifically kora.drive, for uploading the final video to a public server.
- `IPython.display`: For displaying the final video within the notebook.
  
### Usage Instructions
- **Set the YouTube URL**: Change the url variable to the link of the YouTube video you want to download.
- **Execute the Notebook**: Run each cell in the notebook sequentially. It will perform all operations from downloading the video to displaying the final video with subtitles.
- **View the Result**: The final video with subtitles will be displayed within the notebook.
  
### Customization Options
- **Subtitle Language**: The language for translation (set to German "de" in this notebook) can be changed according to your needs.
- **Subtitle Appearance**: Modify the create_subtitle_clip function to alter the appearance of subtitles.
- **Video Quality**: Adjust the filter parameters in the pytube query to download different video formats or qualities.
  
### Important Notes
- Ensure all dependencies are installed in your Jupyter environment before running the notebook.
- The notebook currently uploads the video to a public server using kora.drive. Make sure you have the necessary permissions and configurations for public file sharing.
