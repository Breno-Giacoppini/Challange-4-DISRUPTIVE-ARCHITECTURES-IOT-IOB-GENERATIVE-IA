# Sistema de Previsão de Estoque de Roupas com IA

Este repositório apresenta o **Sistema de Previsão de Estoque de Roupas com IA**, uma ferramenta projetada para otimizar o gerenciamento de estoque em operações de varejo. O sistema utiliza inteligência artificial para prever a demanda de produtos, evitando rupturas e excesso de estoque, e maximizando a eficiência operacional.

## Integrantes

- **Breno Giacoppini Câmara** - RM98695
- **Jaqueline Martins dos Santos** - RM551744
- **Mariana Bastos Esteves** - RM97510
- **Matheus Oliveira Macedo** - RM551155
- **Victor Freitas Silva** - RM99982

## Demonstração em Vídeo

Assista à demonstração no YouTube: [[Link para o vídeo](https://youtu.be/J-j5_O-lcaM)](https://youtu.be/J-j5_O-lcaM)

---

## 1. Demonstração da Versão Final do Projeto

O **Sistema de Previsão de Estoque de Roupas com IA** é um produto funcional que oferece previsões de demanda com base em dados históricos de vendas. Usuários podem inserir dados manualmente ou importar informações via arquivos CSV. A partir desses dados, o sistema gera previsões de demanda para períodos futuros, auxiliando lojistas e gestores de estoque na tomada de decisões estratégicas. Isso permite otimizar o estoque e reduzir desperdícios.

---

## 2. Autocrítica sobre o Processo de Desenvolvimento

### Aspectos Positivos

- **Organização Modular**: A estrutura modular facilitou a implementação e manutenção, permitindo adições e melhorias sem comprometer outras partes do sistema.
- **Flexibilidade de Uso**: O sistema atende a diferentes perfis de usuários, incluindo pequenas empresas, graças à opção de entrada manual e à importação de dados em massa.
- **Eficiência nas Previsões**: O modelo de IA demonstrou eficiência em identificar padrões gerais de vendas, ajudando na previsão de demanda para categorias de produtos específicas.

### Aspectos a Melhorar

- **Limitações na Escalabilidade**: A inserção manual de dados é viável para pequenos volumes, mas se mostrou ineficiente para operações maiores. Uma integração direta com sistemas de ERP ou inventário é essencial para aumentar a escalabilidade.
- **Precisão Variável do Modelo**: Em casos com dados limitados, o modelo apresentou dificuldades para gerar previsões precisas. Esse aspecto reforça a necessidade de explorar métodos complementares, especialmente para capturar sazonalidades e tendências temporais.

### Lições Aprendidas

- **Importância da Validação de Dados**: A qualidade das previsões é diretamente influenciada pela precisão dos dados inseridos, evidenciando a importância de validações rigorosas.
- **Iteração e Testes Constantes**: Testes contínuos ao longo do desenvolvimento possibilitaram ajustes rápidos, aumentando a confiabilidade do sistema.
- **Experimentação de Modelos Alternativos**: Avaliar diferentes algoritmos desde o início teria permitido identificar rapidamente modelos com melhor adequação aos dados específicos do projeto.

---

## 3. Planos para o Futuro do Projeto

### Expansão do Sistema

- **Integração com Sistemas de ERP e e-Commerce**: Automatizar a coleta de dados para evitar a inserção manual, aumentando a eficiência do sistema.
- **Previsões Sazonais**: Implementar a consideração de sazonalidade nas previsões, possibilitando uma análise mais precisa durante períodos de alta demanda, como datas festivas.
- **Dashboard Interativo**: Desenvolver um painel visual que mostre previsões e métricas de desempenho para facilitar a tomada de decisão.

### Melhorias de Precisão

- **Inclusão de Variáveis Externas**: Incorporar dados econômicos e demográficos no modelo para enriquecer as previsões e alcançar maior precisão.
- **Avaliação de Modelos Alternativos**: Explorar algoritmos adicionais para lidar com padrões de dados complexos e sazonalidade, aprimorando a acurácia do sistema.

---

## 4. Integração do Sistema de Previsão de Estoque com Disciplinas Envolvidas

1. **Mastering Relational and Non-Relational Database**
   - Na transição da terceira para a quarta entrega, foi adotado o MongoDB como banco de dados NoSQL. Essa escolha se deu pela flexibilidade e escalabilidade horizontal do MongoDB, que elimina a necessidade de esquemas rígidos e facilita a recuperação de dados volumosos, essenciais para o sistema. O MongoDB permitiu um armazenamento mais eficiente das informações de vendas e previsões.

2. **Mobile Application Development**
   - Um servidor foi desenvolvido com Node.js, incluindo um CRUD completo para operações do projeto, como gestão de dados de vendas e estoque. Esse sistema foi testado com o Postman para assegurar consistência e robustez, possibilitando que o sistema seja utilizado em dispositivos móveis, facilitando o acesso remoto às previsões de estoque.

3. **Advanced Business Development with .NET**
   - A API StylistPro.Produto.API foi aprimorada com:
     - **Integração com ViaCEP**: Inclusão de consulta de CEP para informações geográficas detalhadas, permitindo uma melhor contextualização de previsões de demanda.
     - **Inteligência Artificial com ML.NET**: Implementação de um sistema de recomendações personalizadas com base no histórico de vendas e preferências dos usuários.
     - **Testes Unitários**: Inclusão de testes nas camadas ApplicationService e Repository, aumentando a qualidade e confiabilidade da API.
     - **Práticas de Clean Code e SOLID**: Seguindo princípios como SRP, OCP e DIP, a organização do código foi melhorada, facilitando a manutenção e o crescimento do sistema.

4. **Compliance, Quality Assurance & Tests**
   - Utilizando Azure DevOps, foram planejados testes manuais em sprints para garantir a qualidade do sistema. Realizamos testes de carga com JMeter para avaliar o desempenho e identificar gargalos, ajustando o sistema para lidar com períodos de alta demanda. Esses testes asseguraram a eficiência e robustez das previsões.

5. **Java Advanced**
   - Durante a quarta entrega, implementamos o Spring Security para garantir segurança de dados, protegendo senhas e informações sensíveis. A integração com RabbitMQ otimizou a mensageria entre componentes do sistema, aprimorando o tempo de resposta. O uso do Thymeleaf para criar telas e do Spring Security para segurança proporcionaram uma experiência de usuário mais robusta e segura.

6. **DevOps Tools & Cloud Computing**
   - A implantação do sistema na nuvem envolveu o uso de Serviços de Aplicativo do Azure e Azure Container Registry (ACR) junto com Azure Container Instances (ACI) para oferecer uma estrutura escalável e fácil de manter. Além disso, uma pipeline de CI/CD foi implementada no Azure DevOps, automatizando o build e o deploy. Essa esteira de integração contínua reduziu o tempo de produção, aumentando a eficiência e diminuindo os custos operacionais.

---

Este documento resume o progresso do **Sistema de Previsão de Estoque de Roupas com IA**, destacando suas capacidades atuais, desafios encontrados, e as futuras direções para aprimorar a precisão, escalabilidade e usabilidade do sistema. A aplicação prática dos conhecimentos em diversas disciplinas contribuiu para o desenvolvimento de um sistema robusto, flexível e alinhado às necessidades do mercado de moda e varejo.
