# 🎵 VR Empréstimo Modal

Experiência web imersiva em **A-Frame** para estudo de acordes no contexto de empréstimo modal, com navegação em primeira pessoa, áudio interativo e acompanhamento de progresso.

## ✨ Funcionalidades

- Ambiente 3D com tema de floresta (`aframe-environment-component`)
- Interação com acordes clicáveis em sequência
- Reprodução de acordes via Web Audio API
- Som ambiente + efeito sonoro do pato
- Controle por teclado/mouse e joysticks virtuais (mobile)
- HUD com progresso dos acordes restantes
- Modo mapa, zoom e alternância dia/noite

## 🚀 Como executar

Este projeto é estático (apenas `index.html`), sem etapa de build.

1. Clone o repositório.
2. Abra o arquivo `index.html` no navegador **ou** rode um servidor local simples.

Exemplo com Python:

```bash
python3 -m http.server 8000
```

Depois acesse: `http://localhost:8000`

## 🎮 Controles

### Desktop

- **W/A/S/D**: movimentação
- **Mouse**: olhar ao redor
- **Espaço**: pular
- **Clique**: interagir com acordes/objetos

### Mobile

- **Joystick esquerdo**: movimentação
- **Joystick direito**: rotação da câmera
- Toque na tela para interações

### Botões de interface

- **🔊 Ambiente**: liga/desliga o som ambiente
- **🌙 Noite / ☀️ Dia**: alterna visual da cena
- **🗺️ Visão Mapa / 🚶 Visão Imersiva**: alterna perspectiva
- **➕ / ➖**: zoom da câmera

## 🧩 Tecnologias

- [A-Frame](https://aframe.io/)
- [aframe-environment-component](https://github.com/supermedium/aframe-environment-component)
- [aframe-extras](https://github.com/c-frame/aframe-extras)
- [nipplejs](https://yoannmoi.net/nipplejs/)

## 📁 Estrutura atual

- `index.html`: aplicação principal (HTML, CSS e JavaScript)
- `audiopapkin-forest-ambience-296528.mp3`: áudio ambiente
- `pato.mp3`: efeito sonoro do pato
