# Code_Girls-Gerenciando_Instancias_EC2_na_AWS
Desafio do Curso da DIO: Santander Code Girls - 2025, Módulo Gerenciando Instâncias EC2 na AWS

Este repositório contém a anotações e insights adquiridos durante a as aulas e atividades do curso.

---

## Objetivo do Desafio

Demonstrar o conhecimento sobre:
- Aplicar os conceitos aprendidos em um ambiente prático; 
- Documentar processos técnicos de forma clara e estruturada;
- Utilizar o GitHub como ferramenta para compartilhamento de documentação técnica.

---

## 🧭 Principais Funcionalidades e Passos

### 1. Visualização de AMIs e Instâncias  
- No AWS Explorer, expanda o nó **Amazon EC2**. 
- Para ver AMIs: clique no sub-nó **AMIs**, menu de contexto → “View”.
- Para ver instâncias: clique em sub-nó **Instâncias**, menu de contexto → “View”. 
- Você pode personalizar colunas, aplicar filtros, e usar tags para organização. 

### 2. Iniciando (Launching) uma instância EC2  
- Na visualização de AMIs, selecione uma AMI, menu de contexto → **Launch Instance**.
- Na caixa de diálogo “Launch New Amazon EC2 Instance”, defina:  
  - Tipo da instância (por ex., t2.micro)  
  - Nome da instância  
  - Par de chaves (key pair) ou opção de criar uma nova  
  - Grupo de segurança com as portas necessárias (ex: RDP/3389 para Windows)
- Clique em Launch. Depois, na visualização de instâncias, clique em Refresh para ver a nova instância no estado “running”. 

### 3. Conectando-se à instância  
- Para instâncias Windows: clique com o botão direito na instância → **Open Remote Desktop**. 
- Se necessário, use a opção **Get Windows Password** para recuperar a senha do administrador. 
- Você deve ter acesso ao par de chaves (.pem) ou à senha para autenticação.

### 4. Parar ou Encerrar Instâncias  
- Para **parar** a instância (stop): na visualização de instâncias, selecione a instância → menu de contexto → **Stop** → confirme. Dados no EBS permanecem, instância não está mais sendo executada (mas armazenamento EBS ainda é cobrado). 
- Para **encerrar** (terminate): menu de contexto → **Terminate**. Dados no armazenamento local da instância serão perdidos. 
- Você também pode definir o comportamento de desligamento (Shutdown) para que a instância “pare” ou “encerre” quando uma operação de desligamento for executada dentro da instância.

---



