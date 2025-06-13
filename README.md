# mov2gif
A Simple .mov to .gif converter for macOS

## Installation

### 1. First, install FFmpeg if you don't have it:

```
brew install ffmpeg
```

### 2. Download and move the file mov2gif from this repo to your /usr/local/bin directory:

```
git clone https://github.com/shadabshaukat/mov2gif.git
cd mov2gif/
sudo mv mov2gif /usr/local/bin
```

### 3. Make the mov2gif script executable
```
sudo chmod +x /usr/local/bin/mov2gif
```

## Usage Examples

### Basic conversion:
```
mov2gif input.mov
```

### 2x Speed conversion:
```
mov2gif -x 2.0 input.mov
```

### Custom Width and FPS :
```
mov2gif -s 320 -f 10 input.mov
```

### High Quality Output :
```
mov2gif -q high input.mov
```

### Custom Filename Output :
```
mov2gif -x 2.0 -f 30 -q high -o custom_name.gif input.mov
```

### Show help:
```
mov2gif -h
```

## Features

    Speed control with -x option (2.0 for 2x speed)

    Quality presets (low, medium, high)

    Custom output filename

    Adjustable dimensions and frame rate

    Colorful terminal output

    Progress feedback

    Detailed help message

The script uses FFmpeg's palette generation for high-quality GIFs while keeping the file size reasonable. The speed adjustment is done by modifying the presentation timestamps (PTS) of the video frames.






