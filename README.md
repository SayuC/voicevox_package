### VOICEVOX_CORE
> 元の公式レポ [voicevox_core](https://github.com/Hiroshiba/voicevox_core)
</br>

[日本](https://github.com/AkariOficial/voicevox_package/blob/main/docs/日本.md)語のドキュメントを読むか、[english](https://github.com/AkariOficial/voicevox_package/blob/main/docs/english.md) または [português](https://github.com/AkariOficial/voicevox_package/blob/main/docs/pt-br.md)

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

with open("audio.ogg", "wb") as f:
        f.write(audio)

```

またはコマンドラインで：
```sh
 python ./run.py ./open_jtalk_dic_utf_8-1.11 これはテストです ./audio.ogg
```
