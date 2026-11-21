# Mesa VTT — protótipo V4

Esta publicação usa como base o arquivo V4 enviado pelo proprietário do projeto.

## Abrir
Depois que o GitHub Pages concluir a publicação:
https://guifmartins1992-hub.github.io/mesa-vtt/

## Recursos presentes no protótipo V4
- Interface de mesa virtual com área principal e painel lateral.
- Câmera e microfone locais, com seleção de dispositivos.
- Janela de câmera flutuante, redimensionável e controles de janela.
- Escolha de avatar por imagem local.
- Opções de fundo verde e imagem de fundo; o código carrega MediaPipe Selfie Segmentation para o processamento de fundo.
- Chat local e janela separada de chat.
- Rolagem de dados com grupos, modificadores, operações e vantagem/desvantagem.
- Ficha local com recursos, contadores, sucessos, falhas e anotações.
- Persistência local no navegador.

## Limites importantes
Esta versão ainda é um protótipo de navegador. O armazenamento e a comunicação entre janelas usam recursos locais do navegador; isso não cria uma sala multiplayer entre computadores diferentes.

Ainda não estão configurados:
- cadastro/login e salas privadas acessíveis pela internet;
- sincronização em tempo real de chat, fichas, dados e estado da sala entre jogadores;
- transmissão de câmera e microfone entre participantes;
- compartilhamento de tela remoto com permissão validada no servidor;
- armazenamento em nuvem de avatares e fichas.

Para habilitar esses recursos, falta conectar um backend (por exemplo Supabase) e um servidor de mídia em tempo real (por exemplo LiveKit), além das respectivas credenciais e configuração de implantação.

## Publicação
O workflow em `.github/workflows/pages.yml` publica a raiz do repositório na branch `main` usando GitHub Pages. Em **Settings → Pages**, a origem deve estar como **GitHub Actions**.

## Arquivos
- `index.html`: carregador da aplicação publicada.
- `mesa-vtt-v4.html.gz.b64`: pacote comprimido do HTML V4 original.
- `.github/workflows/pages.yml`: publicação automática pelo GitHub Actions.
