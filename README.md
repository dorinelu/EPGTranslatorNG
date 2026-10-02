# EPG Translator NG

**EPG Translator NG** is an Enigma2 plugin for translating EPG event information directly on the receiver.

Current version: **1.0-r5.2**

Created by **Dorinelu** with AI assistance by ChatGPT  
**DG Labs — Plugins • Tools • Solutions**

## Features

- MyMemory, Google Cloud Translation and DeepL API providers
- Automatic EventView translation
- Translated EPG list titles
- Configurable 24h / 48h EPG translation horizon
- Translated InfoBar **Now / Next** using the shared EPG cache
- Persistent translation cache
- Automatic source-language detection
- Provider status display, e.g. `Translated DE -> RO via DeepL`
- Multilingual Enigma2 interface using gettext

## Interface languages

English, German, Romanian, Italian, Spanish, French, Dutch, Polish, Portuguese, Turkish, Russian and Arabic.

The plugin follows the Enigma2 system language and falls back to English.

## Translation providers

### MyMemory
Works without an API key.

### DeepL
Supports DeepL API Free and paid API accounts. Configure your own API key in the plugin setup.

### Google Cloud Translation
Supports Google Cloud Translation API with your own API key.

> Never publish API keys in this repository or in screenshots/logs.

## Installation

Copy the IPK package to the receiver and install it with:

```sh
opkg install --force-overwrite /tmp/enigma2-plugin-extensions-epgtranslatorng_*.ipk
init 4
sleep 2
init 3
```

## Configuration

Runtime configuration is stored on the receiver in:

```
/etc/enigma2/epgtranslatorng.conf
```

API keys are intentionally not included in the source repository.

## Notes

Developed and tested primarily on modern Python 3 Enigma2 images. Compatibility can vary by image/skin and should be reported through GitHub Issues.
