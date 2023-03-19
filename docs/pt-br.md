### VOICEVOX_CORE

instale (aarch64):
```sh
 pip install https://github.com/AkariOficial/voicevox_package/releases/download/voicevox_core-0.14.1/voicevox_core-0.14.1+cpu.tar.gz
```

Instale o pacote voicevox_core:
```sh
  wget https://github.com/VOICEVOX/voicevox_core/releases/download/0.14.1/download-linux-arm64
  chmod +x download-linux-arm64 && ./download-linux-arm64
```
> Entre na pasta gerada "voicevox_core" e copie a dependência **libonnxruntime.so.1.13.1** para o seu projeto voicevox

Uso：
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

ou na linha de comando:
```sh
 python ./run.py ./open_jtalk_dic_utf_8-1.11 これはテストです ./audio.ogg
```
