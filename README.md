# Lyric Finder 🎵

Reconoce canciones que suenan en tu computadora y muestra la letra automáticamente.

## Requisitos

- Linux con PulseAudio o PipeWire
- [songrec](https://github.com/kenvix2213/songrec) (Shazam client)
- [glyrics](https://www.npmjs.com/package/glyrics) (buscador de letras)
- Node.js/npm

## Instalación rápida

```bash
# Instalar dependencias
sudo apt install songrec
npm install -g glyrics

# Clonar e instalar
git clone https://github.com/TU_USUARIO/lyric-finder.git
cd lyric-finder
chmod +x lyric-finder.sh

# Copiar a una ubicación en tu PATH
sudo cp lyric-finder.sh /usr/local/bin/lyric-finder
```

## Uso

```bash
# Ejecutar
lyric-finder

# O crear un alias en ~/.bashrc
alias lyrics='lyric-finder'
```

## Cómo funciona

1. Detecta automáticamente el monitor de audio de tu sistema
2. Usa Shazam (via songrec) para reconocer la canción que está sonando
3. Busca la letra con glyrics y la muestra en terminal

## Licencia

MIT
