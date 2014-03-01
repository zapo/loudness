#neg23
Python script to automate loudness normalization (to -23 LUFS) using FFmpeg and sox. Run the program with a single argument (your audio file) and it will be passed to FFmpeg for EBU R128 analysis and then to sox for gain adjustment. A new file with "_neg23" appended to the filename will be created and placed in the same directory as the input file. Correct usage: 
```bash
$ neg23 somefile.wav
```

If you want to be able to run neg.py from the terminal by just typing 'neg23', first make the script executable and then copy it to /usr/bin. Like this:
```bash
$ chmod +x neg23.py
$ cp neg23.py /usr/bin/neg23
```

You should have both FFmpeg and sox installed on your machine.
```bash
$ brew install ffmpeg
$ brew install sox
```
