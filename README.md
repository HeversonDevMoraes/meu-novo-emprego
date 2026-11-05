# Meu Emprego Novo 🤖💼

> Transforme sua busca de emprego em um pipeline de dados inteligente, automatizado com agentes de IA (CrewAI + LLMs) e validado por uma única fonte de verdade.

---

## 📖 Visão Geral

Procurar emprego não deve ser um processo exaustivo de envios no escuro. Este repositório implementa um **método estruturado** aliado a uma **ferramenta CLI multi-agente** que lê a descrição de uma vaga e a sua base profissional para gerar currículos personalizados em PDF/LaTeX (em Português ou Inglês), com foco em **zero alucinação** e preservação total da trajetória de carreira.

🔗 **Recursos do Projeto:**
- 📘 [Acesse o E-book Oficial do Método (Gamma)](https://gamma.app/docs/Pipeline-de-Carreira-com-IA-b12la24s0m1z38z)
- 🌐 **Autor:** Heverson Moraes (Curitiba – PR) | [Portfólio & Links](https://linktr.ee/heversonmoraesdev)

---

## ⚙️ O Método: Pipeline de Carreira em 4 Passos

1. **Preparar:** Registrar a trajetória real e honesta em um único arquivo de verdade (`profile_truth.md`) antes de adaptar qualquer currículo.
2. **Encontrar:** Ler a vaga por requisitos, hard/soft skills e contexto.
3. **Candidatar:** Gerar currículos específicos, auditados e legíveis com auxílio de agentes inteligentes.
4. **Aprender:** Registrar o feedback, analisar relatórios de cobertura e ajustar os próximos ciclos de candidatura.

---

## 🤖 Arquitetura da Ferramenta (Agentes IA)

O sistema utiliza agentes especializados integrados via CrewAI para gerenciar a qualidade de ponta a ponta:

- **Estrategista de Carreira:** Analisa a descrição da vaga e reordena/adapta o perfil sem inventar informações.
- **Gerente de Contratação (Avaliador):** Atribui notas rigorosas de 1 a 10 e aponta lacunas e palavras-chave.
- **Editor de Currículo:** Aplica correções e gera os artefatos em JSON, LaTeX e PDF.
- **Loop de Qualidade:** O ciclo entre Gerente e Editor repete-se internamente até o currículo atingir a nota mínima de corte **(≥ 8.5)**.
- **Coach de Entrevista:** Produz um roteiro personalizado com base nas lacunas identificadas na vaga.

---

## 🛠️ Tecnologias Utilizadas

- **Backend / Orquestração:** Python 3.12, CrewAI
- **Provedores de LLM:** OpenAI (GPT-4o), AWS Bedrock (Claude) ou Google Gemini
- **Geração de Documentos:** LaTeX (`pdflatex`) para PDFs de alto padrão profissional

---

## 🚀 Como Começar

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/R238Company/meu-emprego-novo.git](https://github.com/R238Company/meu-emprego-novo.git)
   cd meu-emprego-novo