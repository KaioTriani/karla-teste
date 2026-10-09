# Karla Albuquerque Advocacia

Site completo e responsivo, preparado para importar do GitHub na Hostinger. Inclui imagens locais, WhatsApp, Instagram, localização, áreas de atuação, avaliações públicas e perguntas frequentes. HTML, CSS e JavaScript com Vite para gerar os arquivos de produção.

## Importar na Hostinger

No hPanel, crie um **Web App**, escolha **Importar repositório Git** e selecione `KaioTriani/karla-teste`.

| Configuração | Valor |
| --- | --- |
| Branch | `main` |
| Diretório raiz | `.` (raiz do repositório) |
| Framework | `Vite` |
| Node.js | `22.x` ou `24.x` |
| Gerenciador | `npm` |
| Instalação | `npm ci` |
| Comando de build | `npm run build` |
| Diretório de saída | `dist` |
| Variáveis de ambiente | Nenhuma |

O resultado é um site estático: não precisa de banco de dados, chave de API ou servidor Node em produção. Não use o comando de desenvolvimento como servidor de produção. Após publicar, associe o domínio e confirme o HTTPS no painel.

O fluxo de Web Apps da Hostinger requer um plano compatível. Consulte a [documentação oficial](https://www.hostinger.com/support/how-to-deploy-a-nodejs-website-in-hostinger/).

### Hospedagem tradicional / public_html

Se utilizar hospedagem estática tradicional, execute `npm ci` e `npm run build` localmente e envie **o conteúdo de `dist`** para `public_html`. O `index.html` deve estar diretamente dentro de `public_html`.

## Executar localmente

```sh
npm ci
npm run dev
```

Para conferir a versão de produção:

```sh
npm run build
npm run preview
```

## Arquivos

- `index.html`: conteúdo e metadados.
- `style.css`: layout, responsividade e animações.
- `app.js`: menu mobile e animações de entrada.
- `assets/`: foto local utilizada pelo site (`portrait.jpeg`).
- `vite.config.js`: build com caminhos relativos para permitir instalação em domínio ou subpasta.
- `package-lock.json`: versões fixadas para instalação reproduzível.

Fontes Google Fonts e mapa Google Maps precisam de internet. Os contatos abrem WhatsApp ou telefone, sem enviar mensagens automaticamente. Não há dependência do ChatGPT/Sites para funcionar.

## Conteúdo

Telefone, endereço, experiência e foto foram obtidos do [site oficial](https://karlaalbuquerqueadv.com.br/sobre). Os trechos de Bela Dias e Igor Morais, nota 5,0 e 25 avaliações foram conferidos no Google em 08/10/2026; essa informação é estática. OAB e e-mail foram omitidos conforme orientação do responsável. As áreas de atuação seguem o briefing original.

Esta importação prepara e disponibiliza os arquivos no GitHub; a publicação e a configuração do domínio na Hostinger são feitas no painel da hospedagem.
