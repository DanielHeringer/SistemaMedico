# Sistema Médico

## Alunos: 
Daniel Lamounier Heringer, 743524<br>
João Gabriel Damasceno, 726545<br>
Philipe Fonseca Bittencourt, 726579<br>

## Execução e Configuração
Para configurar e executar, basta ter os requisitos:
<ul>
  <li>  SGBD: MySql </li>
  <li>  Esquema: sistema_medicos </li>
  <li>  O arquivo de configuração é o <i>src\main\resources\application.properties</i>. Nele podem ser alterados o usuário e a senha do SGBD</li>
  <li>  No arquivo <i>src\main\java\br\ufscar\dc\dsw\SistemaMedicoApplication.java</i> estão os comandos para popular o banco. com os seguintes dados:</li>
</ul>

Usuários:

| email  |  senha  | role |
| --- | --- | --- |
|  admin |  admin | ROLE_ADMIN |
|  joao@gmail.com |  joao | ROLE_PACIENTE |
|  philipe@gmail.com |  philipe | ROLE_PACIENTE |
|  daniel@gmail.com |  daniel | ROLE_MEDICO |
|  Delano@gmail.com |  delano | ROLE_MEDICO |


Consultas: 

| data  |  paciente  | medico |
| --- | --- | --- |
| 2021-01-15 |  Joao | Daniel |
| 2021-01-16 |  Joao | Delano |
| 2021-03-03 |  Philipe | Delano |

Caso for rodar mais de uma vez, é necessário retirar o trecho de código em que os dados são inseridos, no arquivo <i>src\main\java\br\ufscar\dc\dsw\SistemaMedicoApplication.java</i>

## O sistema deve atender aos seguintes requisitos:

✔ R1: CRUD 1 de médicos (requer login de administrador)

✔ R2: CRUD de pacientes (requer login de administrador)

✔ R3: Listagem de todos os médicos em uma única página (não requer login)

✔ R4: Listagem de todos os médicos por especialidade (não requer login)

✔ R5: Agendamento de consulta com um médico (requer login do paciente via email + senha).
Depois de fazer login, o paciente pode cadastrar uma consulta. Para isso, deve escolher um
médico (escolhendo a partir de uma lista), uma data/horário, e deve ser gravado a consulta
na base de dados.

✔ R6: Listagem de todas as consultas de um paciente (requer login do paciente via e-mail +
senha). Depois de fazer login, o paciente pode visualizar todas as suas consultas gravadas.

✔ R7: O sistema não deve permitir o cadastro de consultas de um mesmo médico ou de um
mesmo paciente em uma mesma data/horário.

✔ R8: Listagem de todas as consultas de um médico (requer login do médico via e-mail +
senha). Depois de fazer login, o médico pode visualizar todas as suas consultas gravadas.

✔ R9: O sistema deve ser internacionalizado em pelo menos dois idiomas: português + outro
de sua escolha. 
