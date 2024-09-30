# Tranca ou não?

## Desenvolvedores
Valdir Júnior Petrarca de Lima. RA:1969935.
Leandro Otero de Godoy. RA: 1972672.
Moises Júnior Bassiga da Cruz Marques. RA: 1967447.
Italo Gabriel Vieira da Cruz. 1972431.
Miguel Soares da Silva Oliveira. RA: 1967376.

## O que é o nosso projeto?
O nosso projeto é visado em localizar e chamar a atenção do cliente. Quando a Tray foi pela primeira vez na faculdade, eles apresentaram algumas dificuldades, e uma das dificuldades que eles apresentaram foi a localização de clientes que apenas entram no site deles e não realizam um cadastro, ou até mesmo um pré-cadastro. E esse ponto chamou bastante atenção do grupo. Pedimos ajuda e ideias para alguns professores, e eles falaram que o prejeto era um pouco complexo de se fazer e demoraria muito para fazer. Então decidimos continuar com esse projeto e fazer algo simples, mas que daria certo. Fizemos uma loja de Tenis a "SneakerWorld", onde de alguma forma teriamos que chamar a atenção do cliente que entrasse em nosso site. O time estava sem ideia do que fazer para chamar a atenção do cliente. Então apresentamos a nosso projeto para a Tray com uma simples mensagem, dizendo para o cliente realizar o cadastro que ele ganharia 10% de desconto na primeira compra. No final da apresentação, um intefrante da Tray nos deu a ideia de fazer um Pop-up para que aparecesse a mensagem e direcionar o cliente para fazer o cadastro. O time gostou da ideia e estamos desenvolvendo o Pop-up, ele não esta pronto, pois ainda estamos com dificuldade no desenvolvimento do Pop-up.

Conclusão: Nosso projeto é visado na localização do cliente. Estamos no desenvolvimento do Pop-up para chamar a atenção do cliente e fazer ele realizar o cadastro, para caso ele entre em nosso site, faça o cadastro e ganhe a porcentagem de desconto, mas mesmo assim ele não faça a compra, a gente ja tem os dados dele para entrar em contato e assim localizar ele quando a gente quiser.

## Recomandação.

Recomendamos o [VSCode](https://code.visualstudio.com/) para você mexer no nosso projeto.

## O que você precisa fazer para entrar no codigo. 

Siga as instruções a baixo.

### Primeiro passo

Depois de baixar o projeto e extraido ele, você ira abrir a pasta e irá dar o comando "cmd" para abrir o terminal.

![Imagem comando "cmd"](https://github.com/user-attachments/assets/1cbf671c-12a8-4d92-b5a4-6730ba46e1b5)

### Segundo passo

Com o terminal aberto, iremos dar o comando a baixo, para instalar todos os pacotes no Node Package Manager.

```sh
npm install
```

![Imagem comando "npm install"](https://github.com/user-attachments/assets/60c342af-aa03-4c9a-9ce0-ab2e68f17c73)


### Terceiro passo

Depois de instalado os pacotes, iremos dar o comando a baixo para executar o script dev no arquivo package.json do Gerenciador de pacotes.

```sh
npm run dev
```

!["npm run dev"](https://github.com/user-attachments/assets/9ab34dc4-2a57-45bc-ac2d-b2a7cacb690e)


### Quarto passo

Depois de executar o comando a cima, irá aparcer o localhost do nosso projeto, por exemplo:"http://localhost:5173/". Você irá copiar esse localhost e irá colar no seu navegador.


![imagem do localhost](https://github.com/user-attachments/assets/f30932a5-5fc8-4a40-af20-b427d66886ce)

### quinto passo

Depois de colado a url no seu navegador 
![Imagem colando a url no navegador](https://github.com/user-attachments/assets/17b6cd1e-6fdb-4a2b-a3f7-3afe15b49ae7), ira abrir nosso projeto na pagina inicial.

A nossa pagina inicial tem um nav-bar para o cliente navegar em nosso site e la em baixo algumas marcas para ela filtrar os tenis por marca.
![Imagem tela inicial](https://github.com/user-attachments/assets/09c40737-3118-4894-8084-792dd4ec8459)

Nossa tela de cadastro, é uma tela simples onde o cliente se cadastra colocando nome, email e senha,
![Imagem tela castro](https://github.com/user-attachments/assets/d06d372e-facc-4616-b393-f1164337a674)

Nossa tela de produtos existe todos os produtos que tem la em baixo na tela inicial ![imagem tela produtos](https://github.com/user-attachments/assets/76e66a9a-7fb5-453e-bca7-6989401bd879)

No Nav-bar no canto superior direito, tem um campo escrito "filtre por marca": ![tela Imagem filtre por marca](https://github.com/user-attachments/assets/f84e153f-6806-433d-9a73-671c310d2e7a), se o cliente clicar na marca "puma", aparecerá todos os tenis da puma...

Nossa tela de carrinho ainda esta em "construção" ![Imagem tela carrinho](https://github.com/user-attachments/assets/44abc1d7-ca1d-47ff-bcd9-3be5e22c0bd0). 

## backend

Backend: https://github.com/JuniorLima04/trayprojeto45.git

## Primeiro passo
(é preciso instalar o visual estudio 2022)

abrindo a arquuivo ![pasta back](https://github.com/user-attachments/assets/9dbacfe5-680c-406e-b442-a6ca42be66a1), dará duplo clique e entrara no visual estudio 2022

## segundo passo

Depois de aberto o arquivo no visual ira aparecer essa tela ![back aberto](https://github.com/user-attachments/assets/3e26a7b5-bda8-4c0c-a060-26a88a8dd32b).

logo em seguida, você ira instalar na sua maquina um MySQL(eu indico MySQL Workbench, que foi o que realizamos o projeto). 

em seguida você ira la no gerenciador de soluções do backend e vai clicar em "trayprojeto45DbContext.cs" como indica na imagem: ![imagem gerenciador de soluções](https://github.com/user-attachments/assets/a31c554d-821e-4969-8271-e847cda35421), 

e ira mudar o password que você colocou quando configurou o MySQL Workbench:![Mudando a senha do seu MySQL](https://github.com/user-attachments/assets/52628406-8e60-45eb-a99f-7dc1f7740d2f) (Colocar a senha que você criou no workbench)

## Terceiro passo

Depois de instalado o MySQL Workbench e totalmente configurado e senha mudada, você ira entrar no backend e ir em "exibir" e abrir o "terminal" ![Abrindo o terminal no visual](https://github.com/user-attachments/assets/170b0bb9-1bfe-44ee-9570-5c7a365c7508).

depois iremos excutar esse comando no terminal para instalar a ferramenta Entity Framework.

```sh
dotnet tool install --global dotnet-ef
```

## Quarto passo

Você ira executar o comando a baixo no terminal, que é utilizado para atualizar o banco de dados com a migração mais recente. 

```sh
dotnet ef database update
```

## Quinto passo

em seguinda você entrará no local instance no MySQL,que entrará na base de dados: 
![entrando na base de dados](https://github.com/user-attachments/assets/3c465b9f-c9a6-445e-9be8-9fc6ad9c4e5a)

Em seguida, você ira notar que com o comando "dotnet ef database update" vai subir a base de dados no MySQL: 
![Captura de tela 2024-09-30 200806](https://github.com/user-attachments/assets/f0308aa1-90bd-4bde-97cc-da197703c15a)

## sexto passo

Depois ira apertar no "https", no visual studio 2022 do backend, que esta marcado nessa imagem: 
![imagem marcado "https"](https://github.com/user-attachments/assets/ba4cd5a5-f270-4701-a83e-d6a021fe952a). 

Depois de executar o projeto ele ira ficar assim: 
![imagem depois de execução](https://github.com/user-attachments/assets/0f867a21-5ae8-4d54-8e9a-74376265d307)
que é um sinal que o backend esta em execução. 

## Setimo passo

Em seguida, você pode entrar no nosso sistema na tela de cadastro e realizar um cadastro que ira bater frontend com backend e ira as informações para o banco de dados:
![cadastrando um cliente](https://github.com/user-attachments/assets/2a751385-c6c2-4af5-b459-ca6d165d73eb)

![info. Cliente banco de dados](https://github.com/user-attachments/assets/d4696540-cfec-4b49-8aa2-e503934693bf)

Estamos no desenvolvimento do Pop-up para chamar a atenção do cliente e direcionar ele para a tela de cadastro.

### O que cada desenvolvedor fez.

Os desenvolvedores Leandro Otero de Godoy, RA:1972672 e Valdir Júnior Petrarca de Lima. RA:1969935, são os dois desenvolvedores que estão a frente do projeto. O Leandro passou o projeto de HTML para VUE. começou estruturando o front da tela inicial e do cadastro e auxiliando na estruturação do backend, o valdir foi quem estruturou a tela do produtos, carinho e o linkando front com back do tela de cadastro.

Miguel Soares da Silva Oliveira - R.A: 1967376 

	Realizei o auxilio dentro do projeto, juntamente aos demais integrantes do grupo, auxiliando na melhoria do sistema, visando, um melhor desenvolvimento nas paginas Front-End.	
	Foi desenvolvido uma melhoria na pagina inical, realizando a manutenação na página Home, com a edição do Logo SnakeWorld, também editando os botões dentro da Pagina.
	Juntamente com os demais integrantes realizamos a edição de pontos que precisam ser melhorados, como o carrinho, formulario de pedido, também realizando a manutenção da pagina de cadastro, para um melhor desenolvimento.


*Não foi realizado nennhum Comit em meu nome, pois, decorrente a minha maquina não estar funcionando, conforme lhe encaminhei via WhatsApp Professor, sendo assim, solicitei para os demais integrantes adicionarem Comits nas paginas em que auxiliei ou realizei a melhoria dentro do código*

Moises Júnior Bassiga da Cruz Marques. RA: 1967447.   realizou a parte do back and, alterando alguns códigos pra deixar o site mais limpo e menos poluído pra quando o cliente acessar ficar algo fácil e prático.

Italo Gabriel Vieira da Cruz. 1972431. Foi auxiliando o Moises no backend e realizando o estilos do site.

