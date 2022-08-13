# Loja virtual - Venda de jogos (mídia física)

O Escopo do projeto será desenvolver uma página web e no qual o principal objetivo é oferecer aos usuários uma interface para que seja realizado compras e vendas de jogos eletrônicos.
O Brasil é um dos maiores mercados de videogames do mundo, e muitos dos consumidores adquirem algum jogo, terminam e gostariam de trocá-lo por algum novo ou revendê-lo. Por outro lado, há consumidores que gostariam de adquirir novos jogos 
com preços mais acessíveis sem se importar se já foram usados, ou mesmo de contactar vendedores de lojas varejistas menores para comparação de preços entre produtos novos, e também produtos usados.
A intenção da plataforma é prover o encontro do nicho de consumidores de jogos mídia física, permitindo com que seja catalogado jogos e vendedores. De tal forma que por uma interface simples, segurança das transações, sigilo e confiabilidade das informações seja facilitado aos jogadores a compra e venda desses produtos específicos.

## 1 Funcionalidades

Funcionalidades a serem desenvolvidas:

- Login para dois tipos de usuários: compradores e vendedores
- Criação de anúncio de venda
- Carrinho de compras
- Estimativa de frete
- Link com plataforma de pagamento
- Criação de mecanismo de busca

## 2 User Story Map
![image](https://user-images.githubusercontent.com/68930353/183538830-20e7aa2e-3bd7-4f75-90a3-91ff612f7685.png)
![image](https://user-images.githubusercontent.com/68930353/183538839-87e291f1-97d1-4024-bb92-6d6f8baa17fd.png)

## 3 Requisitos não funcionais

- Menus simples e bem estruturados: A navegação por parte dos usuários deve 
ser simples e intuitiva, melhorando a usabilidade e promovendo um maior interesse 
pelo layout da página.
- Interoperabilidade: O site deve possuir capacidade de rodar nos principais 
browsers, e também a capacidade de realizar comunicação com serviços de cartão 
de crédito.
- Segurança das informações pessoais: O site não deve expor as informações 
pessoais dos usuários

## 4 Casos de Uso

### 4.1 Pagina Inicial
#### 4.1.1 Breve Descrição
Página de acesso ao website com as informações de navegação.
#### 4.1.2 Atores
Consumidor e Administrador.
#### 4.1.3 Pré-Condições
Nenhuma pré-condição especial é requerida.
#### 4.1.4 Fluxo de Eventos
Nesta página, quando o usuário entrar no website ele verá os itens em destaque para venda.
Há também uma barra de menu na parte de cima com as opções de navegação, um campo para pesquisas e uma opção de login.
A barra de menu contará com os seguintes botões de navegação: Home, Plataforma, Login e Carrinho
#### 4.1.5 Pós-Condições
Não aplicável.


### 4.2 Pesquisar
#### 4.2.1 Breve Descrição
Campo destinado a se inserir uma palavra-chave e o site lhe mostrar os resultados relativos ao que se procurava.
#### 4.2.2 Atores
Consumidor, Vendedor e Administrador.
#### 4.2.3 Pré-Condições
Os atores deverão estar na página principal ou nas páginas referentes aos catálogos de produtos para ter acesso a esta função.
#### 4.2.4 Fluxo de Eventos
1. O ator informa, no campo fornecido pelo sistema, o seguinte dado: Nome do produto, nome da plataforma ou alguma palavra-chave que possa levar ao produto desejado e após isso clica no botão pesquisar.
2. O sistema verifica a palavra-chave informada.
3. O sistema informa ao operador uma lista de produtos relativos àquilo que foi procurado.
#### 4.2.5 Pós-Condições
Se encontrado algum produto referente a palavra-chave procurada, ele deve aparecer em lista para o usuário.
Se não encontrado, o sistema informará que não há itens relacionados à pesquisa.


### 4.3 Plataforma
#### 4.3.1 Breve Descrição
Botão da barra de menu, na qual há opção por nome do console do videogame desejado. Ao clicar no nome abrirá uma página com lista dos jogos à venda para a determinada plataforma.
#### 4.3.2 Atores
Consumidor, Vendedor e Administrador.
#### 4.3.3 Pré-Condições
Nenhuma pré-condição especial é requerida.
#### 4.3.4 Fluxo de Eventos
O Ator clica na opção Plataforma na barra de menus, a seguir deve escolher o console desejado para que seja listado os produtos.
#### 4.3.5 Pós-Condições
Clicado na opção será mostrado as opções de consoles a ser escolhido


### 4.4 Login 
#### 4.3.1 Breve Descrição
Local destinado ao login no site, digitando o nome de usuário e senha cadastrados. É também onde faz o logout.
#### 4.3.2 Atores
Consumidor, Vendedor e Administrador.
#### 4.3.3 Pré-Condições
Os atores devem ter o cadastro prévio no site.
#### 4.3.4 Fluxo de Eventos
1.O ator fornece seu nome de usuário cadastrado.
2.O ator digita sua senha.
3.Clica no botão login para acessar.
4.O sistema verifica se o login é válido.
#### 4.3.5 Pós-Condições
Ator logado no sistema, podendo atuar no site com identificação.


### 4.5 Efetuar cadastro
#### 4.3.1 Breve Descrição
Destina-se ao cadastramento de novos usuários
#### 4.3.2 Atores
Consumidor, Vendedor e Administrador.
#### 4.3.3 Pré-Condições
Nenhuma pré-condição especial é requerida.
#### 4.3.4 Fluxo de Eventos
1.Ator clica no link “Cadastro” na página inicial.
2.É redirecionado para a página de cadastro.
3.O ator preenche os campos de Nome de Usuário, Email, Senha e Confirmar Senha.
4.É verificado se o email é válido.
5. O sistema verifica no banco de dados se o nome de usuário é inédito
6. O cadastro é realizado e o usuário é redirecionado para Home do site com a conta logada.
#### 4.3.5 Pós-Condições
O sistema informa “Usuário cadastrado”, se todas as condições forem cumpridas


### 4.6 Adicionar produto ao carrinho de compras
#### 4.3.1 Breve Descrição
Adicionar o produto selecionado ao carrinho de compras, local que organiza e consolida todos os produtos desejados.
#### 4.3.2 Atores
Consumidor e Administrador.
#### 4.3.3 Pré-Condições
Os compradores podem ser visitantes ou possuir cadastro, não necessariamente precisam estar previamente logados no sistema.
#### 4.3.4 Fluxo de Eventos
1.Ao encontrar o produto desejado, o comprador pode clicar na função “Adicionar ao carrinho”.
2.O produto é então adicionado ao carrinho.
#### 4.3.5 Pós-Condições
A cada item adicionado o número de itens no carrinho deve ser atualizado.


### 4.7 Pagamento
#### 4.3.1 Breve Descrição
Área destinada ao pagamento do produto.
#### 4.3.2 Atores
Consumidor e Administrador.
#### 4.3.3 Pré-Condições
1.Ter ao menos um produto selecionado.
2.O cliente deve ter uma conta na Pag Seguro para realizar a 
ação.
#### 4.3.4 Fluxo de Eventos
1.Com o(s) produto(s) selecionado(s) no “carrinho”, o usuário deverá clicar 
em comprar.
2.Na área de pagamento, o comprador deve selecionar o meio de 
pagamento fornecido pela Pag Seguro (cartão de débito/crédito, boleto bancário, etc).
3.O consumidor efetua o pagamento.
4.O pagamento é aceito.
#### 4.3.5 Pós-Condições
Produtos vão para página de Área do Usuário, onde pode-se 
acompanhar a entrega do mesmo.


### 4.8 Produto
#### 4.3.1 Breve Descrição
Descrição das informações e preço do produto, quando nele for clicado.
#### 4.3.2 Atores
Consumidor, Vendedor e Administrador.
#### 4.3.3 Pré-Condições
Nenhuma pré-condição especial é requerida.
#### 4.3.4 Fluxo de Eventos
A partir de pesquisa ou página inicial, o usuário deverá clicar em “Visualizar” sobre o produto.
Na página do produto o usuário decide se irá realizar a compra, salvar no Carrinho ou se prosseguirá para alguma outra página através dos botões da barra de menu
#### 4.3.5 Pós-Condições
Não aplicável.

