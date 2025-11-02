### PT-BR

# 🚀 Projeto Completo de Azure Databricks

Este projeto foi **desenvolvido por mim com foco em cenários reais de Engenharia de Dados**, utilizando o **Azure Databricks** como plataforma principal.  
O objetivo foi criar uma solução **end-to-end (E2E)** totalmente funcional — cobrindo desde a **ingestão e transformação de dados** até a **modelagem dimensional e integração com ferramentas de BI**, aplicando **boas práticas de governança, segurança e performance**.

---

## 🧠 Objetivo do Projeto
Desenvolver uma **pipeline de dados completa** que reflita o que é feito em **ambientes corporativos reais**, explorando todos os recursos modernos do ecossistema Databricks.  
Este projeto também foi criado para **reforçar meus conhecimentos técnicos** e servir como **prova prática de domínio em Engenharia de Dados**, especialmente para entrevistas técnicas em 2025.

---

## 🧱 Arquitetura e Fluxo de Dados

A arquitetura segue o padrão **Medallion (Bronze → Silver → Gold)**, garantindo modularidade, rastreabilidade e governança em todas as etapas.

### **1. Preparação e Governança**
- Criei uma conta gratuita no **Azure** e configurei o **Azure Data Lake Storage (ADLS)** como camada de armazenamento.  
- Configurei o **Unity Catalog** para gerenciar credenciais, metadados e segurança, seguindo as melhores práticas do Databricks.  
- Trabalhei com o formato **Parquet**, visando performance e eficiência no processamento.

---

### **2. Camada Bronze (Ingestão)**
- Implementei a ingestão incremental usando **Spark Structured Streaming** com o **Autoloader**.  
- Configurei **checkpoint locations** para garantir idempotência e processamento “exactly once”.  
- Armazenei os dados brutos em formato **Delta Lake**, permitindo versionamento e transações ACID.  

---

### **3. Camada Silver (Transformação)**
- Apliquei **transformações em PySpark** usando conceitos de **Programação Orientada a Objetos (POO)** para aumentar a modularidade do código.  
- Desenvolvi **funções reutilizáveis** e as registrei no **Unity Catalog**, de forma semelhante a funções SQL persistentes.  
- Realizei a padronização e limpeza dos dados, garantindo qualidade e consistência antes da modelagem.

---

### **4. Camada Gold (Modelagem Dimensional)**
- Modelei um **Star Schema completo**, contendo tabelas de **Dimensões e Fatos**.  
- Implementei **SCD Tipo 1 (Upsert)** com `MERGE INTO` para atualizar e inserir registros.  
- Criei **SCD Tipo 2 (Histórico)** utilizando **Delta Live Tables (DLT)**, configurando **Expectations** para controle e qualidade dos dados.  

---

### **5. Consumo e Visualização**
- Disponibilizei os dados através do **SQL Warehouse (Lakehouse)** para consultas otimizadas.  
- Conectei o projeto ao **Power BI** via **Partner Connect**, criando dashboards dinâmicos com dados em tempo real.  

---

## ⚙️ Tecnologias Utilizadas
- **Azure Databricks (Runtime, DLT, SQL Warehouse)**  
- **Azure Data Lake Storage (ADLS)**  
- **Unity Catalog**  
- **PySpark / Python (POO)**  
- **Delta Lake (ACID Transactions)**  
- **Power BI**  

---

## 🎯 Conceitos Abordados
- Arquitetura **Medallion (Bronze, Silver, Gold)**  
- **Ingestão incremental e streaming**  
- **Idempotência e Exactly Once Processing**  
- **Modelagem Dimensional (Star Schema)**  
- **Slowly Changing Dimensions (SCD Tipo 1 e 2)**  
- **Delta Live Tables e Data Quality**  
- **Governança e segurança com Unity Catalog**  
- **Integração BI e consumo analítico**  

---

## 🧩 Resultado Final
O resultado é uma **pipeline de dados moderna, escalável e governada**, que representa o fluxo completo de dados em um **Data Lakehouse corporativo**.  
Ela realiza desde a ingestão automatizada até a modelagem dimensional, com **qualidade e controle histórico garantidos**.

---

## 💡 Meu Aprendizado
Durante o desenvolvimento, aprofundei meu conhecimento em:
- Estruturação de **camadas de dados** no Databricks;  
- Implementação de **cargas incrementais** e controle de histórico;  
- Uso prático de **Delta Live Tables**;  
- Boas práticas de **governança com Unity Catalog**;  
- Integração de **pipelines analíticos com Power BI**.  

Este projeto representa um marco importante na minha jornada para **dominar o Databricks e as práticas de Engenharia de Dados de nível enterprise**.  

---
