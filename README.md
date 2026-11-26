# Certifications Hub — Plataforma de Estudos & Simulados (Datadog & AWS)

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Online-brightgreen?logo=github)](https://araujoajoao.github.io/studylab/)
[![Simulados](https://img.shields.io/badge/Questões-225%20Reais-blue)](#)
[![Single File SPA](https://img.shields.io/badge/Arquitetura-100%25%20Autocontida-orange)](#)

Laboratório consolidado de estudos e simulados interativos para as certificações oficiais da **Datadog** e **AWS**.

---

## 🌐 Acesso Online Imediato (GitHub Pages)

O hub completo está publicado e acessível publicamente pelo navegador sem necessidade de download:

👉 **[https://araujoajoao.github.io/studylab/](https://araujoajoao.github.io/studylab/)**

- **Acesso direto aos exames por URL hash:**
  - AWS Cloud Practitioner: `https://araujoajoao.github.io/studylab/#aws_ccp`
  - Datadog Fundamentals: `https://araujoajoao.github.io/studylab/#dd_fund`
  - Datadog APM & Tracing: `https://araujoajoao.github.io/studylab/#dd_apm`

---

## 🚀 Como Usar & Compartilhar

### 📱 Compartilhamento em Arquivo Único (WhatsApp / Telegram / E-mail)
O arquivo [`index.html`](index.html) (ou suas cópias idênticas [`StudyLAB_Simulados_Completo.html`](StudyLAB_Simulados_Completo.html) e [`Certifications_Hub_Simulados_Completo.html`](Certifications_Hub_Simulados_Completo.html)) é **100% autocontido (Single Page Application offline)**:
- Contém o Hub Central + os 3 simulados completos (225 questões) + todos os modos de estudo + gerador offline de decks Anki.
- **Basta enviar esse único arquivo `.html`** por WhatsApp ou e-mail. Qualquer pessoa no celular (Android/iOS) ou computador abre e navega por todos os simulados sem precisar de pastas ou arquivos adicionais!

```bash
# Abrir no navegador
open index.html
# Ou
open StudyLAB_Simulados_Completo.html
```

Você também pode abrir os simulados modulares individuais na pasta `simulados/`:
* **AWS Certified Cloud Practitioner:** `open simulados/aws_ccp_simulado_01.html`
* **Datadog Fundamentals:** `open simulados/datadog_fundamentals_simulado.html`
* **Datadog APM & Distributed Tracing:** `open simulados/datadog_apm_simulado.html`

---

## 📂 Estrutura do Diretório

```
studylab/
├── index.html                                 # Hub central autocontido (3 simulados embutidos)
├── StudyLAB_Simulados_Completo.html           # Cópia idêntica do index.html
├── Certifications_Hub_Simulados_Completo.html # Cópia idêntica do index.html
├── favicon.ico / favicon.png
├── .nojekyll                                  # Desativa o Jekyll no GitHub Pages
│
├── simulados/                                 # Pasta dedicada aos arquivos finais dos simulados
│   ├── aws_ccp_simulado_01.html               # Aplicação Web: AWS CCP Simulado 01 (45 Qs)
│   ├── aws_ccp_questions.json                 # Dataset JSON AWS CCP com justificativas oficiais
│   ├── aws_ccp_anki.csv                       # Deck Anki AWS CCP (Pronto para importação)
│   │
│   ├── datadog_fundamentals_simulado.html     # Aplicação Web: Datadog Fundamentals (90 Qs)
│   ├── datadog_fundamentals_questions.json    # Dataset JSON Fundamentals (Bilíngue PT/EN)
│   ├── datadog_fundamentals_anki.csv          # Deck Anki Fundamentals (Pronto para importação)
│   ├── Datadog Fundamentals Practice Exam - Complete 90 Questions.pdf # PDF Oficial
│   │
│   ├── datadog_apm_simulado.html              # Aplicação Web: Datadog APM & Tracing (90 Qs)
│   ├── datadog_apm_questions.json             # Dataset JSON APM (Bilíngue PT/EN, balanceado)
│   ├── datadog_apm_anki.csv                   # Deck Anki APM (Pronto para importação)
│   └── Datadog APM Practice Exam - Complete 90 Questions.pdf # PDF Oficial
│
└── assets/                                    # Logos, favicons e identidade visual
    ├── aws-logo.svg / datadog-logo.svg / datadog-logo.png
    └── favicon-*.png / apple-touch-icon.png
```

---

## 🎯 Modos de Estudo Disponíveis

1. **🎓 Modo Treino:** Responda questão a questão com validação imediata e explicação técnica oficial.
2. **⏱️ Modo Simulado:** Prova com cronômetro proporcional oficial, nota de corte (70%) e relatório de acertos.
3. **📊 Modo Gabarito & Revisão:** Visualização da submissão com badges claras de acertos e erros e gabarito fundamentado.
4. **🃏 Flashcards 3D:** Cartões interativos para repetição espaçada com atalhos de teclado (<kbd>Espaço</kbd> para virar, <kbd>→</kbd> para avançar, <kbd>F</kbd> para marcar).
5. **📖 Guia Rápido (Cheat Sheet):** Tabelas de consulta rápida com portas, variáveis de ambiente e serviços.
6. **🌐 Suporte Bilíngue / Justificativas:** Explicações oficiais técnicas em Português e Inglês.

---

## 🛠️ Atualizar Dados ou HTML

Os scripts de geração não fazem parte deste repositório: os HTMLs são os artefatos finais e embutem os dados das questões. Ao alterar uma questão, mantenha sincronizados:

1. O dataset em `simulados/*_questions.json` (e o deck `*_anki.csv`, se aplicável);
2. O array de questões embutido no simulado individual (`simulados/*_simulado*.html`);
3. O objeto `EXAMS_DATA` em `index.html`, incluindo os rótulos de seções/domínios;
4. As cópias `StudyLAB_Simulados_Completo.html` e `Certifications_Hub_Simulados_Completo.html`:

```bash
cp index.html StudyLAB_Simulados_Completo.html
cp index.html Certifications_Hub_Simulados_Completo.html
```

