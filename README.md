# Spring Boot - Kubernetes

Este é um projeto simples que utiliza o Spring Boot para criar uma API e o Kubernetes para orquestrar a implantação da aplicação. A aplicação consiste em um serviço web RESTful desenvolvido com o Spring Boot, que fornece endpoints para interagir com recursos específicos.

O Kubernetes é utilizado para gerenciar o ciclo de vida da aplicação. Neste projeto, um Deployment foi configurado para criar e manter 5 réplicas da aplicação em execução para garantir a alta disponibilidade e escalabilidade horizontal.

## Funcionalidades

- Implementação de uma API RESTful usando Spring Boot.
- Implantação automatizada no Kubernetes com 5 réplicas.

## Instruções de Uso

### Pré-requisitos

Para executar este projeto, é necessário ter as seguintes ferramentas instaladas:

- [Kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- [Minikube](https://minikube.sigs.k8s.io/docs/start/) ou [Kind](https://kind.sigs.k8s.io/docs/user/quick-start/)
- [Docker](https://docs.docker.com/get-docker/)
- Maven

### Instalação e Implantação

1. Clone este repositório:

    ```bash
    git clone https://github.com/GabrielMorais2/springboot-k8s-app.git
    ```

2. Build do projeto:

    ```bash
    cd spring-k8s-app
    mvn clean package
    ```

3. Crie o Deployment e Serivce no Kubernetes:

    ```bash
    kubectl apply -f deployment.yaml
    kubectl apply -f service.yaml
    ```

## Contribuindo

Sinta-se à vontade para abrir um pull request ou relatar um problema.

## Licença

Este projeto é licenciado sob a [Licença MIT](https://opensource.org/licenses/MIT).
