# Site modelo de aluguel de brinquedos

Site de uma página para empresas de aluguel de brinquedos e decoração (Pegue e Monte).
Feito para a Divertidos Brinquedos e pronto para ser adaptado a outros clientes.

## Como adaptar para um novo cliente

1. **Dados da empresa**: no fim do `index.html`, edite o bloco `CONFIG`
   (WhatsApp, número de clientes atendidos, endereço, mensagem padrão).
2. **Nome e logo**: procure por `Divertidos Brinquedos` no `index.html` e troque
   pelo nome do cliente (menu, `<title>`, rodapé e tags `og:` de compartilhamento).
3. **Cidade**: procure por `Chapecó` e troque pela cidade do cliente.
4. **Combos**: cada combo é um bloco `<article class="offer">`. Troque a imagem em
   `combos/`, o nome, o preço e a lista de itens. O primeiro (`featured`) fica em destaque.
5. **Pegue e Monte**: cada tema é um bloco `<article class="kit">`, com fotos em `pegue/`.
6. **Cores**: no topo do `<style>`, o bloco `:root` tem todas as cores
   (`--blue`, `--red`, `--yellow`, `--green`...). Mude ali para a identidade do cliente.
7. **Link de compartilhamento**: troque o endereço nas tags `og:url` e `og:image`
   pelo endereço do site do cliente.

## Publicação

Conecte o repositório a um projeto no Netlify (publish directory `.`).
Cada alteração enviada para a branch `main` é publicada automaticamente.

## Avaliações dos clientes

- O formulário "Deixe sua avaliação" envia para o Netlify (Forms › avaliacoes).
- As avaliações só aparecem no site depois de aprovadas: copie a avaliação para o
  arquivo `reviews.json`, no formato:
  `[{"nome": "Ana", "nota": 5, "alugou": "Plus Super Combo", "comentario": "Tudo perfeito!"}]`
