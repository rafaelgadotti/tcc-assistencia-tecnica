# 🔧 Assistência Técnica Inteligente: Diagnóstico de Falhas em Motores de Indução baseado em Análise Multimodal


> 
> *Plataforma web para otimização do fluxo de assistência técnica, atuando como suporte à decisão no diagnóstico de motores elétricos.*

![Status do Projeto](https://img.shields.io/badge/Status-Em_Desenvolvimento-10b981?style=for-the-badge)
![Linguagem Principal](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Frontend](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

---

## 📖 O Contexto e o Problema
No ambiente industrial, a agilidade no processo de garantia e assistência técnica é crítica para não paralisar linhas de produção. Atualmente, a triagem de falhas em muitas organizações é um processo manual, onde analistas internos revisam  fotos e descrições textuais enviadas por técnicos de campo.

Analisando as soluções de mercado modernas, nota-se que as abordagens baseadas em Inteligência Artificial dependem quase exclusivamente da instalação de sensores físicos (IoT) de vibração ou corrente nos equipamentos. Por outro lado, sistemas tradicionais de ordens de serviço atuam de forma passiva, baseados apenas em registros descritivos. Existe uma lacuna latente para soluções inteligentes que não demandem hardwares adicionais.

## 💡 A Proposta de Solução (Inovação)
Este projeto propõe o desenvolvimento de uma plataforma **Web Desktop** unificada que centraliza e automatiza a triagem de garantias. 

A inovação central reside na utilização de **Inteligência Artificial Multimodal**. O sistema analisa simultaneamente evidências visuais (fotos da avaria) utilizando Visão Computacional, e evidências textuais (relato do técnico) utilizando Processamento de Linguagem Natural (PLN).
A plataforma foi desenhada sob o paradigma **Human-in-the-Loop**. A máquina atua como um Sistema de Suporte à Decisão, gerando um pré-diagnóstico com o nível de confiança. O Analista Interno mantém o controle total, revisando as sugestões e emitindo o laudo técnico definitivo.

## 🚀 Escopo e Funcionalidades
O escopo técnico concentra-se no conjunto motriz, especificamente em **Motores de Indução**:

- **Triagem Assistida por IA:** Identificação de falhas visuais e textuais exclusivas de motores (ex: danos em estatores, bobinagens, carcaças e rolamentos).
- **Extração de Dados:** Importação e leitura automática de relatórios externos.
- **Interface de Validação:** Painel de controle para o analista interno comparar as evidências de campo com o diagnóstico da máquina.
- **Automação Documental:** Geração e exportação automatizada do laudo técnico oficial estruturado em PDF.
- **Gestão de Acesso:** Autenticação e hierarquia de usuários (Analistas e Administradores).
- **Dashboards Analíticos:** Visualização de volumetria de falhas, métricas de garantia e taxa de concordância da IA.

## 🛠️ Arquitetura e Stack Tecnológica
A arquitetura do software segue o padrão de **Monolito Modular em Camadas**, garantindo alta escalabilidade, isolamento de regras de negócio e viabilidade para ambientes corporativos reais:

- **Frontend (Interface do Usuário):** - React.js (via Vite) para alta reatividade.
  - Estilização corporativa moderna com Tailwind CSS.
- **Backend (Regras e APIs Internas):** - Python com o framework FastAPI, focado em alta performance e requisições assíncronas.
- **Banco de Dados:** - PostgreSQL (armazenamento relacional seguro do histórico de laudos) manipulado via ORM (SQLAlchemy).
- **Inteligência Artificial (Modelos 100% Locais):** - *Visão Computacional:* FastAI / PyTorch (Transfer Learning) para análise das avarias mecânicas.
  - *Linguagem Natural:* Scikit-Learn ou modelos SLM (Ollama) para interpretação dos relatos técnicos.
  - *Nota Arquitetural:* Não há dependência de APIs comerciais ou de terceiros (como OpenAI), garantindo custo zero de inferência e sigilo total dos dados industriais.

---

**Rafael Gadotti** *Estudante de Engenharia de Software* Católica SC - Centro Universitário (Jaraguá do Sul - SC)
