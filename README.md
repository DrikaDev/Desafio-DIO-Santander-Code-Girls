## 🚀 Desafio DIO - Santander Code Girls  

Neste desafio, criamos uma **arquitetura no Draw.io** para consolidar nosso conhecimento em **gerenciamento de instâncias EC2 na AWS**. 

O objetivo era projetar uma arquitetura simples utilizando os seguintes serviços:  

### 🟦 Amazon S3  
Serviço de **armazenamento de objetos**, usado para guardar arquivos (imagens, vídeos, backups etc).  
Ele também pode disparar eventos para outros serviços quando algo novo é enviado.  

### 🟨 AWS Lambda  
Serviço **serverless**, que executa funções automaticamente em resposta a eventos.  
Neste caso, pode ser disparado quando um arquivo novo chega ao **S3**.  

### 🟥 Amazon EC2  
Serviço de **máquinas virtuais (IaaS)** na AWS, onde podemos rodar aplicações, bancos de dados e APIs.  

### 🟫 Amazon EBS  
Armazenamento em bloco anexado ao **EC2**, funcionando como um **HD/SSD persistente** para guardar dados.  

---

## 📂 Arquitetura Criada

![Desafio_DIO](https://github.com/user-attachments/assets/1b669a86-58a0-4528-b443-4f7f159ff1ba)

## 🔗 Fluxo de funcionamento

1. 👤 O **usuário (1)** envia um **arquivo (2)** para o **Amazon S3 (3)**.  
2. 🤖 O **AWS Lambda (4)** é acionado automaticamente e processa o arquivo (ex: validação, transformação, extração de metadados).  
3. 💻 O resultado é enviado para a **instância EC2 (5)**, que utiliza o **EBS (6)** para armazenar dados ou rodar aplicações.  
4. 🌍 O **EC2 (5)** pode disponibilizar os dados/processamentos de volta para o **usuário final (7)** quando ele precisar acessar novamente o arquivo.  

---

## ✅ Conclusão

Esse desafio foi uma ótima forma de entender como integrar diferentes serviços da AWS para criar uma arquitetura simples utilizando:  

- **Armazenamento** (S3)  
- **Processamento sob demanda** (Lambda)  
- **Servidores escaláveis** (EC2)  
- **Armazenamento persistente** (EBS)  
