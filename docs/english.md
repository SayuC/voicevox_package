### VOICEVOX_CORE

install (aarch64):
```sh
 pip install https://github.com/AkariOficial/voicevox_package/releases/download/voicevox_core-0.14.1/voicevox_core-0.14.1+cpu.tar.gz
```

Install the voicevox_core package:
```sh
  wget https://github.com/VOICEVOX/voicevox_core/releases/download/0.14.1/download-linux-arm64
  chmod +x download-linux-arm64 && ./download-linux-arm64
```
> Go into the generated folder "voicevox_core" and add dependencie libonnxruntime.so.1.13.1 copy to the voicevox project

Usage：
```python
from pathlib import Path
from voicevox_core import synthetize

audio = synthetize.synthesize_audio(
    36,
    "おはよう",
    Path("./open_jtalk_dic_utf_8-1.11"))

with open("audio.ogg", "wb") as f:
        f.write(audio)
```

or on the command line:
```sh
 python ./run.py ./open_jtalk_dic_utf_8-1.11 これはテストです ./audio.ogg
```
