# Curso de Terapia Floral AYA — landing page

Página refeita a partir de https://landpageflorais.netlify.app, mantendo as mesmas informações,
os mesmos valores e o mesmo fluxo de pagamento (Mercado Pago via função Netlify).

## Arquivos

- `index.html` — página completa (copy, estrutura e scripts)
- `assets/styles.css` — estilos, animações e responsivo
- `assets/img/florais.jpg` — foto usada no hero
- `assets/favicon.svg` — ícone

## Publicar no Netlify

1. Substitua o `index.html` do site atual por este e envie a pasta `assets/`.
2. Mantenha a função `/.netlify/functions/create-preference` já publicada; o botão de pagamento
   continua chamando esse mesmo endpoint com `{ method: "pix" }` ou `{ method: "card" }`.
3. Depois do deploy, teste os dois botões e confira a página de retorno.

## O que foi feito

- Hero em tela cheia com a foto preenchendo a seção e degradê para leitura do texto.
- Cabeçalho transparente sobre o hero e sólido depois que a seção sai da tela.
- Entrada orquestrada: zoom lento da foto, véu que fecha, título linha por linha, texto e CTA em sequência.
- Revelações no scroll, contagem animada dos números (16 módulos, 325 aulas) e hovers em cards, lista e botões.
- Botão flutuante de WhatsApp (5541 99916-8655) e link de dúvidas ao lado do ticket.
- Barra fixa de compra no celular com o valor do Pix, que some quando a seção de inscrição aparece.
- `prefers-reduced-motion` respeitado: com a preferência ativa, tudo aparece sem animação.

## GitHub Pages

A página funciona no GitHub Pages como vitrine, mas o checkout não: a função
`/.netlify/functions/create-preference` só existe no Netlify. No Pages, os botões de pagamento
mostram um aviso e o link para o WhatsApp. Para vender, use o deploy do Netlify.

## Conteúdo

Todo o texto veio da página original. Nenhum dado, depoimento ou número foi inventado.
