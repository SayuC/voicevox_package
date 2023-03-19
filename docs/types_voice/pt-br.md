### Aqui você encontra os tipos de vozes disponíveis.

```python
from voicevox_core import synthetize
from pathlib import Path

audio = synthetize.synthesize_audio(
    SPEAKER_ID=36,
    text="おはよう",
    open_jtalk_dict_dir=Path("./open_jtalk_dic_utf_8-1.11")
)

with open("audio.ogg", "wb") as f:
    f.write(audio)
```

O parâmetro "id" abaixo pode ser especificado acima usando um número que se refere ao ID de cada voz. SPEAKER_ID permite passar um número inteiro.

```json
 [
  {
    "name": "四国めたん / Shikoku Metan",
    "styles": [
      {
        "name": "normal",
        "id": 2
      },
      {
        "name": "doce",
        "id": 0
      },
      {
        "name": "Tsun-Tsun",
        "id": 6
      },
      {
        "name": "sexy",
        "id": 4
      },
      {
        "name": "Sussurrar",
        "id": 36
      },
      {
        "name": "sussurrando",
        "id": 37
      }
    ],
    "speaker_uuid": "7ffcb7ce-00ec-4bdc-82cd-45a8889e43ff",
    "version": "0.14.1"
  },
  {
    "name": "ずんだもん　/ Zundamon",
    "styles": [
      {
        "name": "normal",
        "id": 3
      },
      {
        "name": "doce",
        "id": 1
      },
      {
        "name": "Tsun Tsun",
        "id": 7
      },
      {
        "name": "sexy",
        "id": 5
      },
      {
        "name": "Sussurrar",
        "id": 22
      },
      {
        "name": "sussurrando",
        "id": 38
      }
    ],
    "speaker_uuid": "388f246b-8c41-4ac1-8e2d-5d79f3ff56d9",
    "version": "0.14.1"
  },
  {
    "name": "春日部つむぎ　/ Tsumugi Kasukabe",
    "styles": [
      {
        "name": "normal",
        "id": 8
      }
    ],
    "speaker_uuid": "35b2c544-660e-401e-b503-0e14c635303a",
    "version": "0.14.1"
  },
  {
    "name": "雨晴はう　/ Amabarashi",
    "styles": [
      {
        "name": "normal",
        "id": 10
      }
    ],
    "speaker_uuid": "3474ee95-c274-47f9-aa1a-8322163d96f1",
    "version": "0.14.1"
  },
  {
    "name": "波音リツ　/ Namion Ritsu",
    "styles": [
      {
        "name": "normal",
        "id": 9
      }
    ],
    "speaker_uuid": "b1a81618-b27b-40d2-b0ea-27a9ad408c4b",
    "version": "0.14.1"
  },
  {
    "name": "玄野武宏　/ Takehiro Kurono",
    "styles": [
      {
        "name": "normal",
        "id": 11
      },
      {
        "name": "alegria",
        "id": 39
      },
      {
        "name": "desleixado",
        "id": 40
      },
      {
        "name": "tristeza",
        "id": 41
      }
    ],
    "speaker_uuid": "c30dc15a-0992-4f8d-8bb8-ad3b314e6a6f",
    "version": "0.14.1"
  },
  {
    "name": "白上虎太郎　/ Torataro Shirakami",
    "styles": [
      {
        "name": "ordinário",
        "id": 12
      },
      {
        "name": "yay!",
        "id": 32
      },
      {
        "name": "nervoso",
        "id": 33
      },
      {
        "name": "oko",
        "id": 34
      },
      {
        "name": "bem",
        "id": 35
      }
    ],
    "speaker_uuid": "e5020595-5c5d-4e87-b849-270a518d0dcf",
    "version": "0.14.1"
  },
  {
    "name": "青山龍星　/ Ryuusei Aoyama",
    "styles": [
      {
        "name": "normal",
        "id": 13
      }
    ],
    "speaker_uuid": "4f51116a-d9ee-4516-925d-21f183e2afad",
    "version": "0.14.1"
  },
  {
    "name": "冥鳴ひまり　/ Himari",
    "styles": [
      {
        "name": "normal",
        "id": 14
      }
    ],
    "speaker_uuid": "8eaad775-3119-417e-8cf4-2a10bfd592c8",
    "version": "0.14.1"
  },
  {
    "name": "九州そら　/ Kyūshū sora",
    "styles": [
      {
        "name": "normal",
        "id": 16
      },
      {
        "name": "doce",
        "id": 15
      },
      {
        "name": "Tsun Tsun",
        "id": 18
      },
      {
        "name": "sexy",
        "id": 17
      },
      {
        "name": "Sussurrar",
        "id": 19
      }
    ],
    "speaker_uuid": "481fb609-6446-4870-9f46-90c4dd623403",
    "version": "0.14.1"
  },
  {
    "name": "もち子さん / Mochiko",
    "styles": [
      {
        "name": "normal",
        "id": 20
      }
    ],
    "speaker_uuid": "9f3ee141-26ad-437e-97bd-d22298d02ad2",
    "version": "0.14.1"
  },
  {
    "name": "剣崎雌雄　/ Kenzaki shiyū",
    "styles": [
      {
        "name": "normal",
        "id": 21
      }
    ],
    "speaker_uuid": "1a17ca16-7ee5-4ea5-b191-2f02ace24d21",
    "version": "0.14.1"
  },
  {
    "name": "WhiteCUL",
    "styles": [
      {
        "name": "normal",
        "id": 23
      },
      {
        "name": "diversão",
        "id": 24
      },
      {
        "name": "Triste",
        "id": 25
      },
      {
        "name": "bem",
        "id": 26
      }
    ],
    "speaker_uuid": "67d5d8da-acd7-4207-bb10-b5542d3a663b",
    "version": "0.14.1"
  },
  {
    "name": "後鬼　/ Kōki",
    "styles": [
      {
        "name": "versão humano.",
        "id": 27
      },
      {
        "name": "versão de pelúcia.",
        "id": 28
      }
    ],
    "speaker_uuid": "0f56c2f2-644c-49c9-8989-94e11f7129d0",
    "version": "0.14.1"
  },
  {
    "name": "No.7",
    "styles": [
      {
        "name": "normal",
        "id": 29
      },
      {
        "name": "anúncio",
        "id": 30
      },
      {
        "name": "Leitura",
        "id": 31
      }
    ],
    "speaker_uuid": "044830d2-f23b-44d6-ac0d-b5d733caa900",
    "version": "0.14.1"
  },
  {
    "name": "ちび式じい / Chibi-shiki",
    "styles": [
      {
        "name": "normal",
        "id": 42
      }
    ],
    "speaker_uuid": "468b8e94-9da4-4f7a-8715-a22a48844f9e",
    "version": "0.14.1"
  },
  {
    "name": "櫻歌ミコ　/ Sakuraka Miko",
    "styles": [
      {
        "name": "normal",
        "id": 43
      },
      {
        "name": "segunda forma",
        "id": 44
      },
      {
        "name": "loli",
        "id": 45
      }
    ],
    "speaker_uuid": "0693554c-338e-4790-8982-b9c6d476dc69",
    "version": "0.14.1"
  },
  {
    "name": "Saya/SAYO",
    "styles": [
      {
        "name": "normal",
        "id": 46
      }
    ],
    "speaker_uuid": "a8cc6d22-aad0-4ab8-bf1e-2f843924164a",
    "version": "0.14.1"
  },
  {
    "name": "ナースロボ＿タイプＴ　/　Nāsurobo",
    "styles": [
      {
        "name": "normal",
        "id": 47
      },
      {
        "name": "facilmente",
        "id": 48
      },
      {
        "name": "Temer",
        "id": 49
      },
      {
        "name": "segredo",
        "id": 50
      }
    ],
    "speaker_uuid": "882a636f-3bac-431a-966d-c5e6bba9f949",
    "version": "0.14.1"
  }
]
```
