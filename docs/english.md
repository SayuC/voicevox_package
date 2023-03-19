### VOICEVOX_CORE

Install package pip aarch64:
```sh
 pip install https://github.com/AkariOficial/voicevox_package/releases/download/voicevox_core-0.14.1/voicevox_core-0.14.1+cpu.tar.gz
```

Install open-jtalk:
```sh
  wget https://sourceforge.net/projects/open-jtalk/files/Dictionary/open_jtalk_dic-1.11/open_jtalk_dic_utf_8-1.11.tar.gz
  tar -xzf open_jtalk_dic_utf_8-1.11.tar.gz
```

Install the voicevox_core package:
```sh
  wget https://github.com/VOICEVOX/voicevox_core/releases/download/0.14.1/download-linux-arm64
  chmod +x download-linux-arm64 && ./download-linux-arm64
```
> Go into the generated folder "voicevox_core" and copy the dependencie **libonnxruntime.so.1.13.1** to the your voicevox project

Usage：
```python
from pathlib import Path
from voicevox_core import synthetize

audio = synthetize.synthesize_audio(
    SPEAKER_ID=36,
    text="おはよう",
    open_jtalk_dict_dir=Path("./open_jtalk_dic_utf_8-1.11")
)

with open("audio.ogg", "wb") as f:
    f.write(audio)
```

Or on the cmd (command line):
```sh
 python ./run.py ./open_jtalk_dic_utf_8-1.11 これはテストです ./audio.ogg
```
