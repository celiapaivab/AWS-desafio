# Gerenciamento de Instâncias EC2 na AWS

Este repositório foi criado como parte do desafio de consolidação de conhecimentos em **Amazon EC2**, com foco em gerenciamento de instâncias na AWS. Ele reúne **anotações** e o **diagrama em Draw.io** desenvolvido durante as aulas.

## Conteúdo do Repositório

- `README.md` → anotações e explicações detalhadas.
- `Desafio.drawio` → diagrama elaborado com base no conteúdo do curso.

## Conceitos Principais

### O que é o Amazon EC2?

- **Elastic Compute Cloud (EC2)** são as máquinas virtuais da AWS.
- Composta por **CPU, memória, disco, rede e sistema operacional**.
- Faz parte do modelo **IaaS (Infraestrutura como Serviço)**.
- AWS cuida do hardware e da virtualização.
- Responsabilidade do usuário: **aplicativos, dados, configurações de rede e conexões**.

### Terminologia Importante

- **AMI (Amazon Machine Image):** imagem base usada para criar instâncias.
- **Security Groups:** firewall virtual que controla tráfego de entrada e saída.
- **Instância:** unidade de computação criada a partir de uma AMI.

### Como Escolher a Instância Correta

- Basear a escolha nas **necessidades da aplicação**.
- Considerar **eficiência, escalabilidade e custo**.
- Avaliar **CPU, memória, storage e rede** necessários.

### Otimização de Recursos

- **Desligar instâncias não utilizadas:** ideal para ambientes de teste/dev.
- **Remover recursos ociosos:** evitar gastos desnecessários.
- **Escalar recursos:**
    -   **Vertical:** aumentar/reduzir CPU, RAM, storage em uma instância.
    -   **Horizontal:** adicionar/remover instâncias para suportar a aplicação.

### Modelos de Compra de Instâncias

- **Sob Demanda:** paga por hora; ideal para testes e cargas
    variáveis.
- **Reservadas:** mais baratas, mas exigem compromisso anual.
- **Spot:** até 90% de desconto, mas podem ser encerradas pela AWS a
    qualquer momento.

### Armazenamento na Nuvem

- **Amazon S3 (Simple Storage Service):** armazenamento de objetos, seguro e escalável.
    - Classes de armazenamento otimizadas por custo.
    - É barato, seguro e escalável.
    - Dados antigos podem ir para o Glacier (muito barato, mas lento para acessar).
- **Amazon EBS (Elastic Block Store):** armazenamento em blocos anexado a instâncias EC2.
    - Ideal para bancos de dados, logs ou arquivos de aplicação.
    - Dá para aumentar ou diminuir conforme a necessidade.

## Insights Pessoais

- EC2 é como se fossem máquinas virtuais que você pode “alugar” na AWS, é como ligar um computador novo, só que na nuvem.
- Fazer escolha correta da instância para gastar menos e ter melhor desempenho.
- Desligar instâncias quando não estiver usando e remover recursos ociosos para diminuir os custos.
- O EBS é como um HD externo conectado ao seu computador.
- O S3 guarda seus objetos em caixas chamadas buckets.

## Diagrama do Desafio

O diagrama em Draw.io está incluído neste repositório: `Desafio.drawio`

## Referências

- Material do curso **Santander Code Girls - 2025**.
- [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/)
- [AWS S3 Storage Classes](https://aws.amazon.com/pt/s3/storage-classes/)
