# Bridge Lite

Versão web leve experimental para edição básica de projetos Minecraft Bedrock.

## Publicar no GitHub Pages
1. Crie um repositório no GitHub.
2. Envie **todos os arquivos desta pasta** para a raiz do repositório.
3. Abra **Settings → Pages**.
4. Em Build and deployment, escolha **Deploy from a branch**.
5. Selecione `main` e `/ (root)` e salve.
6. Aguarde a publicação e abra o endereço fornecido pelo GitHub.

O projeto usa caminhos relativos, então funciona em repositórios GitHub Pages com endereço `/nome-do-repositorio/`.

## Recursos implementados
- Interface responsiva para celular e desktop.
- Arquivos JSON, JS, TS, MCFunction e texto.
- Importação de arquivos ou diretórios via seletor do navegador.
- Criação de arquivos e caminhos de pasta.
- Salvamento automático local via IndexedDB.
- Validação e formatação básica de JSON.
- Exportação do projeto como ZIP.
- PWA e cache dos arquivos principais.

## Limitações importantes
Esta é uma base Lite independente, não uma conversão completa do Bridge 1.8.5. Ainda não inclui Monaco/IntelliSense, autocomplete de componentes Bedrock, plugins do Bridge, integração direta com a pasta `com.mojang`, visualizador avançado de entidades, nem importação automática de `.mcaddon`/`.mcpack`. Navegadores móveis não permitem acesso irrestrito ao sistema de arquivos; a importação/exportação ocorre pelos seletores e downloads do navegador.

A biblioteca JSZip é carregada por CDN para reduzir o tamanho inicial do app. A primeira exportação ZIP requer conexão. O restante da interface pode ser armazenado em cache pelo PWA após a primeira visita.

## Privacidade
Os arquivos ficam no armazenamento local do navegador deste dispositivo. Não há servidor de upload implementado. Limpar os dados do site/navegador pode apagar projetos locais; exporte cópias ZIP regularmente.

## Nota sobre o código-fonte de referência
O ZIP fornecido foi analisado como referência de arquitetura e recursos. Esta implementação Lite é uma base web separada e não incorpora o código original do Bridge.
