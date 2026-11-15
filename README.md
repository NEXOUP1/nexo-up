# Site NEXO UP: arquivos e publicação

## Arquivos

Envie todos estes arquivos juntos, na mesma pasta do `index.html`, sem renomear nada:

- `index.html`: o site completo, em um único arquivo.
- `favicon-16x16.png`, `favicon-32x32.png`, `favicon.webp`: ícones da aba do navegador.
- `apple-touch-icon.png`: ícone para a tela inicial do iPhone.
- `android-chrome-192x192.png`, `android-chrome-512x512.png`: ícones para Android.
- `site.webmanifest`: nome e ícones do site para celular.
- `video-barbearia.mp4`, `video-salao.mp4`: vídeos de exemplo do portfólio.
- `calendario-mensal.jpg`: calendário de exemplo (fictício) do portfólio.
- `README.md`: este guia (não é necessário para o site funcionar).

## Configuração (um único lugar)

No fim do `index.html`, localize o bloco `CONFIG`:

```js
var CONFIG = {
  whatsappNumber: "5551998424483",   // só dígitos, com DDI 55 e DDD
  whatsappDisplay: "+55 51 99842-4483",
  instagramUrl: "https://www.instagram.com/nexoup26/"
};
```

- Para trocar o WhatsApp, altere `whatsappNumber` e `whatsappDisplay`. Todos os botões são atualizados sozinhos.
- Para trocar o Instagram, altere `instagramUrl`. Se deixar vazio, o item some da página.

## Como testar antes de publicar

1. Abra o `index.html` no navegador com dois cliques.
2. No computador, reduza a janela até uns 400 px de largura. Nada pode sair da tela nem criar rolagem lateral.
3. No celular, confira:
   - os cards de serviços, condições e planos ficam em uma coluna;
   - os vídeos do portfólio tocam;
   - o botão "Falar no WhatsApp" abre a conversa com a mensagem pronta.
4. Toque em cada botão do WhatsApp e confira se a mensagem está certa.
5. Toque em cada pergunta frequente e confira se ela abre e fecha.

## Como publicar no GitHub Pages

1. Crie um repositório público no GitHub, por exemplo `nexo-up`.
2. Clique em **uploading an existing file** e envie todos os arquivos da lista acima.
3. Clique em **Commit changes**.
4. Vá em **Settings > Pages**. Em **Source**, escolha **Deploy from a branch**, depois **main** e **/ (root)**. Clique em **Save**.
5. Espere 1 a 2 minutos. O endereço aparece nessa mesma tela.

Para editar depois, abra o `index.html` no GitHub, clique no lápis e depois em **Commit changes**.

## O que ainda precisa ser definido

Este é o único ponto pendente marcado no site:

1. **Dias e horários de atendimento** (seção de contato).

Pontos para revisar antes de publicar:

- Os vídeos de exemplo vieram de contas de terceiros, com nomes de criadores no arquivo. Confirme que você tem permissão para usá-los, ou troque por conteúdos próprios.
- A FAQ diz que os conteúdos são excluídos quando o pagamento atrasa, mas o bloco de condições comerciais fala em suspensão temporária. Escolha uma das duas regras e ajuste o texto nos dois lugares.

## Observações técnicas

- O site usa as fontes Inter e Space Grotesk, do Google Fonts. Sem internet, o texto aparece em fonte do sistema.
- Não há cookies, rastreadores nem formulários. O contato é feito somente pelo WhatsApp.
- Para trocar um exemplo do portfólio, substitua o arquivo de vídeo ou imagem mantendo o mesmo nome. Se usar outro nome, altere também o `src` no `index.html`.
