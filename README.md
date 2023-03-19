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

### 音声データベースのドキュメントはこちら
> 声の種類を変更したい場合は [ここ](https://github.com/AkariOficial/voicevox_package/blob/main/docs/types_voice/pt-br.md#aqui-voc%C3%AA-encontra-os-tipos-de-vozes-dispon%C3%ADveis)
