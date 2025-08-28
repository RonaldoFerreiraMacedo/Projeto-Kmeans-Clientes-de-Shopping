# 🧠 Projeto Final - Segmentação de Clientes com K-Means  

## 📌 Objetivo  
Este projeto faz parte do **Módulo 33 - Modelos Avançados** e tem como objetivo aplicar **clustering (agrupamento)** para segmentação de clientes de um shopping center.  
Utilizamos o **K-Means** para identificar padrões de comportamento em relação à renda, idade e hábitos de consumo.  

---

## 📊 Dataset  
O dataset utilizado contém **200 clientes** e possui as seguintes variáveis:  

- **CustomerID** → Identificador único do cliente  
- **Gender** → Gênero do cliente  
- **Age** → Idade do cliente  
- **Annual Income (k$)** → Renda anual em milhares de dólares  
- **Spending Score (1-100)** → Score atribuído pelo shopping, baseado no comportamento de compra  

---

## 🛠️ Etapas do Projeto  

### 🔍 1. Exploração de Dados  
- Verificação de valores ausentes → *Não havia nulos*  
- Identificação de outliers com boxplots → *Distribuição sem outliers extremos*  
- Análise exploratória com gráficos para observar padrões  

### 🧹 2. Tratamento de Dados  
- **Encoding**: variável `Gender` convertida em numérica (`0 = Female`, `1 = Male`)  
- **Padronização**: aplicação de `StandardScaler` para evitar influência de escalas diferentes  

### 🤖 3. Modelagem (K-Means)  
- Aplicação do algoritmo **K-Means** com `k=2` (dois clusters principais observados)  
- Visualização dos clusters em gráficos 2D  
- Extração dos centróides e interpretação  

### 📈 4. Avaliação e Interpretação  
- **Cluster 0**: Clientes mais velhos, com score de gastos mais baixo  
- **Cluster 1**: Clientes mais jovens, com score de gastos elevado  

---

## 💡 Insights de Negócio  
- O **Cluster 1 (jovens com maior gasto)** é o público ideal para **ações de marketing mais agressivas**.  
- Podem ser realizadas campanhas exclusivas, eventos e promoções voltadas a esse perfil.  
- Já o **Cluster 0 (menor score de gastos)** pode receber campanhas de fidelização, descontos progressivos ou ações de engajamento para aumentar seu consumo.  

---

## 📂 Estrutura do Projeto  
