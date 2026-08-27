# ClínicaApp

Aplicação desktop para gerenciar médicos, pacientes, disponibilidades e consultas de uma clínica. O projeto separa os fluxos de paciente e médico e mantém os dados localmente em arquivos de texto.

Projeto acadêmico desenvolvido na disciplina de Linguagem de Programação II do IFBA.

## Funcionalidades

- Cadastro de pacientes e médicos
- Identificação do usuário por ID
- Cadastro de horários disponíveis por médico
- Agendamento de consultas por especialidade
- Visualização da agenda e do histórico do paciente
- Cancelamento e solicitação de reagendamento
- Controle de status das consultas
- Persistência local de pacientes, médicos e consultas

## Tecnologias

- Java 21
- JavaFX 21
- FXML
- Maven
- Collections, Streams e API de data e hora

## Estrutura principal

- `models/`: entidades do domínio
- `SistemaAgendamento.java`: regras de cadastro, disponibilidade e agendamento
- `ClinicaController.java`: integração entre as telas FXML e as regras da aplicação
- `ArquivoUtils.java`: leitura e gravação dos arquivos locais
- `src/main/resources/view/`: telas da aplicação

## Como executar

~~~bash
mvn javafx:run
~~~

Requer JDK 21 e Maven. O `pom.xml` atual usa o classificador JavaFX para Windows; para executar em Linux ou macOS, ajuste ou remova o classificador das dependências JavaFX.
