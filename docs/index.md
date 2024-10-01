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
 
  • [RF001] Login
    O usuário deve ser capaz de entrar no sistema utilizando usuário (email) e senha.
    Deverá haver um login para pais, professores e admins.

    - Pais só podem ver as faltas do(s) seu(s) filho(s)
    - Professores podem aplicar as faltas da sua turma somente no dia atual;
    - Admins podem alterar as faltas de qualquer momento.

  • [RF002] Fazer cadastro
    O usuário administrador deve ser capaz de criar uma conta de professores e pais no sistema inserindo dados como email,      nome e senha.
  
  • [RF003] Registrar e exibir Faltas
    O sistema deve poder acessar, registrar,  alterar e exibir as faltas dos alunos em cada matéria.

  • [RF004] Operar Banco de Dados da Escola
    O sistema deve ter acesso a um banco de dados onde estão armazenados todos os dados dos alunos.

  • [RF005] Acesso aos Cronogramas de Aulas
    O sistema deve ter acesso aos horários de aula de todas as turmas.

  • [RF006] Gerar relatório
    O sistema deve ser capaz de gerar relatórios (faltas da semana, do mês e boletim) em relação às faltas dos alunos.

  • [RF007] Notificação aos responsáveis
    O sistema deve verificar as faltas dos alunos todo final de mês e notificar os pais/responsáveis se este exceder 20% de      faltas do total de aulas dadas até o momento.

* Requisitos Não Funcionais:
  
  • [RNF001] LGPD
    O sistema deve atender todos os requisitos da LGPD.

  • RNF002] Acessibilidade
    O sistema deve ser acessível e intuitivo.
      - Tamanho e redimensionamento de fonte:
    A fonte padrão deve ser de 16 pixels, pois fontes menores podem causar dificuldades a idosos e pessoas com deficiências     visuais. O redimensionamento da fonte deve ocorrer de forma adequada para não desformatar o site.
    Utilização do VLibras.
    Contraste de cor entre o texto e o fundo, modo de alto contraste e modo escuro.
    Suporte ao teclado:
	    - Todos os elementos interativos do site devem ser acessíveis via teclado, permitindo que os usuários usem sem o           mouse.

  • [RNF003] Visualizar Faltas
    Os pais só podem visualizar as faltas dos seus filhos
    Os professores só podem visualizar as faltas dos seus alunos
    Os administradores podem visualizar todas as faltas

  • [RNF004] Aplicar Faltas
    Os professores só podem aplicar as faltas do dia atual
    Os administradores podem alterar as faltas a qualquer momento

  • [RNF005] Criptografia de Senhas
    A senha deve ser criptografada por meio de um hash na hora do cadastro e esse hash será salvo no banco de dados.
  
# Diagrama de Atividades

*&lt;Diagrama para visualizer as pessoas das áreas de negócios e de desenvolvimento de uma organização para entender o processo e comportamento.&gt;*

# Diagrama de Casos de Uso

*&lt;Diagrama para visualizar o comportamento dos atores&gt;*

# Descrição dos Casos de Uso

*&lt;Descrição do comportamento entre os atores/resquisitos&gt;*

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
