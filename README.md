# Vencato e Cardoso — Site institucional

Site institucional da Vencato e Cardoso Advogados Associados. HTML, CSS e JavaScript puros — sem framework, sem build step.

## Estrutura

```
├── home.html            # Página inicial
├── institucional.html   # Sobre o escritório
├── equipe.html          # Sócios e colaboradores
├── areas.html           # Áreas de atuação (PF/PJ)
├── blog.html            # Blog e livros publicados
├── contato.html         # Canais de contato, formulário e mapa
├── css/                 # style.css (compartilhado) + um arquivo por página
├── assets/
│   ├── img/              # Fotos e capas de livros
│   ├── logo/              # Logotipo oficial (SVG)
│   └── icones/             # Ícones SVG usados no site
├── robots.txt
└── sitemap.xml
```

## Rodando localmente

Como não há build step, basta abrir os arquivos `.html` direto no navegador, ou servir a pasta com qualquer servidor estático, por exemplo:

```bash
npx serve .
```

## Formulário de contato

O formulário de ouvidoria (`contato.html`) envia e-mails via [FormSubmit](https://formsubmit.co), sem precisar de backend próprio. O e-mail de destino está configurado no atributo `action` do `<form id="form-ouvidoria">` em `contato.html`.

## Deploy

Site estático — pronto para deploy direto na Vercel (ou qualquer hospedagem estática), sem etapa de build.

Antes de publicar em produção, revisar:
- `robots.txt` e `sitemap.xml` (domínio já configurado para `vencatoecardoso.com.br`)
- Tags de meta/Open Graph em cada página (`<head>`)
