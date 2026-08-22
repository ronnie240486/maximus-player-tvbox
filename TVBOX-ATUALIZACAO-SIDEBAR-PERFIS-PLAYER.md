# Atualização TV Box — sidebar, perfis e player

Esta branch é derivada da versão TV Box congelada e não altera a versão mobile.

## Alterações

- O botão **Câmeras** foi removido do sidebar da Home.
- A Home adia validações de rede, lembretes e carregamentos pesados até depois da primeira interação do controle remoto, deixando o sidebar disponível imediatamente.
- O fundo `bg_url` salvo localmente é carregado em paralelo ao MAC e aparece também durante a tela inicial de verificação.
- O foco visual dos perfis é desenhado como uma sobreposição limitada ao avatar; o nome e o espaço externo não recebem borda.
- O gerenciamento de perfis e a grade de avatares usam alvos pequenos e diretos para o D-pad.
- O mini player e o player grande continuam usando a mesma sessão compartilhada e a mesma `VideoView`; a expansão apenas altera o modo/layout da sessão.

## Arquivos de player preservados

Os arquivos abaixo não foram alterados nesta atualização:

- `app/player.tsx`
- `app/channels.tsx`
- `app/channel-details.tsx`
- `src/components/TVChannelPreview.tsx`
- `src/state/player-session.tsx`

A New Architecture e o Hermes continuam ativos. O filtro de conteúdo adulto e o branding existente também permanecem na fonte.
