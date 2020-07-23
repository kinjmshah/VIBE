# Changes needed to implement on Windows 10

- Install ffmpeg if not already installed 
- `demo.py`: Update `egl` to `EGL` in `os.environ['PYOPENGL_PLATFORM']='egl'`
- `demo_utils.py`: 
	- function `video_to_images`: change `/tmp'` to `\\tmp` (~ line 185)
	- In `command` definition: change `f'{img_folder}/%06d.png'` to `f'{img_folder}\\%06d.png'` (~ line 195)
