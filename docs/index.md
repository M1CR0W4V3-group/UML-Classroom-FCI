<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Ciência da Computação</a></h3>


<font size="+12"><center>
*&lt;Sistema de Presenças&gt;*
</center></font>

>*Observação 1: A estrutura inicial deste documento é só um exemplo. O seu grupo deverá alterar esta estrutura de acordo com o que está sendo solicitado na disciplina.*

>*Observação 2: O índice abaixo não precisa ser editado se você utilizar o Visual Studio Code com a extensão **Markdown All in One**. Essa extensão atualiza o índice automaticamente quando o arquivo é salvo.*

**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do Projeto](#introdução-do-projeto)
- [Análise de Requisitos Funcionais e Não-Fucionais](#descrição-dos-requisitos)
- [Diagrama de Atividades](#diagrama-de-atividades) 
- [Diagrama de Casos de Uso](#diagrama-de-comportamento-atores)
- [Descrição dos Casos de Uso](#descrição-das-funcões)
- [Diagrama de Senquencia](#diagrama-de-ordem-interações)
- [Diagrama de Classes](#diagrama-orientado-objetos)
- [Diagrama de Estados](#diagrama-estrutura-componente)
- [Diagrama de Implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* Eduardo Oliveira Carvalho
* Felipe Viviani Schulze
* Guilherme Ferreira Martins Ramos
* Lucas Tuon de Matos
* Rodrigo Nascimento Tomaz


# Descrição do Projeto

  A Escola Infinito precisa de um sistema moderno e intuitivo para controlar a presença de seus alunos, já que até então,
  esse processo era feito no papel. A equipe Micro-Ondas recebeu a tarefa de automatizar o controle de presenças de modo
  que atenda os requisitos e expectativas dos gestores da escola. 

# Análise de Requisitos Funcionais e Não-Funcionais

* Requisitos Funcionais:
 
 [RF001] Login

O usuário deve ser capaz de entrar no sistema utilizando usuário (email) e senha.
Deverá haver um login para pais, professores e admins.

 * Pais só podem ver as faltas do(s) seu(s) filho(s)
 * Professores podem aplicar as faltas da sua turma somente no dia atual;
 * Admins podem alterar as faltas de qualquer momento.

Prioridade:	       ◾ Essencial	      ◻ Importante  	◻ Desejável 


[RF002] Fazer cadastro

O usuário administrador deve ser capaz de criar uma conta de professores e pais no sistema inserindo dados como email, nome e senha.

* Deve validar dados obrigatórios como e-mail, nome e função do usuário.
* Professores devem ser atribuídos a uma ou mais turmas.
* Pais devem ser atribuídos a alunos.
* Validação de e-mail duplicado.



Prioridade:	       ◾ Essencial	      ◻ Importante  	◻ Desejável

[RF003] Registrar e exibir Faltas

O sistema deve poder acessar, registrar,  alterar e exibir as faltas dos alunos em cada matéria.

* Professores podem registrar faltas diariamente para sua turma no dia da aula.
* As faltas podem ser filtradas por data, disciplina, turma e aluno.
* Admins podem corrigir faltas e editar registros antigos.



Prioridade:	       ◾ Essencial	      ◻ Importante  	◻ Desejável





[RF004] Operar Banco de Dados da Escola

O sistema deve ter acesso a um banco de dados onde estão armazenados todos os dados dos alunos.

* As informações devem ser atualizadas em menos de 24 horas no B.D. 
* O banco deve armazenar informações de presença, cronograma, alunos e seus responsáveis.



Prioridade:	       ◾ Essencial	      ◻ Importante  	◻ Desejável

[RF005] Acesso aos Cronogramas de Aulas

O sistema deve ter acesso aos horários de aula de todas as turmas.

* Deve permitir a criação, alteração e visualização do cronograma de aulas.
* Professores só podem visualizar o cronograma da sua própria turma.
* Admins podem gerenciar cronogramas de todas as turmas.



Prioridade:	       ◾ Essencial	      ◻ Importante  	◻ Desejável


[RF006] Gerar relatório

O sistema deve ser capaz de gerar relatórios (faltas da semana, do mês e boletim) em relação às faltas dos alunos.

* Relatórios devem ser exportáveis em formato PDF. 
* Relatórios de alunos com presença inferior a 75% devem ser gerados automaticamente.



Prioridade:	       ◾Essencial	      ◻ Importante  	◻ Desejável


[RF007] Notificação aos responsáveis

O sistema deve verificar as faltas dos alunos todo final de mês e notificar os pais/responsáveis se este exceder 20% de faltas do total de aulas dadas até o momento. 

* Notificações devem ser enviadas via e-mail da instituição ou por SMS.




Prioridade:	      ◾Essencial	      ◻ Importante  	◻ Desejável



* Requisitos Não Funcionais:

[RNF001] LGPD

O sistema deve atender todos os requisitos da LGPD.

* Todos os dados sensíveis devem ser criptografados, especialmente dados pessoais e senhas.


Prioridade:	       ◾ Essencial	      ◻ Importante  	◻ Desejável


[RNF002] Acessibilidade

O sistema deve ser acessível e intuitivo.

* Tamanho e redimensionamento de fonte:
   - A fonte padrão deve ser de 16 pixels, pois fontes menores podem causar dificuldades a idosos e pessoas com deficiências visuais. O redimensionamento da fonte deve ocorrer de forma adequada para não desformatar o site.
* Utilização do VLibras.
* Contraste de cor entre o texto e o fundo, modo de alto contraste e modo escuro
* Suporte ao teclado:
   - Todos os elementos interativos do site devem ser acessíveis via teclado, permitindo que os usuários usem sem o mouse.



Prioridade:	       ◻ Essencial	      ◾ Importante  	◻ Desejável


[RNF003] Visualizar Faltas


* Os pais só podem visualizar as faltas dos seus filhos
* Os professores só podem visualizar as faltas dos seus alunos
* Os administradores podem visualizar todas as faltas


Prioridade:	       ◾ Essencial	      ◻ Importante  	◻ Desejável


[RNF004] Aplicar Faltas

Maneira que o sistema de faltas operará:

* Os professores só podem aplicar as faltas do dia atual
* Os administradores podem alterar as faltas a qualquer momento


Prioridade:	       ◾ Essencial	      ◻ Importante  	◻ Desejável


[RNF005] Criptografia de Senhas
* A senha deve ser criptografada por meio de um hash na hora do cadastro e esse hash será salvo no banco de dados.


Prioridade:	       ◾ Essencial	      ◻ Importante  	◻ Desejável

[RNF006] Suporte para diferentes sistemas

O sistema deve ser acessível por qualquer navegador web moderno e também ser responsivo, adaptando-se a dispositivos móveis.

* O layout deve ajustar-se automaticamente para tablets e celulares.
* Deve funcionar nos principais navegadores: Chrome, Firefox, Safari. 


Prioridade:	        ◾ Essencial	      ◻ Importante  	◻ Desejável


[RNF007] Performance com acessos simultâneos 

* O sistema deve ser escalável para suportar pelo menos 100 usuários, sendo que pais e funcionários da escola o estarão utilizando diariamente. 
* O sistema deve ser capaz de suportar picos de uso durante períodos de chamada.
Prioridade:	        ◻ Essencial	      ◾ Importante  	◻ Desejável

[RNF005] Backups e Recuperação de Dados

* Deve haver backup automático diário dos dados do sistema, com possibilidade de recuperação em caso de falhas.
* Backups devem ser armazenados em local seguro e acessível remotamente.
Prioridade:            ◾ Essencial	      ◻ Importante  	◻ Desejável

# Diagrama de Atividades

![Diagrama de AtividadesCerto drawio](https://github.com/user-attachments/assets/94910f05-1cb8-4d92-9009-5da5013b2217)

# Diagrama de Casos de Uso

*&lt;Diagrama para visualizar o comportamento dos atores&gt;*

# Descrição dos Casos de Uso

Atores:

*Usuários: São o grupo central do sistema, aqueles que irão o utilizar. Poderão ser administradores, professores ou responsáveis dos alunos.

*Administradores: Aqueles que irão gerenciar a aplicação, criando os demais usuários e modificando o registro de faltas, em casos de erros de registro por parte do professor.

*Professores: Acessam o painel de chamada para registrar a presença de alunos que sejam de sua matéria. Também podem gerar um relatório em PDF com base no registro de faltas.

*Responsáveis: Acessam o histórico de falta do aluno de sua responsabilidade, podendo selecionar entre um ou mais, dependendo de quantos alunos tenha matriculado. Também podem gerar um relatório PDF das faltas de seus dependentes.

Sistema de Presenças:

*É o software que armazena os dados e as funcionalidades. Apresenta a interface para os usuários com os registro de faltas, feito por integração aos dados do banco, e apresenta os relatórios.

O sistema é projetado para fornecer um controle eficiente das faltas escolares, com a possibilidade de modificação, visualização e exportação de relatórios. Cada ator tem acesso as funcionalidades do software de acordo com sua função, com os administradores agindo por trás da aplicação, professores resgistrando as faltas de seus alunos e responsáveis visualizando a presença de seus dependentes.


# Diagrama de Sequência

*&lt;Diagrama de ordem e interação dos objetos&gt;*

# Diagrama de Classes

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

# Diagrama de Estados

*&lt;Diagrama para permite modelar o comportamento interno de um determinado objeto, subsistema ou sistema global&gt;*

# Diagrama de Implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

# Referências

*&lt;Lista de referências&gt;*
