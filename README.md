# Mr Photo Retro · V0

Landing page estática e responsiva para apresentação. Inclui proposta de valor, como funciona, galeria com placeholders, personalização de cabine e fotos, ocasiões e contato.

## Executar

Requer Node.js 20 ou superior. Não há dependências para instalar.

```sh
npm run build
```

Abra `dist/index.html` no navegador. Todo o conteúdo, CSS e comportamento estão em `src/index.html`, permitindo também abrir esse arquivo diretamente para apresentar. As fontes Federo e Montserrat são carregadas pelo Google Fonts; há fontes de fallback offline.

## Cloudflare Pages

Conecte o repositório e selecione a branch após aprovação do PR.

- Framework: None
- Comando de build: `npm run build`
- Diretório de saída: `dist`
- Diretório raiz: raiz do repositório

Não requer backend, tokens ou variáveis de ambiente. Esta entrega não altera DNS nem publica no domínio oficial.

## Antes do lançamento comercial

- Substituir o wordmark provisório pelo logo oficial.
- Adicionar foto da cabine, galeria e exemplos reais de personalização nos espaços identificados. Ao usar imagens, fornecer alt, width e height; carregar as da galeria com loading="lazy".
- Preencher `WHATSAPP_NUMBER` no script com país + DDD + número. Enquanto vazio, o botão abre uma explicação da prévia e não envia mensagens.
- Confirmar Instagram e região de atendimento, substituindo o aviso do rodapé.
- Confirmar copy e condições comerciais da personalização.
- Remover a faixa de prévia, as notas de dados pendentes e a meta `robots` noindex quando a versão comercial estiver aprovada. Até lá, manter noindex.

## Direção visual

Cores: #1A3263, #547792, #FAB95B, #E8E2DB e #141414. Federo nos títulos e Montserrat no texto. Slogan: “A sua melhor memória!”. Sem fotos de banco apresentadas como eventos realizados, números de clientes ou depoimentos inventados.

A V0 usa HTML/CSS/JS estáticos sem dependências para permitir apresentação imediata. A estrutura pode ser migrada para Astro quando houver necessidade de componentes e mais páginas; esta versão não usa Astro.
