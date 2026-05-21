# Dio's Portfolio & Links | Site Pessoal

Este é o meu website. Um projeto focado em minimalismo, performance e acessibilidade, construído com HTML e CSS puros. O objetivo principal é servir como meu portfólio oficial.

 **Live Demo:** [https://diogo-abreu.vercel.app/](https://diogo-abreu.vercel.app/)

---

## Tech Stack & Architecture

A filosofia deste projeto é *Keep It Simple* (KISS). Evitei frameworks pesados (React/Next.js) para garantir um carregamento instantâneo em qualquer dispositivo.

- **Frontend:** HTML5 & CSS3 puro (BEM methodology structure).
- **Typography:** Noto Sans Mono (IETF hosted).
- **SEO & Semântica:** 
  - Dados estruturados usando **JSON-LD (Schema.org)** com os tipos `ProfilePage` e `Person`.
  - Configuração rigorosa de Meta Tags Open Graph para compartilhamento em redes sociais.
- **Internacionalização (i18n):** Estrutura de roteamento estático nativo via subpastas (`/` para PT-BR e `/en` para EN) com tags `hreflang` configuradas para SEO internacional.

---

## CI/CD & Infrastructure

Mesmo sendo um projeto estático, a esteira de desenvolvimento segue padrões de projeto:

- **Deployment & Hosting:** [Vercel](https://vercel.com/) (Edge Network).
- **Git Flow Automatizado:**
  - Branch `main` reflete o ambiente de produção.
  - Branch `develop` usada para integração de features.
  - **Preview Branches:** Cada Pull Request gera um deploy isolado automaticamente via Vercel CI/CD para testes antes do merge final.
- **SEO Crawling:** Configuração personalizada de `robots.txt` e `sitemap.xml`.

---

## Project Structure

```text
├── assets/             # Imagens, ilustrações da OC (Aska) e mídias
├── en/                 # English version of the portfolio
│   └── index.html      # English entry point
├── index.html          # Main entry point (PT-BR)
├── styles.css          # Estilos globais do projeto
├── robots.txt          # Regras de indexação para motores de busca
└── README.md           # Esta documentação

