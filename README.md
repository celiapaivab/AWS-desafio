# 🚀 Gerenciamento de Instâncias EC2 na AWS

Este repositório foi criado como parte do desafio de consolidação de
conhecimentos em **Amazon EC2**, com foco em gerenciamento de instâncias
na AWS. Ele reúne **anotações, insights práticos** e o **diagrama em
Draw.io** desenvolvido durante as aulas.

## 📑 Conteúdo do Repositório

-   `README.md` → anotações e explicações detalhadas.\
-   `Desafio.drawio` → diagrama elaborado com base no conteúdo do curso.

## 📘 Conceitos Principais

### 🔹 O que é o Amazon EC2?

-   **Elastic Compute Cloud (EC2)** são as máquinas virtuais da AWS.\
-   Composta por **CPU, memória, disco, rede e sistema operacional**.\
-   Faz parte do modelo **IaaS (Infraestrutura como Serviço)**.\
-   Responsabilidade do usuário: **aplicativos, dados e conexões**.

### 🔹 Terminologia Importante

-   **AMI (Amazon Machine Image):** imagem base usada para criar
    instâncias.\
-   **Security Groups:** firewall virtual que controla tráfego de
    entrada e saída.\
-   **Instância:** unidade de computação criada a partir de uma AMI.

### 🔹 Como Escolher a Instância Correta

-   Basear a escolha nas **necessidades da aplicação**.\
-   Considerar **eficiência, escalabilidade e custo**.\
-   Avaliar **CPU, memória, storage e rede** necessários.

### 🔹 Otimização de Recursos

-   **Desligar instâncias não utilizadas:** ideal para ambientes de
    teste/dev.\
-   **Remover recursos ociosos:** evitar gastos desnecessários.\
-   **Escalar recursos:**
    -   **Vertical:** aumentar/reduzir CPU, RAM, storage em uma
        instância.\
    -   **Horizontal:** adicionar/remover instâncias para suportar a
        aplicação.

### 🔹 Modelos de Compra de Instâncias

-   **Sob Demanda:** paga por hora; ideal para testes e cargas
    variáveis.\
-   **Reservadas:** mais baratas, mas exigem compromisso anual.\
-   **Spot:** até 90% de desconto, mas podem ser encerradas pela AWS a
    qualquer momento.

### 🔹 Armazenamento na Nuvem

-   **Amazon S3:** armazenamento de objetos, seguro e escalável.
    -   Classes de armazenamento otimizadas por custo.\
    -   Regras de ciclo de vida (Lifecycle) para mover dados para
        Glacier.\
-   **Amazon EBS:** armazenamento em blocos anexado a instâncias EC2.
    -   Ex.: bancos de dados, logs, dados de apps.

## 📝 Insights Pessoais

-   A escolha correta da instância impacta diretamente em **custos e
    performance**.\
-   O uso de **escala automática** é essencial para lidar com variações
    de demanda.\
-   **Gerenciamento de custos** (desligar instâncias, usar
    Spot/Reservadas) é tão importante quanto o desempenho.

## 📊 Diagrama do Desafio

O diagrama em Draw.io está incluído neste repositório:\
👉 `Desafio.drawio`

## 📚 Referências

-   Material do curso **Amazon EC2 -- AWS Cloud Foundations**.\
-   [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/)\
-   [AWS S3 Storage
    Classes](https://aws.amazon.com/pt/s3/storage-classes/)
