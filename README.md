## Projeto "Postman"

- Autor Moisés Ademir Chiaretto
  
- Descrição das explicações de cada item da 'estrutura da Collection" **Test** desenvolvida'.

- Objetivo:

  - Criar testes com o Postman com Javascript, JWT, CRUD, e os verbos HTTP (Get, Post, Put, Patch, Delete).

  - Utilizar a ferramenta **_Newman_** para executar a **Collection "Test" e as Environments (variáveis) "API_REST_gorest.co.in"**, ambos criados no Postman.

  
**Postman v11.0.12**

<br>

|Postman        |API            |JSON          |Newman           |QA - Tester      |
|---------------|---------------|--------------|-----------------|-----------------|
| ![01_Logo_Postman](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/9a62ed55-bcd1-4297-abc6-380c7dc6153d) | ![02_API_REST](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/13f3c6ca-d172-4a75-baa9-f57e3afedc4f) | <img width="164" alt="04_JSON" src="https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/4f05e9f8-2810-41c6-8393-facb1d962581"> | <img width="158" alt="00_Newman_Postman" src="https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/b36c772b-9616-433e-8c46-23c94d0717e1"> | ![14_QA_TESTER](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/22073e10-e1fa-4071-9ebb-1997f6e65bb3) |

<br>


## Estrutura da Collection "Test"

- No Painel à esquerda encontra-se o botão **Collection**, este selecionado irá listar as **Collections do Worksapce** aberto / sendo utilizado.

![03_Estutura_da_Collection_Environment_02](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/0d398e15-07dc-4b8f-889f-248cd60f2f53)


## Exemplo das Environments (variáveis) "API_REST_gorest.co.in" utilizadas na Collection "Test"


- No Painel à esquerda encontra-se o botão **Environments**, este selecionado irá listar as **Environments do Worksapce** aberto / sendo utilizado.

![04_Environment_02](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/08a64fbe-9c5a-49b6-b8d3-9d6d4dab2b31)


- No canto superior direito do Postman encontra-se o botão **"Environment quick look"**, conforme a imagem abaixo.
- Este botão serve para criar as **"Environments ou Variáveis"** a serem utilizadas nas **"requests"** da Collection "Test", facilitando assim uma possível alteração de URL, Endppoint, por exemplo.

![04_Environment](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/b5013695-93b0-436e-89a6-3fa1698c5437)


## Método, URL e Endpoint

- Selecionar qual o verbo HTTP, ou seja, o método a ser utilizado, no exemplo da imagem abaixo é o método **GET.**

- Informar a URL e o Endpoint, porém não da forma abaixo:

    - https://gorest.co.in/public/v2/users
 
    - **url** = https://gorest.co.in/
 
    - **endpoint** = public/v2/users/
 
  - E sim utilizando as **"Environments ou Variáveis"** criadas, por exemplo:

     - **{{url}}{{endpoint}}**
   
     - **importante observar** que as variáveis sempre são informadas **entre chaves dupla.**
   
![05_Metodo_URL_EndPoint](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/f081250d-63b2-4f06-9d57-2f2c1a97845b)

   
  - Documentação desta API REST.
 
     - https://gorest.co.in   

   
## Botão Send

  * Botão **Send** utilizado para executar o **método GET** da request selecionado **GET ALL**

  ![06_Botao_Send](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/f5d957dd-5a6b-4b55-94cc-01d81c9da05c)

## Response - Guia Body 

  - Exibe o resultado da requisição ou "request" da API Rest.

  ![07_Response_Guia_Body](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/8130d9fb-48a8-4cf3-ad22-cd247655aed3)


## Response - Guia Tests Results

  - Exibe o resultado referente ao **Script (código desenvolvido para os asserts).**

  ![08_Response_Guia_Test_Results](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/3e695b05-663f-4e9a-b4ef-65abdc70fa5e)


## Response - Console

  - Exibe no **Console** o resultado das execuções de requisições da API Rest e também o que foi enviando para impressão no console, usado no **Script**, usando o seguinte comando:

  **console.log("Os dados retornados não estão em um formato de array.");**

  ![10_Botao_Console](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/55e3b022-ffbf-41bd-96ed-21b402155442)

  ![09_Botao_Console](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/4db46552-7d00-4489-a7c7-3707e4142c25)


## Guia Authorization

- Selecionar no campo **Auth Type** a opção igual a **Bearer Token** é permitido a autorização para conexão a API [https://gorest.co.in/public/v2/users]

![11_Guia_Authorization](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/f14b8380-537a-490a-a5db-f28799bf26f9)


## Guia Headers

  - Informar no campo da coluna **Key** o texto igual a **Authorization**

  - Informar no campo da coluna **Value** o texto igual a **Bearer b7e0f9be923eabf55779250a1266ee97af8c9a99adc308e.............**

  - Desta forma informando o **Token** gerado é possível a autorização para conexão a API [https://gorest.co.in/public/v2/users]


![12_Guia_Headers](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/b8be78ed-0c46-4da7-8136-489613fcf0aa)



## Guia Body

  - Selecionar a opção **raw**

  - A opção "raw" no Postman é usada para enviar dados brutos no corpo de uma solicitação HTTP. Isso significa que você pode enviar dados no formato que desejar, como JSON, XML, texto simples, etc.

  - Selecionar a opção **JSON**

  - A opção "JSON" no Postman é uma maneira conveniente de enviar dados no formato JSON no corpo de uma solicitação HTTP.

  - **Observe o exemplo abaixo**, enviando dados com o **Método Post**

  ![13_Guia_Body](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/6652edf1-c264-42c3-a542-fd1bc6d171d2)


## Guia Scripts

  - A guia **"Scripts"** no Postman é uma área onde você pode escrever código JavaScript para automatizar e personalizar o comportamento das solicitações HTTP.

  - A imagem abaixo exibe um exemplo do **código JavaScript para automatizar os testes.**

![14_Guia_Scripts](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/eec05d9c-7315-4132-ad88-ef3a43f57930)


## Guia Test Results

  - Exibe o resultado da automatização dos testes na **"Guia Scripts"**

  - A imagem abaixo exibe um exmplo dos passos executados.


![15_Guia_Test_Results](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/a3091032-2eaa-46ae-b549-174f174595f4)


## Run Collection

  - Executando todas as **requests da collection**

  - Clicar com o botão direito sobre o nome da collection **Test**, clicar na opção **Run Collection**

  ![16_Run_Collection](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/0da1b79e-ce8e-4101-b550-575cd06e4f62)


  - Após clicar na opção **Run Collection** será exibida a imagem abaixo para a execução da coleection.

  - Selecionar quais as **requets** você deseja excutar na collection.

  - Clicar no botao **Run Test**

  ![17_Run_Collection](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/03acba4e-15f6-4988-a044-3a744960f41f)


- **Observe** as imagens abaixo o resultado da execução de **cada request** da collection.

|Telas de Execução da Collection "Test" em Postman   |    |    |    |
|----------------------------------------------------|----|----|----|
| ![18_Run_Collection](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/909c1e4a-4aa7-49c1-8c91-87427b19bc53) | ![19_Run_Collection](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/db4b2948-e2a3-4435-be83-f29f5955d9bd) | ![20_Run_Collection](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/b7b0ddee-726a-46a8-978b-c6a696c76c8d) | ![21_Run_Collection](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/17fb0b58-e885-46de-b9d5-070fd2af0092) |
<br>

***

## Newman
<br>
O Newman é uma ferramenta de linha de comando que executa coleções de testes do Postman, permitindo automação e integração contínua de testes de API, incluindo a aplicação e manipulação de variáveis definidas no ambiente do Postman.
<br>

### Instalar o Newman no Prompt de Comando como Administrador
<br>

```

npm install -g newman


```
<br>

## Validar se a instalação do "Newman" foi realizada corretamente

**_Digitar no Prompt de Comando como Administrador_**
<br>

```

newman --version


```
<br>

<img width="182" alt="00_Newman_Version" src="https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/6c6c0e6f-130b-4a8e-b838-ba3a2e359117">


<br>

### Exportar a Collection "Test"
<br>
<img width="332" alt="000_Export_Colletion" src="https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/e0393291-a4fa-4fc1-9846-7ff11430378e">

<br>

### Exportar as Environments (variáveis) "API_REST_gorest.co.in"
<br>

|Exportando as Environments (variáveis) "API_REST_gorest.co.in"  |            |
|----------------------------------------------------------------|------------|
| <img width="543" alt="00_Edit_Environments" src="https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/b1a9c6d1-3b58-4f99-a933-1712d184446b"> | <img width="618" alt="00_Export_Environments" src="https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/7703943a-379e-4826-be28-65cb32a8c9ef"> |

<br>
### Execução em _"Newman"_ da Collection "Test" e das Environments (variáveis) "API_REST_gorest.co.in"

**_Digitar no Prompt de Comando como Administrador_**

<br>

```

newman run Test.postman_collection.json --environment API_REST_gorest.co.in.postman_environment.json


```
<br>
<br>

### Resultado da execução utilizando a ferramenta "_Newman"_ da Collection "Test" e das Environments (variáveis) "API_REST_gorest.co.in"
<br>

|Resultado da execução utilizando a ferramenta "_Newman"         |            |          |
|----------------------------------------------------------------|------------|----------|
| <img width="459" alt="01_Execucao_Newman" src="https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/eb4359ad-9d02-4d84-82fe-bac16e97f576"> | <img width="420" alt="02_Execucao_Newman" src="https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/c4823f89-154f-4cc7-81cb-ec94af46de25"> | <img width="357" alt="03_Execucao_Newman" src="https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/6a4e3b48-e30c-4e3f-ba11-abe0fcbe0e6a"> |

<br>
<br>

