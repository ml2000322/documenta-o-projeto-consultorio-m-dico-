+------------------+          +--------------------+         +------------------+
|   especialidades |<---------|      medicos       |-------->|     clinicas     |
|------------------|          |--------------------|         |------------------|
| especialidade_ID |◄──┐      | medico_ID          |         | clinica_ID       |
| nome             |   └─────►| CRM                |         | nome             |
+------------------+          | nome               |         | endereco         |
                              | especialidade_ID FK|         +------------------+
                              | clinica_ID FK      |
                              +--------------------+
                                       ▲
                                       |
                                       |
                              +--------------------+
                              |     consultas       |
                              |--------------------|
                              | consulta_ID        |
                              | paciente_ID FK     |
                              | medico_ID FK       |
                              | tipoConsulta       |
                              | dataConsulta       |
                              | statusConsulta     |
                              | observacoes        |
                              +--------------------+
                                       ▲
                                       |
                                       |
                              +--------------------+
                              |     pacientes       |
                              |--------------------|
                              | paciente_ID        |
                              | nome               |
                              | cpf                |
                              | telefone           |
                              | dataNasc           |
                              | cidade             |
                              +--------------------+
