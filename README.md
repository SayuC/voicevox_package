### VOICEVOX_CORE
> 元の公式レポ [voicevox_core](https://github.com/Hiroshiba/voicevox_core)
[![dependency status](https://deps.rs/repo/github/VOICEVOX/voicevox_core/status.svg)](https://deps.rs/repo/github/VOICEVOX/voicevox_core)
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
> 声の種類を変更したい場合は [ここ](https://github.com/AkariOficial/voicevox_package/blob/main/docs/types_voice/%E6%97%A5%E6%9C%AC.md#%E3%81%93%E3%81%93%E3%81%A7%E3%81%AF%E4%BD%BF%E7%94%A8%E5%8F%AF%E8%83%BD%E3%81%AA%E3%83%9C%E3%82%A4%E3%82%B9%E3%81%AE%E3%82%BF%E3%82%A4%E3%83%97%E3%82%92%E8%A6%8B%E3%81%A4%E3%81%91%E3%82%8B%E3%81%93%E3%81%A8%E3%81%8C%E3%81%A7%E3%81%8D%E3%81%BE%E3%81%99) の[português]()                  
