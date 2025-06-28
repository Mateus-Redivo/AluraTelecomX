# 📊 Challenge Alura - Análise de Evasão TelecomX

## 🎯 Sobre o Projeto

Este projeto foi desenvolvido como parte do **Challenge Alura** e consiste em uma análise completa de evasão de clientes (Customer Churn) para a empresa fictícia **TelecomX Brasil**, uma operadora de telecomunicações.

O objetivo principal é identificar padrões comportamentais e características demográficas dos clientes que cancelam seus serviços, fornecendo insights acionáveis para estratégias de retenção.

## 📁 Estrutura do Projeto

```
├── README.md                    # Este arquivo
├── TelecomX_BR.ipynb           # Notebook principal com análise completa
├── TelecomX_Data.json          # Dataset original em formato JSON
└── TelecomX_dicionario.md      # Dicionário de dados
```

## 🚀 Principais Resultados

### 📈 Métricas Chave Descobertas
- **Taxa de Evasão:** 26.5% (1.869 de 7.043 clientes)
- **Receita Perdida Anual:** R$ 1.669.571,52
- **Perfil Crítico:** Clientes com fibra óptica sem serviços complementares
- **Janela Crítica:** Primeiros 18 meses são determinantes para retenção

### 🔍 Insights Principais
1. **Paradoxo da Fibra Óptica:** 41.9% de evasão (maior que DSL: 18.8%)
2. **Poder dos Serviços Complementares:** Segurança online reduz evasão em 65%
3. **Impacto Demográfico:** Idosos e pessoas sem vínculos familiares apresentam maior risco
4. **Valor dos Clientes Perdidos:** Clientes que saem pagam 21.5% mais que os fiéis

## 🛠️ Tecnologias Utilizadas

### Linguagens e Bibliotecas
- **Python 3.x**
- **Pandas** - Manipulação e análise de dados
- **NumPy** - Computação numérica
- **Matplotlib** - Visualização de dados
- **Seaborn** - Visualizações estatísticas avançadas

### Ferramentas
- **Jupyter Notebook** - Ambiente de desenvolvimento
- **JSON** - Formato de dados de entrada

## 📊 Metodologia

### 1. 📌 Extração (Extract)
- Carregamento de dados JSON aninhados
- 7.043 registros de clientes com múltiplas dimensões

### 2. 🔧 Transformação (Transform)
- **Normalização de dados aninhados** usando `pd.json_normalize()`
- **Limpeza da variável target** (Churn: Yes/No → 1/0)
- **Otimização de tipos de dados** para eficiência
- **Criação de variáveis derivadas:**
  - `Contas_Diarias`: Valor diário calculado
  - `tenure_category`: Categorização do tempo de relacionamento

### 3. 📊 Carga e Análise (Load)
- **Análise exploratória completa**
- **Visualizações interativas**
- **Segmentação de clientes por risco**
- **Cálculo de impacto financeiro**

## 📈 Principais Análises Realizadas

### 1. Análise Demográfica
- Evasão por gênero, idade, status familiar
- Identificação de grupos de risco

### 2. Análise Temporal
- Impacto do tempo de relacionamento (tenure)
- Identificação da "barreira dos 18 meses"

### 3. Análise de Serviços
- Performance por tipo de internet
- Impacto de serviços complementares
- Análise de streaming e suporte técnico

### 4. Análise Financeira
- Cálculo de receita perdida
- Perfil de valor dos clientes evadidos
- Projeções de impacto

## 🎯 Segmentação de Risco Identificada

### 🔴 Alto Risco (73.7% evasão)
- **Perfil:** Fibra + Sem Segurança + Sem Suporte + Sem Parceiro
- **Quantidade:** 213 clientes
- **Ação:** Intervenção imediata

### 🟡 Médio Risco (47.8% evasão)
- **Perfil:** Novos clientes (<12 meses) + Sem Dependentes
- **Quantidade:** 906 clientes
- **Ação:** Programa de onboarding intensivo

### 🟢 Baixo Risco (6.3% evasão)
- **Perfil:** Clientes antigos (>36 meses) + Com Dependentes
- **Quantidade:** 1.182 clientes
- **Ação:** Programa de advocacy

## 💡 Recomendações Implementadas

### 🚨 Ações Imediatas (0-30 dias)
1. **Programa Emergencial Fibra Óptica**
2. **Retenção Ativa para Alto Risco**
3. **Segurança Online Gratuita** para clientes críticos

### 📈 Melhorias Estruturais (30-90 dias)
1. **Programa "Primeiros 18 Meses"**
2. **Pacotes Segmentados** por perfil
3. **Canais de Suporte Dedicados**

### 🔮 Estratégias de Longo Prazo (90+ dias)
1. **Programa de Fidelidade "TelecomX+"**
2. **Transformação Digital** com IA
3. **Parcerias Estratégicas**

## 📊 ROI Esperado

- **Redução de Churn:** De 26.5% para 20%
- **Economia Anual:** R$ 1.085.871
- **Investimento Total:** R$ 500.000
- **ROI:** 217% no primeiro ano
- **Payback:** 5.5 meses

## 🚀 Como Executar o Projeto

### Pré-requisitos
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Execução
1. Clone ou baixe este repositório
2. Abra o Jupyter Notebook:
   ```bash
   jupyter notebook TelecomX_BR.ipynb
   ```
3. Execute as células sequencialmente

### Estrutura do Notebook
- **Extração:** Carregamento dos dados JSON
- **Transformação:** Limpeza e preparação dos dados
- **Análise:** Exploração completa dos dados
- **Relatório Final:** Conclusões e recomendações

## 📋 Dados Utilizados

### Fonte
- **Arquivo:** `TelecomX_Data.json`
- **Registros:** 7.043 clientes
- **Período:** Dados históricos de telecomunicações

### Principais Variáveis
- **customerID:** Identificação única
- **Churn:** Indicador de evasão (variável target)
- **Dados Demográficos:** Gênero, idade, estrutura familiar
- **Serviços:** Telefonia, internet, streaming, suporte
- **Financeiro:** Valores mensais e totais

## 🤝 Contribuições

Este projeto foi desenvolvido como parte do Challenge Alura. Contribuições e melhorias são bem-vindas!

### Como Contribuir
1. Fork o projeto
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Push para a branch
5. Abra um Pull Request

## 📞 Contato

Para dúvidas ou sugestões sobre este projeto, entre em contato!

## 📄 Licença

Este projeto está sob licença MIT. Veja o arquivo LICENSE para mais detalhes.

---

### 🏆 Principais Conquistas do Projeto

✅ **Análise Completa de Churn** com insights acionáveis  
✅ **ROI Projetado de 217%** com estratégias baseadas em dados  
✅ **Segmentação de Clientes** em 3 níveis de risco  
✅ **Identificação de R$ 1.67M** em receita recuperável  
✅ **Metodologia ETL** robusta para dados aninhados  
✅ **Visualizações Profissionais** para apresentação executiva  

---

