RFC – Detecção Automática e Explicável de Fake News usando IA

RFC ID: RFC-001
Título: Plataforma Web de Detecção de Fake News com Explicabilidade Integrada
Autor: Lucas Matheus Rodrigues
Data: 02/12/2025
Status: Proposta / Em Revisão
Versão: 1.0

1. Contexto

A desinformação se espalha rapidamente nas redes sociais, influenciando política, saúde pública e opinião social. Ferramentas atuais de fact-checking são manuais e lentas, e sistemas automáticos não explicam suas decisões.

Este projeto propõe uma solução automatizada, escalável e explicável.

2. Problema

A desinformação cresce mais rápido do que a capacidade humana de verificar.

Classificadores automáticos não explicam suas decisões.

Usuários têm dificuldade em confiar em sistemas sem transparência.

3. Objetivo

Criar uma aplicação web capaz de detectar fake news usando NLP e fornecer explicações claras sobre o motivo da classificação.

4. Escopo da Solução (MVP)
Entrada

Usuário fornece um texto ou notícia.

Processamento

Modelo NLP (ex.: BERT/RoBERTa) classifica o texto.

LIME/SHAP/Attention explicam o motivo.

API externa de fact-checking confirma em fontes confiáveis.

Saída

Probabilidade de ser fake news.

Explicação textual.

Highlight dos trechos suspeitos.

Links para verificação cruzada.

5. Público-Alvo

Jornalistas

Estudantes e pesquisadores

Público geral

Instituições públicas e ONGs

6. Diferenciais

Explicabilidade integrada (XAI)

Verificação cruzada automática

Interface acessível

Escalabilidade para integração futura via API

Caráter educacional

7. Arquitetura Proposta
7.1. Frontend

React ou Next.js

Interface para inserir texto e visualizar explicações

7.2. Backend

Python (FastAPI ou Flask)

Módulos:

Classificação NLP

Explicabilidade XAI

Verificação cruzada

7.3. Banco de Dados

PostgreSQL

Armazena histórico de consultas e feedback

7.4. Serviços Externos

Google Fact Check Tools

Reuters Fact Check

Wikipedia API

8. Requisitos
Requisitos Funcionais

RF01 – Permitir ao usuário inserir texto

RF02 – Classificar automaticamente

RF03 – Exibir explicabilidade

RF04 – Consultar APIs externas

RF05 – Salvar histórico

Requisitos Não Funcionais

RNF01 – Resposta ≤ 3 segundos

RNF02 – Precisão ≥ 80%

RNF03 – Interface responsiva

RNF04 – API documentada

RNF05 – Arquitetura modular

9. Datasets

FakeNewsNet

LIAR Dataset

PHEME Dataset

BR-Fake (caso inclua português)

10. Critérios de Sucesso

Transparência compreendida pelos usuários

Precisão ≥ 85%

MVP funcional

Feedback positivo em testes

11. Riscos

Viés nos datasets

Limites de APIs externas

Explicabilidade difícil de interpretar para leigos

12. Conclusão

A solução oferece uma plataforma moderna para detecção automática e explicável de fake news, combinando NLP, verificações externas e transparência para enfrentar a desinformação.
