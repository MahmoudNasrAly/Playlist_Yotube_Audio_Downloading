# Playlist_Yotube_Audio_Downloading

Key features of this project:

Uses yt-dlp for robust playlist downloading
Converts downloaded files to high-quality MP3
Allows custom download directory
Simple, interactive command-line interface
Handles errors gracefully

Installation requirements:
```bash
pip install yt-dlp
pip install ffmpeg-python
```
 Ensure FFmpeg is installed on your system for audio conversion.
To use:

Install required libraries
Run the script
Paste playlist URL when prompted
Choose download directory (optional)

The script will download all audio tracks from the playlist as MP3 files.

You need to install FFmpeg. Here's how to install it on different operating systems:
Windows:
Download from official FFmpeg site
Add to system PATH
Or use: winget install ffmpeg

## macOS:
```
brew install ffmpeg
```
## Linux (Ubuntu/Debian):
```
sudo apt update
sudo apt install ffmpeg
```
## Linux (Fedora):
```
sudo dnf install ffmpeg
```
After installation, the script should work. If not, you can specify FFmpeg path:
```
ydl_opts = {
    'ffmpeg_location': '/path/to/ffmpeg',
    # ... other options remain the same
}
```

Troubleshooting tips:

Verify FFmpeg installation with ffmpeg -version
Ensure YouTube playlist URL is correct

## if you still have a problem  on Windows:

Download FFmpeg:

Go to https://github.com/BtbN/FFmpeg-Builds/releases
Download the Windows build (usually ffmpeg-master-latest-win64-gpl.zip)
```
# Unzip the downloaded file
# Create a folder like C:\ffmpeg
# Extract contents there

# Add to PATH (replace with your actual path)
$env:Path += ";C:\ffmpeg\bin"

# To make it permanent, use System Environment Variables:
# Open Control Panel > System > Advanced System Settings 
# Click "Environment Variables"
# Under "System variables", edit "Path"
# Add the full path to FFmpeg's bin folder
```
## Verify installation: 
```
ffmpeg -version
```
