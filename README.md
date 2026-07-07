Sistema Clínica Vida+

Sistema simples de linha de comando para gerenciar o cadastro de pacientes de uma clínica, escrito em Python puro (sem dependências externas).

Funcionalidades


Cadastrar paciente — registra nome, idade e telefone.
Ver estatísticas — mostra total de pacientes, idade média, paciente mais novo e paciente mais velho.
Buscar paciente — procura um paciente pelo nome (não diferencia maiúsculas/minúsculas).
Listar todos os pacientes — exibe todos os pacientes cadastrados.
Sair — encerra o sistema.


Requisitos


Python 3.6 ou superior


Nenhuma biblioteca externa é necessária.

Como executar

bashpython projeto_s+.py

(substitua pelo nome real do arquivo .py, caso seja diferente)

Como usar

Ao iniciar, o sistema exibe um menu:

=== SISTEMA CLÍNICA VIDA+ ===
1. Cadastrar paciente
2. Ver estatísticas
3. Buscar paciente
4. Listar todos os pacientes
5. Sair

Digite o número da opção desejada e siga as instruções na tela.

Exemplo de cadastro

Escolha uma opção: 1
Nome do paciente: Maria Silva
Idade: 34
Telefone: (11) 91234-5678
Paciente cadastrado com sucesso!

Estrutura do código

FunçãoDescriçãocadastrar_paciente()Coleta os dados do paciente e adiciona à lista pacientes.ver_estatisticas()Calcula total, idade média, e identifica o paciente mais novo/velho.buscar_paciente()Filtra a lista pacientes pelo nome informado.listar_pacientes()Percorre e exibe todos os registros da lista pacientes.

Os dados são armazenados apenas em memória, na lista pacientes. Isso significa que todos os cadastros são perdidos ao encerrar o programa — não há persistência em arquivo ou banco de dados.

Limitações conhecidas


Sem validação de entrada (ex: idade não numérica causa erro).
Sem persistência de dados entre execuções.
Busca por nome exige correspondência exata (não busca parcial).


Possíveis melhorias futuras


Salvar os dados em um arquivo (JSON, CSV) ou banco de dados.
Validar entradas do usuário (idade, telefone).
Permitir edição e remoção de pacientes.
Adicionar busca parcial por nome.
