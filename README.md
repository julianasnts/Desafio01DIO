## <img align="center" width="40px" src="https://hermes.digitalinnovation.one/assets/diome/logo-minimized.png"> Este repositório foi criado como parte dos estudos e desafios do **Santander Code Girls**

## Sobre o Projeto

Este projeto demonstra a implementação de uma arquitetura de nuvem funcional na **Amazon Web Services (AWS)**, integrando quatro serviços fundamentais: **EC2, EBS, S3 e Lambda**. O objetivo foi construir uma solução coesa, desde o provisionamento de um servidor web até a automação de tarefas com uma função serverless.

Este laboratório prático foi desenvolvido como parte do **Bootcamp Santander | DIO**.

# Projeto de Integração de Serviços Essenciais AWS

![Amazon EC2](https://img.shields.io/badge/Amazon%20EC2-FF9900?style=flat-square&logo=amazon-ec2&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=flat-square&logo=amazon-s3&logoColor=white)
![AWS Lambda](https://img.shields.io/badge/AWS%20Lambda-FF9900?style=flat-square&logo=aws-lambda&logoColor=white)
![Amazon EBS](https://img.shields.io/badge/Amazon%20EBS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

## 🏗️ Arquitetura da Solução

A solução foi desenhada da seguinte forma:

1.  **Aplicação**: Um servidor web (Apache/Nginx) é executado em uma instância **EC2**, servindo como a camada de computação principal.
2.  **Armazenamento Persistente**: Um volume **EBS** é anexado à instância EC2 para garantir que os dados da aplicação persistam independentemente do ciclo de vida da instância.
3.  **Armazenamento de Objetos**: Um bucket **S3** é utilizado para armazenar e versionar arquivos estáticos (como imagens e documentos) de forma segura e escalável.
4.  **Automação Serverless**: Uma função **Lambda** em Python é acionada por eventos no S3 (ex: upload de um novo objeto), processando o arquivo e registrando logs no CloudWatch, demonstrando uma arquitetura orientada a eventos.

## 🛠️ Funcionalidades Implementadas

-   **Provisionamento de Servidor Web**: Instância EC2 com Amazon Linux 2, configurada com Security Groups para acesso HTTP e SSH.
-   **Armazenamento em Bloco Persistente**: Volume EBS de 8 GiB acoplado e montado na instância, garantindo a durabilidade dos dados.
-   **Repositório de Objetos Versionado**: Bucket S3 configurado com controle de versionamento e políticas de acesso para uploads seguros.
-   **Gatilho de Automação com Lambda**: Função serverless que reage a uploads no S3, executando código sob demanda sem gerenciamento de servidores.

## 🎨 Diagrama da Arquitetura

O diagrama da solução foi desenvolvido no **Draw.io**, com algumas personalizações para alcançar um visual mais moderno e profissional:

-   **Ícones**: Para garantir a clareza, utilizei a biblioteca de ícones oficiais da AWS em vez dos padrões da ferramenta.
-   **Cores**: Optei por um fundo escuro para melhor contraste, aplicando a paleta de cores personalizada da AWS (como o laranja e o azul) para destacar os serviços.
-   **Layout**: A organização dos elementos, setas e fontes foi ajustada para criar um fluxo intuitivo e facilitar a compreensão da arquitetura.

## 📸 Evidências

Os screenshots que comprovam a implementação e o funcionamento de cada etapa da arquitetura estão neste repositório.

## ✅ Principais Aprendizados

A execução deste desafio solidificou o entendimento sobre como orquestrar diferentes serviços da AWS para criar soluções robustas. As principais competências exercitadas foram:

-   **Computação em Nuvem (IaaS)**: Gerenciamento completo de instâncias EC2.
-   **Estratégias de Armazenamento**: Diferenciação e aplicação de EBS (bloco) e S3 (objeto).
-   **Arquitetura Serverless**: Implementação de lógica de negócios com Lambda de forma eficiente e escalável.
-   **Segurança e Redes**: Configuração de Security Groups e políticas de acesso em buckets.

## 🔗 Links Úteis

-   [Documentação AWS EC2](https://docs.aws.amazon.com/ec2/)
-   [Documentação AWS EBS](https://docs.aws.amazon.com/ebs/)
-   [Documentação AWS S3](https://docs.aws.amazon.com/s3/)
-   [Documentação AWS Lambda](https://docs.aws.amazon.com/lambda/)

-   ## ✨ Autor

- [Ariana Eger](https://github.com/arisgerr)

### 🔗 Desafio proposto por [Digital Innovation One - DIO](https://www.dio.me/)
