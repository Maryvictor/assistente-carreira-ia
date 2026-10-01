# 🔎 Assistente de Carreira com IA

> Uma consultora de carreira construída com IA generativa que analisa a vaga **antes** da candidatura e responde: *vale a pena investir meu tempo nessa vaga?*

Projeto pessoal de **Maria Victor**, construído com **Claude (Anthropic), Claude Projects e engenharia de prompt**.

---

## 💡 O que ele faz

A partir do link de uma vaga, o assistente segue um fluxo fixo:

```mermaid
flowchart LR
    A[Link da vaga] --> B[Leitura da vaga]
    B --> C[Pesquisa da empresa]
    C --> D[Glassdoor e salário]
    D --> E[Score Técnico + Cultural]
    E --> F{Deseja se candidatar?}
    F -- Sim --> G[Currículo ou carta<br/>personalizados]
    F -- Não --> H[Próxima vaga]
```

```
Score Geral = (Técnico × 1 + Cultural × 3) ÷ 4

≥ 65%   → Vai nessa! 🚀
45–64%  → Vai por sua conta e risco ⚠️
< 45%   → Corre que é cilada! 🚨
```

## ⏱️ Por que eu criei

- **Economizo tempo** analisando cada vaga e gerando um currículo (ou carta) específico para ela.
- **Aposto nas vagas certas** para a minha experiência e o meu perfil, em vez de me candidatar em volume.
- **A decisão final é sempre minha:** o assistente para depois da análise e só gera o currículo se eu disser "sim".
- **Nada é inventado:** se falta informação, ele avisa em vez de preencher.

O prompt passou por **várias versões** até chegar a este formato, ajustando critérios, pesos e regras conforme eu usava no dia a dia.

## 📂 Arquivos de referência (privados)

O assistente se apoia em materiais que eu construí com acompanhamento profissional. Eles **não estão publicados** aqui por conterem dados pessoais, mas é importante saber de onde vêm:

| Arquivo | O que é | Origem |
|---|---|---|
| **Currículo mestre** | Histórico completo de experiências, projetos e resultados | É o perfil completo do LinkedIn em Pdf |
| **Currículo ATS** | Versão otimizada para sistemas de triagem automática (ATS) | Construído com um mentor de carreira |
| **Perfil DISC** | Modelo comportamental que descreve como a pessoa age no trabalho a partir de quatro fatores: Dominância, Influência, Estabilidade e Conformidade | Teste da Intermetrics, analisado com um mentor de carreira |
| **Motivadores** | O que me dá energia e sentido no trabalho | Teste da Intermetrics, analisado com um mentor de carreira |
| **Sabotadores** | Padrões mentais que me tiram do meu melhor, baseados no livro *Inteligência Positiva* | Analisado com um mentor de carreira |

É por isso que a **cultura pesa 3x mais** que a parte técnica no score: o perfil comportamental não é um palpite da IA, é um diagnóstico feito com especialistas.

## 📁 Estrutura

```
├── prompt/
│   └── assistente-de-carreira.md   # o prompt completo
└── exemplos/
    └── exemplo-analise.md          # uma análise real, anonimizada
```

## 🛠️ Stack

`Claude (Anthropic)` · `Claude Projects` · `Engenharia de prompt` · `Busca web` · `Otimização para ATS`

---

**Maria Victor** · Analista de Dados · MBA em Analytics & IA (FIA)
