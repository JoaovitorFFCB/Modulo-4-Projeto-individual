Existem outras entidades além dessas três?
  Sim, é necessário definir quais são os cursos ofertados, as turmas disponíveis, os professores para cada turma, os horários das turmas, qual a disponibilidade dos professores em relação ao horário e para os alunos podem ser definidos campos como nome, documentação e endereço.

Quais são os principais campos e tipos?
  Tabela Cursos: Campos: id/ Formação WebDev/ Formação Data Analytics; Tipo: INT/ VARCHAR/ VARCHAR
  Tabela Turmas: Campos: id/ Turma WebDev/ Turma Data Analytics; Tipo: INT/ VARCHAR/ VARCHAR
  Tabela Horário: Campos: id/ Manhã/ Tarde/ Noitr; Tipo: INT/ VARCHAR/ VARCHAR/ VARCHAR
  Tabela Professor: Campos: id/ Nome/ Sobrenome; Tipo: INT/ VARCHAR/ VARCHAR
  Tabela Alunos: Campos: id/ Nome/ Sobrenome; Tipo: INT/ VARCHAR/ VARCHAR
  Tabela Endereço: Campos: id/ Rua/ Numero/ Complemento; Tipo: INT/ VARCHAR/ VARCHAR/ VARCHAR
  Tabela Documentos: Campos: id/ CPF/ RG/ Matricula; Tipo: INT/ INT/ INT/ VARCHAR

Como essas entidades estão relacionadas?
  Cursos está em relação de 1x1 com Turmas
  Turmas está em relação nxn com Horário / 1xn com Professor / nxn com Alunos
  Horário está em relação de nxn com Turmas / nxn com Professor
  Professor está em relação de 1xn com Turmas / nxn com Horário
  Alunos está em relação de nxn com Turmas / nxn com Professor / 1x1 com Documentos / 1x1 com Endereço
  Endereço está em relação de 1x1 com Alunos
  Documentos está em relação de 1x1 com Alunos
