# Bridge Lite — Web Edition

Reimplementação web independente, mobile-first, para edição de projetos de Minecraft Bedrock.

## Publicar no GitHub Pages
1. Extraia este ZIP.
2. Envie `index.html`, `app.js`, `styles.css`, `manifest.webmanifest` e `sw.js` para a raiz de um repositório.
3. Abra **Settings → Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`.

## Recursos desta versão
- Interface responsiva para celular e desktop.
- Criar projeto com `manifest.json`.
- Explorador de arquivos e pastas.
- Editor de texto com suporte a JSON, JavaScript e MCFunction.
- Validação e formatação JSON.
- Importação de `.zip`, `.mcpack`, `.mcaddon` e `.mcworld` (um pacote por vez), além de arquivos individuais.
- Exportação ZIP.
- Salvamento automático no armazenamento local do navegador.
- Indicador de progresso para importação, exportação e compactação.
- PWA e cache offline da interface.

## Limitações honestas
Esta é uma base funcional de reimplementação, não paridade completa com Bridge v2. Não possui ainda IntelliSense Bedrock, árvore JSON visual, editor de entidades/ícones/animações, plugins do Bridge, leitura direta da pasta `com.mojang`, sincronização com Minecraft ou suporte a todos os formatos binários. Os módulos ZIP são carregados sob demanda via jsDelivr na primeira importação/exportação ZIP; a edição de texto funciona sem esse módulo.

## Licença e origem
Projeto independente, sem reutilização do código-fonte do Bridge. O Bridge original é um projeto separado; esta interface não é oficial nem afiliada ao Bridge Core.
