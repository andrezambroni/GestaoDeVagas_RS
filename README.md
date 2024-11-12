# Gestão de Vagas

Este repositório contém um sistema de gestão de vagas desenvolvido no curso da Rocketseat. O projeto é dividido em duas partes principais: Backend e Frontend.

## Tecnologias Utilizadas

### Backend
- **Java 17**
- **Spring Boot 3.1.4**
- **JUnit** para testes unitários
- **Docker** para containerização
- **PostgreSQL** como banco de dados
- **Prometheus** para monitoramento
- **Grafana** para visualização de métricas

### Frontend
- **Java 17**
- **Spring Boot 3.2.1**

## Estrutura do Projeto

### Backend
- `.github/workflows/prod.yml`: Configuração do GitHub Actions para CI/CD.
- `.mvn/wrapper`: Arquivos do Maven Wrapper.
- `.vscode/settings.json`: Configurações do Visual Studio Code.
- `config/prometheus.yml`: Configuração do Prometheus.
- `docker-compose.yml`: Configuração do Docker Compose para serviços como PostgreSQL, Prometheus e Grafana.
- `Dockerfile`: Dockerfile para construção da imagem do backend.
- `mvnw`, `mvnw.cmd`: Scripts do Maven Wrapper.
- `pom.xml`: Arquivo de configuração do Maven.
- `src/main/java/br`: Código fonte principal do backend.
- `src/test/java/br`: Testes unitários do backend.

### Frontend
- `.mvn/wrapper`: Arquivos do Maven Wrapper.
- `mvnw`, `mvnw.cmd`: Scripts do Maven Wrapper.
- `pom.xml`: Arquivo de configuração do Maven.
- `src/main/java/br`: Código fonte principal do frontend.
- `src/test/java/br`: Testes unitários do frontend.

## Configuração e Execução

### Backend
1. **Configuração do Ambiente**:
   - Certifique-se de ter o Docker e o Docker Compose instalados.
   - Configure as variáveis de ambiente necessárias.

2. **Construção e Execução**:
   - Para construir o projeto, execute:
     ```sh
     ./mvnw clean install
     ```
   - Para executar os serviços usando Docker Compose, execute:
     ```sh
     docker-compose up
     ```

### Frontend
1. **Configuração do Ambiente**:
   - Certifique-se de ter o Maven instalado.

2. **Construção e Execução**:
   - Para construir o projeto, execute:
     ```sh
     ./mvnw clean install
     ```
   - Para executar a aplicação, execute:
     ```sh
     ./mvnw spring-boot:run
     ```

## Testes

### Backend
Os testes unitários estão localizados em [CreateJobControllerTest.java](http://_vscodecontentref_/1). Para executar os testes, utilize o comando:
```sh
./mvnw test
