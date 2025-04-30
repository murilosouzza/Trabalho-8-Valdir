# Trabalho sobre requisitos
# UNIMAR (Universidade De Marília)
# Professor: Valdir
# Aluno: Murilo Santos Souza
# RA: 2038823 
# Curso: ADS, Turma C, Noturno
# Cenário: Sistema de Gerenciamento de Clínica Médica  
# Descrição do Sistema: 
A clínica médica deseja implementar um sistema para gerenciar consultas, médicos, 
pacientes e prontuários médicos. O sistema deve permitir que os pacientes agendem 
consultas online, que os médicos acessem e atualizem prontuários e que os 
administradores gerenciem o cadastro de médicos e pacientes.  
Atores:  
• Paciente: Usuário que agenda consultas e visualiza seu histórico médico.  
• Médico: Profissional de saúde que realiza consultas, acessa e atualiza 
prontuários dos pacientes.  
• Administrador: Usuário que gerencia o cadastro de médicos e pacientes, além 
de gerenciar as consultas.  
Exercícios:  
# 1. Listando 6 casos de uso considerando todos os atores
- Agendar consulta.
- Visualizar histórico médico.
- Acessar ficha do paciente.
- Atualizar ficha do paciente.
- Cadastrar médico.
- Cadastrar paciente.
- Gerenciar consulta.


# 2. Relacionar cada ator com seus respectivos casos de uso.

| Ator| Casos de uso |
|---|---|
| *Paciente*  | Agendar consulta, Visualizar histórico médico. |
| *Médico* | Acessar ficha do paciente, e atualizar o prontuário dele. |
| *Admnistrador* |Cadastro de médicos, cadastro de pacientes, administrar consultas. |

# 3. Escolha dois casos de uso para detalhar, especificando pré-condições, fluxo.

# Caso de uso 1: Agendar consulta.
# Ator: Paciente.
# Pré-condição:
O paciente deve estar cadastrado e autenticado no sistema.
# Fluxo principal:
* O paciente acessa a função de agendamento.
* O sistema mostra os médicos e seus horários disponíveis.
* Dentro disso o paciente escolhe um médico e um horário disponível.
* O sistema registra o agendamento.
* O sistema confirma o agendamento.
# Fluxos alternativos (Exceção)
* Se o horário já estiver preenchido, o sistema informa e solicita uma nova escolha
* Caso o médico não esteja mais disponível o sistema atualiza a lista de médicos disponíveis.
# Pós-condição
* Consulta agendada com êxito, sendo vísivel tanto ao paciente quanto ao médico
# Caso de uso 2: Atualizar a ficha do paciente
# Ator: Médico
# Pré condição:
O médico deve estar autenticado e autorizado a acessar a ficha do paciente
# Fluxo principal
* O médico seleciona seu paciente depois da consulta.
* O sistema exibe a ficha médica.
* O médico adiciona ou muda informações sobre a consulta.
* O sistema salva essas alterações na ficha.
# Fluxos alternativos (Exceção)
* Caso o paciente não seja encontrado o sistema exibe uma mensagem de erro.
* Se acabar havendo erro ao salvar informações, o sistema alerta o médico e mantém os dados antigos.
# Pós-condições
* Ficha atualizada com as informações da consulta.


