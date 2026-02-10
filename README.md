🗺️ Roadmap – Projeto Spring + Consumo de API
:) Este projeto foi desenvolvido com o objetivo de praticar Spring Boot sem Web, consumo de API externa e boas práticas de organização de código em Java.

🟢 1. Estrutura de um Projeto Spring
Base do projeto
Organização em pacotes (model, service, application)
Classe principal anotada com @SpringBootApplication
Uso do método run() como ponto de execução da aplicação
->Objetivo: entender a estrutura inicial de um projeto Spring

🟢 2. Inferência de Tipos no Java (var)
Código mais limpo e moderno
Uso da palavra-chave var
O Java infere automaticamente o tipo da variável
-> Objetivo: reduzir verbosidade e melhorar a legibilidade do código

🟢 3. Consumo de API
Integração com serviços externos
Classe responsável por consumir a API
Método obterDados() retorna os dados em formato JSON (String)
Uso de URL + API Key
->Objetivo: aprender a consumir dados de APIs externas

🟢 4. Modularização do Código
Separação de responsabilidades
Uma classe para consumo da API
Uma classe para conversão de dados
Classes específicas para os modelos
-> Objetivo: manter o código organizado, reutilizável e fácil de manter

🟢 5. Serialização e Desserialização
Conversão entre JSON e Java
JSON → Objeto Java (desserialização)
Uso da biblioteca Jackson
Conversão com ObjectMapper.readValue()
-> Objetivo: transformar dados da API em objetos Java

🟢 6. Interfaces + Generics
Código flexível e reutilizável
Criação da interface IConverteDados
Uso de Generics (<T>)
Conversão de diferentes tipos de classes com o mesmo método
-> Objetivo: aplicar boas práticas e reaproveitar código

🟢 7. Implementação da Interface
Aplicação prática
Classe ConverteDados implements IConverteDados
Implementação do método genérico
Tratamento de exceções durante a conversão
-> Objetivo: separar contrato (interface) da implementação

🟢 8. Mapeamento com Jackson
Evitar erros de conversão
Uso de @JsonAlias para mapear nomes diferentes no JSON
Uso de @JsonIgnoreProperties(ignoreUnknown = true)
->Objetivo: garantir robustez ao lidar com JSONs maiores que o modelo

🟢 9. Gerenciamento de Dependências (Maven)
Controle do projeto
Inclusão do Jackson no pom.xml
Maven responsável por baixar e gerenciar as dependências
-> Objetivo: entender como o projeto cresce de forma organizada

🟢 10. Execução e Testes
Validação do fluxo completo
Execução da aplicação Spring
Impressão do JSON retornado pela API
Impressão do objeto Java convertido
-> Objetivo: validar que todo o fluxo funciona corretamente
