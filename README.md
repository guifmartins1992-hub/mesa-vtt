# Mesa VTT

Protótipo inicial de mesa virtual de RPG.

## Publicação
O workflow em `.github/workflows/pages.yml` publica automaticamente a raiz do repositório na branch `main` pelo GitHub Pages. Em Settings → Pages, selecione GitHub Actions como origem, caso ainda não esteja selecionada.

## Recursos presentes nesta versão
- Área principal para compartilhamento de tela local.
- Janela de câmera flutuante, arrastável e redimensionável.
- Acesso local à câmera e microfone, seletor de entrada e medidor de atividade.
- Avatar selecionado de arquivo local.
- Controles visuais de fundo verde e imagem.
- Chat local e rolagem com grupos, modificadores, operações e vantagem/desvantagem.
- Ficha com 3 recursos, 10 contadores independentes de 10 marcações, sucessos, falhas e anotações salvas no navegador.

## Limitações
Esta versão é somente um protótipo local. Não tem salas multiplayer, login, sincronização, chat remoto, transmissão de áudio/vídeo entre participantes, permissões de mestre ou fichas privadas na nuvem. O compartilhamento de tela só aparece neste navegador. A seleção de imagem/fundo verde ainda não remove o fundo nem segmenta automaticamente a pessoa.
Para multiplayer será necessário configurar backend e serviço de mídia em tempo real (por exemplo Supabase e LiveKit).
