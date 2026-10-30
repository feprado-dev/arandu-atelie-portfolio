# Arandu Ateliê — landing page de portfólio

Landing page de página única para um escritório de arquitetura **fictício**, feita como projeto de portfólio. Marca, arquiteta (Beatriz Valença), textos e contatos são inventados; fotos e vídeos são apenas ilustrativos.

HTML, CSS e JavaScript puros, sem build e sem dependências.

## Destaques técnicos

- **Vídeos leves:** cada vídeo começa como uma imagem de capa (carrega na hora); o vídeo só é baixado depois do `load` da página, quando a seção se aproxima da tela, e pausa fora dela. Não carrega com "reduzir movimento" nem em economia de dados.
- **Linha interativa:** no manifesto, uma linha SVG acompanha o mouse indo e voltando (`clipPath`), com um ponto luminoso e um rastro de nuvem desenhado em `<canvas>`; no celular, segue a rolagem.
- **Formulário para WhatsApp:** monta a mensagem com nome, cidade, tipo de projeto e recado (aqui em modo demonstração).
- **Responsivo:** testado de 320 px a 1440 px, inclusive tablet e celular deitado.
- **Acessibilidade:** respeita `prefers-reduced-motion`, textos alternativos e alvos de toque de 44 px.
- **Segurança (Vercel):** `vercel.json` com CSP, `nosniff`, `X-Frame-Options` e cache para os arquivos.

## Rodar localmente

```bash
python3 -m http.server 5219
```

e abra http://localhost:5219.
