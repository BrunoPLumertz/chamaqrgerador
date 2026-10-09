# ChamaQR · Criador de Posts

Gerador de posts para **Instagram** e **LinkedIn** do [ChamaQR](https://chamaqr.lovable.app).
Escolha **setor**, **especialidade** e **finalidade** e o post sai pronto, com legenda e hashtags.
Tudo roda no navegador: um único `index.html`, sem build e sem servidor.

## O que faz

- **Criar post em 3 cliques:** setor → especialidade → finalidade → **Montar post**.
  São 8 setores, 16 especialidades e 7 finalidades, com 5 versões de cada combinação (560 posts).
- **🎲 Surpreenda-me:** sorteia uma combinação.
- **↻ Outra versão / ↻ Título / ↻ Subtítulo / ↻ Botão:** troca a versão inteira ou só um texto.
- **Formatos:** Instagram 1080×1080 e 1080×1350 (vertical, com parágrafo de apoio extra) e LinkedIn 1200×1200 e 1200×627.
- **Sessões:** monte vários posts de uma vez (por exemplo, "Apresentação do produto", "Marketing", "Casos de uso"), escolha a quantidade de cada uma e baixe tudo em **ZIP**.
- **Downloads:** PNG do post atual, **ZIP com todos os formatos** do post atual e ZIP por sessão ou dos posts selecionados. O ZIP inclui a legenda.
- **Ajustes avançados:** editar título, subtítulo, botão, legenda, hashtags, estilo (Paper, Dark, Cyan, Impacto), layout (clássico, cor invertida, centralizado), visual (QR Code, etiquetas, lista com check, número grande, aspas) e o link do QR.
- **QR Code real** (escaneável), gerado no navegador e apontando para o link que você definir.
- **Seu trabalho fica salvo** no navegador (post em edição, sessões e último setor/finalidade).

## Design

- Paleta do ChamaQR: branco, creme-azulado, grafite e vermelho.
- Tipografia Inter, embutida no arquivo, para o PNG sair igual ao que aparece na tela.
- Quebras de linha cuidadas: linhas equilibradas, sem palavra solta no fim e sem separar "QR Code" ou "Mesa 12".

## Publicar no Vercel

1. Suba `index.html`, `vercel.json` e este `README.md` na raiz do repositório (branch `main`).
2. O Vercel faz o deploy automaticamente a cada commit. Não precisa de configuração de build.

## Notas

- Não há dependências externas em tempo de execução: as bibliotecas de QR Code ([qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator), MIT) e de ZIP ([JSZip](https://stuk.github.io/jszip/), MIT ou GPLv3) estão embutidas no `index.html`.
- A geração de texto por IA só existe na versão publicada dentro do Claude. No Vercel, os textos vêm do montador por tema e objetivo, sem IA.
- Os textos de exemplo usam só o que a página do ChamaQR informa (sem app, sem cadastro para quem escaneia, protocolo, plano grátis com até 5 pontos). Revise-os se o produto mudar.
