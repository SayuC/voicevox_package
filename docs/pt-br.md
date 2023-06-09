### VOICEVOX_CORE

instale o pacote pip aarch64:
```sh
 pip install https://github.com/AkariOficial/voicevox_package/releases/download/voicevox_core-0.14.1/voicevox_core-0.14.1+cpu.tar.gz
```

Instale o open-jtalk:
```sh
  wget https://sourceforge.net/projects/open-jtalk/files/Dictionary/open_jtalk_dic-1.11/open_jtalk_dic_utf_8-1.11.tar.gz
  tar -xzf open_jtalk_dic_utf_8-1.11.tar.gz
```

Instale o pacote voicevox_core:
```sh
  wget https://github.com/VOICEVOX/voicevox_core/releases/download/0.14.1/download-linux-arm64
  chmod +x download-linux-arm64 && ./download-linux-arm64
```
> Entre na pasta gerada "voicevox_core" e copie a dependência **libonnxruntime.so.1.13.1** para o seu projeto voicevox.

Uso：
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

Ou na linha de comando:
```sh
 python ./run.py ./open_jtalk_dic_utf_8-1.11 これはテストです ./audio.ogg
```
