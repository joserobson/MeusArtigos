# Meus Artigos
  Escrever aqui os textos para meu blog.
  
  **Entendendo os Padrões Dependency Injection (Injeção de Dependência) e Unit Of Work (Unidade de Trabalho)**
  
  Implementando os padrões DI e Unit of Work e Repository usando os frameworks Castle Windsor e NHibernate
  
  Sumário
  	- Introdução
    - Problemas
    	- Como abrir/fechar conexões
        - Como gerenciar transações
        
     **Introdução**
     
     Neste artigo vamos falar sobre os padrões dependecy injection, repository e unit of work.
     
    -  Dependency Injection ou Injeção de Dependência: É um padrão de projeto de software que visa reduzir o
     acoplamento entre as classes e aplicarrealizar o desenvolvimento para interfaces. Na DI o desenvolvedor não precisa
     instanciar um objeto dentrao de uma classe, removendo assim as dependências chamadas hard-coded. O framewok de injeção de dependência fica responsável por instanciar os objetos da aplicação através do construtor. 

     
     - Repository ou Repositório: Padrão que provê uma camada de acesso parapor outras camadas da aplicação paracom os dados daarmazenados aplicaçãodo sistema. Ele abstrai o acesso a informação independente da forma como os dados estão armazenados
     como também da ferramenta usada para armazenar essasas informações.

     
     -  Unit of work ou unidade de trabalho: Padrão utilizado para definir e a gerenciar as trabalhostransações transacionais de uma aplicação.
     
     
     **Problemas**
     
		Quando você está desenvolvendo uma aplicação dirigida a dados, aplicações cujo foco é a leitura e gravação de dados, você deve considerar alguns princípios. Nesta seção eu irei descrever e então explicar brevemente cada princípio.
        
     **Como abrir e fechar conexões**
      
     	O primeiro problema: Como e onde abrir e fechar conexões. Certamente, o melhor para gerenciar é conexões é na camada de banco de dados(provavelmente nos repositórios). Então, nós podemos abrir a conexão, executar o comando do banco de dados e fechar a conexão para cada método de um repositório.  
