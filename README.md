# Aula XR — Empréstimo Modal

Experiência musical interativa em 3D para estudar **empréstimo modal**. O app apresenta uma sequência de acordes em um ambiente criado com A-Frame, reproduz os acordes pelo navegador e conduz a atividade com falas em áudio.

## Acessar o app

O projeto está publicado no GitHub Pages:

**[Abrir Aula XR — Empréstimo Modal](https://glauberlasantiago.github.io/vr-emprestimo-modal/)**

## Recursos

- ambiente musical 3D responsivo;
- sequência interativa de acordes;
- síntese dos acordes com Web Audio API;
- falas explicativas em MP3 para cada etapa;
- movimentação por dois joysticks virtuais no celular;
- alternância entre visão em primeira pessoa e visão de mapa;
- controles de zoom, ambiente sonoro e modo dia/noite;
- indicador de progresso compacto em telas móveis;
- autenticação com Google e salvamento do progresso no Firebase.

## Como usar

1. Abra o app e aguarde o carregamento da cena.
2. No celular, use o joystick esquerdo para se movimentar e o direito para controlar a visão.
3. Interaja com o acorde destacado para ouvi-lo e avançar na aula.
4. Acompanhe o acorde atual e a quantidade restante no painel de progresso.
5. Use **Visão Mapa** e os botões **+** e **−** para observar a cena de cima.
6. Entre com uma conta Google se quiser salvar e restaurar seu progresso.

## Executar localmente

Como o navegador restringe alguns recursos de áudio e módulos quando um HTML é aberto diretamente, sirva a pasta com um servidor HTTP local.

Com Node.js:

```bash
npx serve .
```

Ou com Python:

```bash
python -m http.server 8000
```

Depois, abra o endereço exibido no terminal, normalmente `http://localhost:3000` ou `http://localhost:8000`.

## Estrutura do projeto

```text
.
├── index.html       # Interface, cena 3D, estilos e lógica do app
├── audio/           # Falas da aula organizadas por acorde e frase
├── firebase.json    # Configuração do Firebase Hosting
└── .firebaserc      # Projeto Firebase associado
```

Os arquivos de fala seguem o padrão:

```text
audio/chord_<acorde>_phrase_<frase>.mp3
```

## Tecnologias

- HTML, CSS e JavaScript;
- [A-Frame](https://aframe.io/);
- Web Audio API;
- NippleJS;
- Firebase Authentication e Firestore;
- GitHub Pages.

## Publicação

O GitHub Pages publica diretamente a branch `main`. Alterações enviadas para essa branch podem levar alguns instantes para aparecer no endereço público.

O projeto também contém configuração para publicação com Firebase Hosting.

## Autor

Desenvolvido por **Glauber L. A. Santiago**.
