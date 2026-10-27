# 📋 Sistema de Monitoramento de Vagas em Tempo Real

> **Desenvolvimento de um protótipo físico e funcional de baixo custo para monitorar vagas de estacionamento em tempo real e exibir a disponibilidade aos motoristas.**

[![Status](https://img.shields.io/badge/Status-Em%20andamento-yellow)]()
[![Curso](https://img.shields.io/badge/Curso-Manutenção%20e%20Suporte-blue)]()
[![Disciplina](https://img.shields.io/badge/Disciplina-Governança%20de%20TI-purple)]()
[![Framework](https://img.shields.io/badge/Framework-IoT%20Prototyping-orange)]()

---

## 📑 Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [Problema e Justificativa](#-problema-e-justificativa)
- [Objetivos](#-objetivos)
- [Framework / Metodologia Adotada](#-framework--metodologia-adotada)
- [Escopo e Delimitações](#-escopo-e-delimitações)
- [Entregáveis](#-entregáveis)
- [Cronograma](#-cronograma)
- [Estrutura do Repositório](#-estrutura-do-repositório)
- [Como Navegar este Projeto](#-como-navegar-este-projeto)
- [Resultados e Conclusões](#-resultados-e-conclusões)
- [Referências](#-referências)
- [Glossário de Termos Técnicos](#-glossário-de-termos-técnicos)
- [Equipe](#-equipe)

---

## 🎯 Sobre o Projeto

| Campo | Detalhe |
|-------|---------|
| **Instituição** | ETEC Jaraguá |
| **Curso** | Manutenção e Suporte em Informática |
| **Disciplina** | Governança de TI |
| **Semestre** | 2026.1 |
| **Orientador(a)** | Prof. Taina Barros |
| **Tipo de Trabalho** | TCC – Trabalho de Conclusão de Curso |

**Resumo:**

Este trabalho é uma pesquisa aplicada voltada para o desenvolvimento de um protótipo físico e funcional de baixo custo, projetado para monitorar vagas de estacionamento em tempo real. O problema central é a dificuldade e o tempo gasto para localizar vagas disponíveis em ambientes lotados. A solução propõe o uso de um microcontrolador acessível (como ESP32 ou Arduino) conectado a sensores de presença ultrassônicos, integrados a um banco de dados gratuito na nuvem. A validação é feita através de testes manuais na bancada da escola usando carrinhos de brinquedo, visando entregar um sistema de resposta rápida que atualiza um aplicativo mostrando o status da vaga.

**Palavras-chave:** `IoT`, `Microcontroladores`, `ESP32`, `Sensores Ultrassônicos`, `Automação`

---

## ❗ Problema e Justificativa

### Problema

> A falta de visibilidade sobre a ocupação de vagas de estacionamento gera perda de tempo para os motoristas, aumento no consumo de combustível e estresse. Atualmente, a identificação de vagas livres é feita de forma manual e visual pelo condutor, resultando em tráfego desnecessário e sistemas comerciais possuem um alto custo de implementação.

### Justificativa

- 📊 **Dados do cenário atual:**
  - Tempo médio para encontrar vaga: 15 minutos em horários de pico.
  - Custo de implantação de sistemas comerciais: Aproximadamente R$ 3.000,00 por vaga.
- 💰 **Impacto no negócio:**
  - Otimização do tempo do motorista e melhoria no fluxo interno do estacionamento.
  - Redução drástica de custos através do uso de componentes de prototipagem acessíveis, permitindo que pequenos estacionamentos adotem a tecnologia.
- 📖 **Relevância acadêmica:**
  - Aplicação prática de conceitos de programação (Back-end e Front-end) e eletrônica.
  - Integração de hardware físico (sensores na protoboard) com banco de dados em nuvem via Wi-Fi.

---

## 🎯 Objetivos

### Objetivo Geral

Desenvolver um protótipo físico e funcional de baixo custo para monitorar vagas de estacionamento em tempo real, informando a disponibilidade ao motorista via interface visual.

### Objetivos Específicos

1. [x] Planejar e Definir Componentes: Selecionar microcontroladores (ESP32/Arduino), sensores ultrassônicos baratos, banco de dados gratuito na nuvem e ferramentas visuais para o app.
2. [x] Montar e Programar o Back-end: Montar o circuito físico na placa de testes (protoboard), programar a leitura de presença e o envio de dados via Wi-Fi.
3. [ ] Criar o Aplicativo/Site (Front-end): Desenvolver uma interface direta (via Thunkable, App Inventor ou HTML/CSS) conectada ao banco de dados para alterar as cores do mapa (verde para livre, vermelho para ocupada).
4. [ ] Realizar Testes Práticos: Avaliar na bancada da escola, usando maquetes, a precisão da detecção de distância e a velocidade com que a cor muda na tela.

---

## 📐 Framework / Metodologia Adotada

### Framework de Governança

| Framework | Versão | Processos/Domínios Utilizados |
|-----------|--------|-------------------------------|
| **Prototipagem Ágil de IoT** | **1.0** | **Concepção, Montagem em Bancada, Integração Cloud e Validação** |

### Práticas / Processos Aplicados

| Prática / Processo | Aplicação no Projeto |
|--------------------|---------------------|
| ESP32 ou Arduino | Microcontrolador central para processamento dos sensores e comunicação Wi-Fi com a internet (Back-end). |
| Sensor Ultrassônico | Leitura de presença física para identificar se há um carrinho na vaga. |
| Thunkable / App Inventor | Ferramentas visuais gratuitas para a criação da interface do aplicativo (Front-end) do motorista. |
| Banco de Dados Cloud | Estrutura de banco de dados gratuito na nuvem para armazenar a informação de "vaga livre" ou "vaga ocupada" e integrá-la ao mapa. |

### Metodologia de Pesquisa

- **Tipo:** Pesquisa aplicada.
- **Abordagem:** Qualitativa e Quantitativa (testes de funcionalidade e medição de tempo de resposta).
- **Coleta de dados:** Testes práticos manuais feitos na bancada da escola usando carrinhos de brinquedo e maquetes.
- **Ferramentas:** Protoboard, IDE do Arduino, sensores ultrassônicos, banco de dados em nuvem.

---

## 🔲 Escopo e Delimitações

### ✅ Dentro do Escopo

- Montagem do hardware na placa de testes (protoboard) com sensores ultrassônicos.
- Programação do microcontrolador para envio de dados de status para a internet via Wi-Fi.
- Criação de uma interface de usuário simples com mudança automática de cores (Verde/Vermelho).
- Testes práticos avaliando erro de distância na detecção e a velocidade de mudança de cor no celular.

### ❌ Fora do Escopo

- Implementação física em um estacionamento real (projeto restrito à bancada e maquetes).
- Desenvolvimento de sistema de pagamentos automáticos ou reserva antecipada de vagas.

### ⚠️ Premissas e Restrições

- **Premissa 1:** A escola disponibiliza a bancada e infraestrutura básica de rede para conectar o microcontrolador via Wi-Fi.
- **Restrição 1:** O projeto deve priorizar a economia estrita, utilizando apenas componentes acessíveis e ferramentas de software gratuitas.

---

## 📦 Entregáveis

| # | Entregável | Formato | Localização | Status |
|---|-----------|---------|-------------|--------|
| 1 | Documento de Arquitetura e Planejamento | MD | `docs/01-documento-arquitetura.md` | ✅ Concluído |
| 2 | Circuito eletrônico montado em protoboard | Físico | `Físico (Bancada)` | 🔄 Em Andamento |
| 3 | Código-fonte do Microcontrolador (Back-end) | .ino / C++ | `src/backend/` | 🔄 Em Andamento |
| 4 | Aplicativo Front-end integrado ao banco de dados | App/APK | `src/frontend/` | ⬜ Pendente |
| 5 | Relatório de Testes Práticos e Validação | MD | `docs/05-relatorio-testes.md` | ⬜ Pendente |

---

## 📅 Cronograma

| Fase | Atividade | Início | Fim | Status |
|------|-----------|--------|-----|--------|
| 1 | Planejamento e Escolha dos Componentes | 01/08/2026 | 15/08/2026 | ✅ Concluído |
| 2 | Montagem do Circuito e Programação (Back-end) | 16/08/2026 | 30/09/2026 | 🔄 Em Andamento |
| 3 | Criação do Aplicativo/Site (Front-end) | 01/10/2026 | 31/10/2026 | ⬜ Pendente |
| 4 | Testes Práticos na Bancada da Escola | 01/11/2026 | 15/11/2026 | ⬜ Pendente |
| 5 | Análise de Resultados e Documentação Final | 16/11/2026 | 30/11/2026 | ⬜ Pendente |

---

## 📁 Estrutura do Repositório


---
tcc-gov-ti-monitoramento-vagas/
│
├── README.md                       # ← Você está aqui
│
├── docs/
│   ├── 01-documento-arquitetura.md # Arquitetura e planejamento
│   └── 05-relatorio-testes.md      # Resultados da validação
│
├── src/
│   ├── backend/                    # Código-fonte do ESP32/Arduino (.ino)
│   └── frontend/                   # Código/projeto do aplicativo
│
└── maquete/
└── esquema-e-fotos.md          # Fotos e detalhes da bancada de testes


---

## 🧭 Como Navegar este Projeto

| Eu quero... | Vá para... |
|-------------|-----------|
| Entender o projeto em 2 min | Leia o [Resumo](#-sobre-o-projeto) e os [Objetivos](#-objetivos) |
| Ver o problema e os dados | Seção [Problema e Justificativa](#-problema-e-justificativa) |
| Consultar o código Back-end | `src/backend/` |
| Ver a interface Front-end | `src/frontend/` |
| Analisar os testes práticos | `docs/05-relatorio-testes.md` |

---

## 📊 Resultados e Conclusões

### Principais Resultados Esperados

| Métrica | Meta Projetada |
|---------|----------------|
| Precisão do Sensor Ultrassônico | 100% de acerto na detecção do carrinho de brinquedo na distância estipulada na maquete. |
| Velocidade de Resposta na Tela | Mudança da cor no celular em menos de 2 segundos após a colocação do objeto na vaga. |
| Custo Total de Componentes | Inferior a R$ 100,00 por vaga monitorada. |

### Conclusões

*(Seção a ser consolidada após a Etapa 4 dos Testes Práticos na Bancada da Escola)*

---

## 📚 Referências

> Formato ABNT (NBR 6023:2018) — ordem alfabética.

1. MONK, Simon. **Programação com Arduino: com orçamentos fáceis e baratos**. Porto Alegre: Bookman, 2017.
2. SPERINSKI, Cezar. **Internet das Coisas com ESP32 e Arduino**. São Paulo: Editora Erica, 2020.

---

## 📖 Glossário de Termos Técnicos

> Termos utilizados neste TCC para consulta rápida.

<details open>
<summary><strong>Termos do Projeto</strong></summary>

| Termo | Definição (no contexto deste projeto) |
|-------|---------------------------------------|
| **IoT** | Internet das Coisas – conexão de objetos físicos à internet. |
| **ESP32** | Microcontrolador de baixo custo com Wi-Fi e Bluetooth integrados. |
| **Sensor Ultrassônico** | Dispositivo que mede distâncias através de ondas sonoras (HC-SR04). |
| **Protoboard** | Placa de ensaio usada para montagem de circuitos eletrônicos sem solda. |
| **Back-end** | Lógica de programação executada no microcontrolador e na nuvem. |
| **Front-end** | Interface visual do aplicativo acessada pelo motorista. |

</details>

---

## 👥 Equipe

| Nome | RA | Função | Contato |
|------|-----|--------|---------|
| {{Nome do Aluno 1}} | {{RA}} | Desenvolvimento Hardware | {{email@etec.sp.gov.br}} |
| {{Nome do Aluno 2}} | {{RA}} | Desenvolvimento Software | {{email@etec.sp.gov.br}} |

**Docente:** Prof. Taina Barros — {{email@etec.sp.gov.br}}

---

## 📄 Licença

Este trabalho é de natureza acadêmica e foi desenvolvido como requisito parcial para conclusão do curso de **Manutenção e Suporte em Informática** na disciplina de **Governança de TI** na **ETEC Jaraguá**.

© 2026 ETEC Jaraguá — Todos os direitos reservados.

---

<details>
<summary>📝 <strong>Checklist de Entrega (uso interno da equipe)</strong></summary>

### Documentação
- [x] Documento de Arquitetura e Planejamento
- [ ] Relatório de Testes Práticos e Validação

### Artefatos Técnicos
- [ ] Circuito eletrônico montado em protoboard
- [ ] Código-fonte do Microcontrolador (Back-end)
- [ ] Aplicativo Front-end integrado ao banco de dados

### Apresentação
- [ ] Roteiro dos slides da defesa
- [ ] Ensaio da apresentação realizado

</details>
