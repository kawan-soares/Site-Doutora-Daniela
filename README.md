# Clínica de Psicologia Alpha Equilíbrio

Site da psicóloga **Daniela da Silva Soares** (CRP 06/122468), psicóloga clínica e neuropsicóloga, com atendimento on-line e presencial em Alphaville – Barueri/SP.

🌐 **No ar:** [clinicaalphaequilibrio.com.br](https://clinicaalphaequilibrio.com.br)

📍 Alameda Rio Negro, 967 – Sala 613 · Edifício Alpha Premium · Alphaville – Barueri/SP

## Sobre o site

Página única em HTML, CSS e JavaScript puro, sem frameworks e sem etapa de build.

- Áreas de atuação, equipe e profissionais parceiros em páginas próprias, cada uma com seu link (`/#area-ansiedade`, `/#equipe`, `/#parceiros`)
- Agendamento pelo WhatsApp
- Painel de acessibilidade com Libras (VLibras), leitura em voz alta, tamanho do texto, alto contraste e outras ferramentas
- Imagens em WebP com carregamento sob demanda; mapa e VLibras só carregam quando a pessoa pede
- Dados estruturados (JSON-LD) e prévia de compartilhamento para WhatsApp e redes sociais

## Estrutura

```
index.html   → página completa (HTML + CSS + JS)
images/      → fotos, logo, ícone e imagem de compartilhamento
```

## Como editar

Tudo fica no `index.html`.

**CRP:** procure `var CRP =`. O número aparece sozinho no topo, no "Sobre", na equipe e no rodapé.

**Profissionais parceiros:** procure `var PARCEIROS = [`. Para incluir alguém:

1. Copie um bloco `{ ... }` e cole abaixo do último, com uma vírgula entre eles.
2. Troque os dados (nome, CRP, formação, abordagem, público, modalidade, apresentação, áreas).
3. Coloque a foto quadrada na pasta `images/` e aponte o campo `foto` para ela.
4. No campo `whatsapp`, use só números com 55 + DDD. Vazio (`""`) usa o WhatsApp da clínica.

## Publicação

O site é publicado pelo Netlify, ligado a este repositório. Todo `git push` na branch `main` atualiza o site em menos de um minuto:

```bash
git add .
git commit -m "descrição da alteração"
git push
```

## Desenvolvimento

Desenvolvido por [Kawan Fernandes](https://github.com/kawan-soares).
