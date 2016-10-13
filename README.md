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
     
     1. Dependency Injection ou Injeção de Dependência: É um padrão de projeto de software que visa reduzir o acoplamento entre as classes e realizar o desenvolvimento para interfaces. Na DI o desenvolvedor não precisa instanciar um objeto o framewok de injeção de dependência fica responsável por instanciar os objetos da aplicação.

     
     2. Repository ou Repositório: Também é um padrão de projeto que provê o acesso de outras camadas da aplicação com os dados armazenados do sistema. Ele abstrai o acesso a informação independente da forma como os dados estão armazenados como também da ferramenta usada para armazenar as informações.

     
     3. Unit of work ou unidade de trabalho:

     	
        
        
