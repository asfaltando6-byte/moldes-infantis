# Pequenos Vestidos — página de vendas

Site estático em português, preparado para GitHub e Vercel. Prévia disponível no ChatGPT; código preparado para publicação na Vercel.

## Conteúdo

- `dist/index.html`: estrutura e textos da página.
- `dist/style.css`: estilos e adaptação para celular.
- `dist/script.js`: carrossel, preços, navegação e botões.
- `dist/config.js`: preços, quantidades e links de checkout.
- `dist/assets/`: mockup WebP e amostras vetoriais próprias.
- `vercel.json`: diretório de saída e cabeçalhos.

## Abrir no computador

Abra `dist/index.html` no navegador. Todos os arquivos e imagens estão no pacote e não dependem de fontes externas.

Para servir localmente, se tiver Python: `python3 -m http.server 8080 --directory dist`.

## Publicar pelo GitHub e Vercel

1. Use o repositório `asfaltando6-byte/moldes-infantis`.
2. Na Vercel, importe esse repositório como novo projeto.
3. Selecione o preset **Other**, sem comando de instalação ou build.
4. O diretório de saída é **dist**, já definido em `vercel.json`.
5. Publique e confira o endereço gerado.

O arquivo `.openai/hosting.json` é usado somente para a prévia de desenvolvimento; não é necessário na Vercel.

## Editar a oferta

Em `dist/config.js`, configure os dois planos:

- `preco`: valor numérico, com ponto decimal.
- `quantidade`: quantidade de referências previstas.
- `checkout`: URL HTTPS completa do checkout.

Os preços e quantidades da página e do FAQ são atualizados pelo JavaScript.
Valores iniciais propostos: Básico com 60 referências por R$ 7,90 e Premium com 180 referências + 3 bônus por R$ 19,90.
Com o checkout vazio, o botão abre um aviso de indisponibilidade, sem capturar dados ou simular uma compra.

## Estado do produto

Este pacote contém a página de vendas, seis amostras ilustrativas e o mockup. Não contém os PDFs completos de 60/180 referências ou os bônus finais.
Antes de habilitar as compras, produza e revise os materiais prometidos, confirme preço e quantidade, configure entrega no checkout e atualize as amostras para refletir os PDFs finais. Revise as informações do vendedor, contato, políticas e condições da sua operação.
A página não inclui avaliações inventadas, números de clientes, contagem regressiva, pixel ou notificações de vendas.

## Imagens

`mockup.webp` foi criado com geração de imagem integrada. Brief: fotografia editorial de catálogo visual de vestidos infantis, em ateliê de costura creme e rosa, livros e páginas abertas, luz suave, título “Pequenos Vestidos”. É uma apresentação ilustrativa.
As amostras SVG são exemplos de layout e desenhos vetoriais próprios. São referências visuais, não moldes para cortar tecidos.

## Verificação

Sintaxe dos arquivos JavaScript conferida. Imagens locais, navegação por âncoras, aviso de compra, carrossel e FAQ verificados na prévia. Layout revisado em larguras de 390px e 320px por enquadramento em iframe. Configuração pronta para importar na Vercel, sem deploy realizado.
