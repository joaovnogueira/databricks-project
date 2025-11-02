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

## ⚙️ Tecnologias Utilizadas
- **Azure Databricks (Runtime, DLT, SQL Warehouse)**  
- **Azure Data Lake Storage (ADLS)**  
- **Unity Catalog**  
- **PySpark / Python (POO)**  
- **Delta Lake (ACID Transactions)**  

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

Este projeto representa um marco importante na minha jornada para **dominar o Databricks e as práticas de Engenharia de Dados**.  

---

### EN

# 🚀 Complete Azure Databricks Project  

This project was **developed by me to simulate real-world Data Engineering scenarios** using **Azure Databricks** as the main platform.  
The goal was to build a **fully functional end-to-end (E2E) data pipeline** — covering everything from **data ingestion and transformation** to **dimensional modeling and BI integration** — while applying **best practices for governance, security, and performance**.

---

## 🧠 Project Objective
To develop a **complete enterprise-grade data pipeline** that reflects real corporate environments, leveraging all the modern features of the Databricks ecosystem.  
I created this project to **strengthen my technical expertise** and serve as **practical evidence of my proficiency in Data Engineering**, especially for **technical interviews in 2025**.

---

## 🧱 Architecture and Data Flow

The architecture follows the **Medallion pattern (Bronze → Silver → Gold)**, ensuring modularity, traceability, and strong data governance at every stage.

### **1. Preparation and Governance**
- Set up a free **Azure** account and configured **Azure Data Lake Storage (ADLS)** as the main data layer.  
- Configured **Unity Catalog** for credential management, metadata governance, and security, following real-world best practices.  
- Used **Parquet** as the base data format for performance and compression efficiency.  

---

### **2. Bronze Layer (Ingestion)**
- Implemented **incremental ingestion** using **Spark Structured Streaming** with the **Autoloader** feature.  
- Configured **checkpoint locations** to ensure idempotency and **exactly-once processing**.  
- Stored raw data in **Delta Lake** format to enable ACID transactions and version control.  

---

### **3. Silver Layer (Transformation)**
- Applied **PySpark transformations** using **Object-Oriented Programming (OOP)** principles to improve modularity.  
- Built **reusable functions** and registered them in **Unity Catalog**, similar to persistent SQL functions.  
- Standardized and cleansed the data to ensure quality and consistency before modeling.  

---

### **4. Gold Layer (Dimensional Modeling)**
- Designed a full **Star Schema**, including **Dimension** and **Fact** tables.  
- Implemented **SCD Type 1 (Upsert)** using `MERGE INTO` for updates and inserts.  
- Created **SCD Type 2 (Historical)** logic with **Delta Live Tables (DLT)**, and defined **Expectations** to enforce data quality.  

---

## ⚙️ Technologies Used
- **Azure Databricks (Runtime, DLT, SQL Warehouse)**  
- **Azure Data Lake Storage (ADLS)**  
- **Unity Catalog**  
- **PySpark / Python (OOP)**  
- **Delta Lake (ACID Transactions)**  

---

## 🎯 Key Concepts Covered
- **Medallion Architecture (Bronze, Silver, Gold)**  
- **Incremental and streaming ingestion**  
- **Idempotency and Exactly Once Processing**  
- **Dimensional Modeling (Star Schema)**  
- **Slowly Changing Dimensions (SCD Type 1 & Type 2)**  
- **Delta Live Tables and Data Quality**  
- **Data Governance and Security with Unity Catalog**  
- **BI Integration and Analytical Consumption**  

---

## 🧩 Final Outcome
The final result is a **modern, scalable, and fully governed data pipeline**, representing a complete data lifecycle within a **corporate-grade Data Lakehouse**.  
It performs automated ingestion, transformation, and dimensional modeling — ensuring **data quality, history tracking, and performance optimization**.

---

## 💡 What I Learned
Throughout the development, I deepened my understanding of:
- Structuring **data layers** within Databricks;  
- Implementing **incremental loads** and historical tracking;  
- Building **Delta Live Tables (DLT)** workflows;  
- Applying **Unity Catalog** for governance and reusability;  

This project marks an important milestone in my journey to **master Databricks and Data Engineering practices**.  


