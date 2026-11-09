# Rádio Esperança 101.1FM — PWA para GitHub Pages

Personalização do aplicativo de rádio Nativa FM **V1.9.4**, usando o projeto anteriormente validado. O pacote contém somente os arquivos do site e este guia (opcional na publicação).

## Personalização desta emissora

- Nome: **Rádio Esperança 101.1FM**
- Slogan: **A voz da fé, a sintonia da esperança!**
- Frequência / rótulo: **101.1 FM**
- Streaming: `https://stream.zeno.fm/cm199aqfxsptv`
- Identificador Zeno: `cm199aqfxsptv`
- Metadados em tempo real: `https://api.zeno.fm/mounts/metadata/subscribe/cm199aqfxsptv`
- Tema: **Laranja Neon #FF963E**. O VU-meter circular continua usando suas cores originais multicoloridas, com análise real de áudio quando CORS permite.
- Logotipo: imagem original fornecida pelo responsável, aplicada à tela e aos ícones de instalação.
- **Sem nenhum botão de contato/WhatsApp.** Nenhum número de telefone foi incluído no código.
- Botão **COMPARTILHAR** preservado ao lado do botão ligar/desligar; prepara convite para instalar a rádio por meio do WhatsApp, sem contato ou telefone de destino fixo.

## Compartilhamento automático

O link compartilhado vem automaticamente da localização HTTPS do aplicativo publicado no GitHub Pages. Por exemplo, se instalar de `https://usuario.github.io/radio-esperanca/`, esse será o endereço do convite.

Para compartilhar um domínio próprio em vez do endereço publicado, edite apenas `config.js`:

```js
shareInstallUrl: 'https://radio.exemplo.com.br/'
```

Mantenha o valor vazio `''` para detectar o endereço automaticamente.

## Publicar no GitHub Pages

1. Crie um repositório, como `radio-esperanca`.
2. Envie **o conteúdo de dentro do ZIP diretamente para a raiz** do repositório (o `index.html` deve ficar na raiz).
3. Em **Settings → Pages**, escolha **Deploy from a branch**, a branch `main` e a pasta `/(root)`.
4. Acesse a URL HTTPS gerada. Pela página pública, utilize o botão de instalação ou as opções do navegador. Abra a PWA pelo ícone instalado para mostrar a tela do rádio.
5. Teste a transmissão, a troca de metadados, o equalizador, o controle liga/desliga e o compartilhamento no aparelho real.

## Funcionalidades preservadas da V1.9.4

Reprodução automática ao abrir a PWA instalada (sujeita às permissões do navegador), reconexão automática, metadados Zeno, VU-meter circular multicolorido calculado com base no áudio quando possível, tela de instalação, funcionamento em Android/iOS/Windows, layout compacto sem rolagem e dois controles inferiores (ligar/desligar + compartilhar).

**Limitações:** as políticas do navegador podem exigir um toque para liberar o som. O visualizador baseado no áudio depende de CORS do provedor; sem permissão CORS, o app prioriza reproduzir o áudio. A transmissão não foi comprovada online nesta entrega sem teste real no dispositivo. Envio do convite só ocorre depois que a pessoa confirma no WhatsApp.

## Arquivos

`index.html`, `styles.css`, `app.js`, `config.js`, `landing.js`, `gate.js`, `sw.js`, `manifest.webmanifest`, `.nojekyll`, `assets/` e `icons/`. `README.md` serve apenas como orientação.

**Versão de cache da nova emissora:** `radio-esperanca-1011-v1.9.4-01`.
