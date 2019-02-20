-Funcionalidades


O projeto a seguir contem as seguintes funcionalidades : 

 	entrar no sistema como usuário

 	sair do sistema

 	criar um novo projeto

 	editar informações de um projeto existente

 	mudar o estado de um projeto

 	consultar as informações de um usuário

 	consultar as informações de um projeto

 	consultar as informações de uma atividade

 	verificar as atividades da unidade academia

-Classes do Projeto
	
  Main : 

			Motivação : Criar uma classe onde tudo se forma
			
			Solução : com essa classe , tudo fica bem estruturado e no seu devido lugar
			
			Vantagem : organização das funcionalidades


  Projeto : 
			
			Motivação : Criar uma classe que agrega as informações em comum entre os estados de projeto

			Solução : Fazer essa classe conter o que há em comum entre os estados , e faze-los herdar isso

			Vantagem : Permite que suas subclasses herdem suas caracteristicas
		
  Heranças de Projeto :

			Projeto em Criação :
		
				Motivação : Criar algo que armazene os dados de um projeto ainda em criação

				Solução : Com essa classe , as informações de um projeto em criação são facilmente armazenadas

				Vantagem : Um projeto em criação não poder ter acesso a algo que não está relacionado
			
				Desvantagem : Não herdar caracteristicas privadas da sua super-classe[

			Projeto Iniciado :

				Motivação : Criar algo que armazene as informações de um projeto já iniciado

				Solução : A criação de uma sub-classe de Projeto , que contenha essas informações

				Vantagem : Não poder ter acesso a algo pertencente a outra sub-classe da mesma super-classe

				Desvantagem : Não herdar caracteristicas privadas da super-classe

			Projeto em Andamento : 

				Motivação : Criar algo que possua as informações de um projeto já em andamento

				Solução : A criação de uma sub-classe contendo as informações específicas

				Vantagem : Não poder ter suas informações usadas por outras sub-classes

				Desvantagem : Não conter informações privadas de sua super-classe

			Projeto concluido :

				Motivação : Conter dados de um projeto que já foi concluido

				Solução : Uma sub-classe de Projeto , contendo tudo que um projeto deve ter , e tudo que um projeto concluido deve ter

				Vantagem : Possuir caracteristicas em comum com outras sub-classes da mesma super-classe , mas tambem ter caracteristicas unicas

				Desvantagem : Não possuir informações privadas de sua super-classe

  Colaborador : 

			Motivação : Conter informações comuns entre colaboradores

			Solução : Uma classe contendo essas caracteristicas

			Vantagem : Facil utilização de métodos e variáveis não privadas

			Desvantagem : Para ter acesso à suas caracteristicas privadas , é necessário métodos públicos

  Heranças de Colaborador : 

			Aluno de Graduação :

				Motivação : guardar dados de um aluno de graduação

				Solução : Uma classe contendo os dados de um aluno de graduação que é colaborador

				Vantagem : Utilização de métodos e variáveis , desde que não sejam privadas , de sua super-classe

			Aluno de Mestrado :

				Motivação : guardar os dados de um aluno de mestrado

				Solução : uma sub-classe de Colaborador , contendo as informações de um aluno de mestrado

				Vantagem : Acesso a todos as informações de um Colaborador

			Aluno de Doutorado : 

				Motivação : guardar os dados de um aluno de doutorado

				Solução : com essa classe , é possivel conter os dados de um aluno de doutorado , e os de um Colaborador

				Vantagem : Acesso aos dados de um Colaborador

			Professor :

				Motivação : guardar os dados de um professor

				Solução : com essa classe , é possivel conter os dados de um professor

				Vantagem : Acesso aos dados de um Professor e de um Colaborador

			Pesquisador :

				Motivação : Conter os dados de um pesquisador

				Solução : Criar uma sub-classe de Colaborador , contendo os dados do mesmo , alem dos seus próprios dados

				Vantagem : Acesso aos dados de um pesquisador e um colaborador

			Profissional :

				Motivação : conter os dados de um profissional

				Solução : criar uma classe contendo esses dados

				Vantagem : Conter os dados da super-classe , alem dos proprios
	
  Interface :

		Motivação : Poder trocar os estados de um projeto

		Solução : criar uma interface que é implementada pelos estados de projeto

		Vantagem : Trocar de estado facilmente

  Extensibilidade :

  	Motivação : possuir várias classes com caracteristicas similares

  	Solução : Criar uma super-classe com várias sub-classes , fazendo-as possuir suas características

  	Vantagem : Não precisar colocar as caracteristicas em comum entre várias classes
