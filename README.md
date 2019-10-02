**Engenharia Reversa de um banco de dados existente usando Code-First me Fluent API..

  
Nesse exemplo, dica útil para  um programador .Net,  veremos como  fazer engenharia reversa de uma banco de dados  partindo da existência de um banco de dados, sem precisar  “mexer na estrutura do seu banco legado”.  Para isso usaremos alguns recursos do CodeFirs Entity Framework e API Fluent. Com ele podemos facilmente mapear classes de um modelo de banco de dados, inclusive melhorando as nomeclaturas da propriedade dos objetos da base.
O Entity Framework: fornece uma maneira fácil de usar a abordagem de primeiro código para um banco de dados existente. Ele criará classes de entidade de todas as tabelas   do seu banco de dados existente e as configurará com: 
DataAnnotations: foram introduzido no .NET 3.5 como uma forma de adicionar a validação para as classes usadas por aplicações ASP.NET. 

 : [Acesse o link para saber mais sobre os DataAnnotations](https://docs.microsoft.com/pt-br/dotnet/api/system.componentmodel.dataannotations?view=netframework-4.8)	 

Nesse exemplo, vou usar o console Application para demonstrar.

1-	Abra o visual Studio  Crie um  projeto novo do tipo Console Application.

2-	Com o botão direito do mouse em seu projeto no Visual Studio -> Adicionar -> Novo Item. Fig(1)
![Legenda](https://i.ibb.co/Z8wsTWM/img1.png)	

3	- Selecione Modelo de Dados da Entidade **ADO.NET** na caixa de diálogo Adicionar Novo Item, especifique o nome do modelo (este será um nome de classe de contexto) e **clique em Adicionar**.

![Legenda](https://i.ibb.co/FhXRxsH/img-2.png)	

4	– Após seguir o passo anterior  abrira o assistente do modelo do Entity, como mostrado abaixo. **Selecione a opção CodeFirst From Database e clique em Next**.

![Legenda](https://i.ibb.co/gvT9VCN/img-3.png)
 
Figura 3

5	- Agora, selecione em **New Connection**, seguida insira o **Server Name** (nome do seu servidor SQL e o banco de dados), feito isso clique em OK para continuar.
![Legenda](https://i.ibb.co/y6j9vJX/img-4.png)

 
Figura 4
6	-  Agora, escolha as tabelas para as quais deseja gerar classes e clique em Finish.
![Legenda](https://i.ibb.co/k4bRcxS/img-5.png)

Figura 5
Isso irá gerar todas as classes de entidade para das suas tabelas e   banco de dados, como mostrado abaixo.
![Legenda](https://i.ibb.co/25zjsG8/img-6.png)
Figura 6

Por exemplo, ele criará  a classe de contexto que usa a Fluent API para configurar os modelos de classes da entidade conforme seu banco de dados. 
   fique a vontade para inserir mais propiedades 
 de validações.
 ![Legenda](https://i.ibb.co/y0m4TkN/img-7.png)
Figura 7

Vamos fazer um teste para ver se o INSERT esta funcionando. 
 ![Legenda](https://i.ibb.co/k3fpBfp/img-8.png)

Figura 8
repare que os dados foram inseridos com sucesso.
 ![Legenda](https://i.ibb.co/1rX0D3p/img-10.png)

**bom, espero ter ajudado com este breve resumo sobre #engenharia #reversa de um #banco de dados existe usando o Code-First, Fluent API e Entity Framework**.

abs
 
**Referências**
https://docs.microsoft.com/pt-br/dotnet/api/system.componentmodel.dataannotations?view=netframework-4.8
https://marketplace.visualstudio.com/items?itemName=ErikEJ.EntityFramework6PowerToolsCommunityEdition















 

 





    
    
