### VOICEVOX_CORE

インストール(aarch64):
```sh
 pip install https://github.com/AkariOficial/voicevox_package/releases/download/voicevox_core-0.14.1/voicevox_core-0.14.1+cpu.tar.gz
```

使い方：
```python
from pathlib import Path
from voicevox_core import synthetize

audio = synthetize.synthesize_audio(
    36,
    "おはよう",
    Path("./open_jtalk_dic_utf_8-1.11"))
```

またはコマンドラインで：
```sh
 python ./run.py ./open_jtalk_dic_utf_8-1.11 これはテストです ./audio.ogg
```
