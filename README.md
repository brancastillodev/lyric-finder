# Canta 🎵

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
git clone https://github.com/brancastillodev/lyric-finder.git
cd lyric-finder
chmod +x canta.sh

# Copiar a una ubicación en tu PATH
sudo cp canta.sh /usr/local/bin/canta
```

## Uso

```bash
# Ejecutar
canta

# O crear un alias en ~/.bashrc
alias canta='canta'
```

## Cómo funciona

1. Detecta automáticamente el monitor de audio de tu sistema
2. Usa Shazam (via songrec) para reconocer la canción que está sonando
3. Busca la letra con glyrics y la muestra en terminal

## Licencia

MIT
