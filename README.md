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
O arquivo [`index.html`](file:///home/joaoaraujo/Documents/labs/StudyLAB/index.html) (ou [`StudyLAB_Simulados_Completo.html`](file:///home/joaoaraujo/Documents/labs/StudyLAB/StudyLAB_Simulados_Completo.html)) é **100% autocontido (Single Page Application offline)**:
- Contém o Hub Central + os 3 simulados completos (225 questões) + todos os 5 modos de estudo + gerador offline de decks Anki.
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
StudyLAB/
├── index.html                                 # Portal central de acesso a todos os exames
│
├── simulados/                                 # Pasta dedicada aos arquivos finais dos simulados
│   ├── aws_ccp_simulado_01.html               # Aplicação Web: AWS CCP Simulado 01 (45 Qs)
│   ├── aws_ccp_questions_enriched.json        # Dataset JSON AWS CCP com justificativas oficiais
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
├── assets/                                    # Logos e identidade visual
│   └── datadog-logo.png
│
├── scripts/                                   # Scripts de compilação, parsing e exportação
│   ├── build_aws_simulado.py                  # Gera questions enriched da AWS
│   ├── generate_aws_html.py                   # Compila o HTML interativo da AWS
│   ├── build_consolidated_dataset.py          # Gera questions.json do Datadog Fundamentals
│   ├── generate_html_v2.py                    # Compila o HTML do Datadog Fundamentals
│   ├── generate_anki_csv.py                   # Exporta o CSV para Anki do Fundamentals
│   ├── build_apm_consolidated_dataset.py      # Gera questions.json do Datadog APM
│   └── generate_apm_html.py                   # Compila o HTML do Datadog APM
│
└── archive/                                   # Histórico de extrações, dumps e rascunhos
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

## 🛠️ Recompilar Dados ou HTML

Para atualizar ou reprocessar os dados para a pasta `simulados/`:

```bash
# AWS Certified Cloud Practitioner
python3 scripts/build_aws_simulado.py
python3 scripts/generate_aws_html.py

# Datadog Fundamentals
python3 scripts/build_consolidated_dataset.py
python3 scripts/generate_html_v2.py
python3 scripts/generate_anki_csv.py

# Datadog APM & Distributed Tracing
python3 scripts/build_apm_consolidated_dataset.py
python3 scripts/generate_apm_html.py
```

