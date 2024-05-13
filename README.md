## Projeto "Postman"
- Autor Moisés Ademir Chiaretto
  
- Descrição das explicações de cada item da 'estrutura da Collection" **Test** desenvolvida'.
  
- **Postman v11.0.12**

![01_Logo_Postman](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/9a62ed55-bcd1-4297-abc6-380c7dc6153d)

![02_API_REST](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/13f3c6ca-d172-4a75-baa9-f57e3afedc4f)



## Estrutura da Collection "Test"

- No Painel à esquerda encontra-se o botão **Collection**, este selecionado irá listar as **Collections do Worksapce** aberto / sendo utilizado.

![03_Estutura_da_Collection_Environment_02](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/0d398e15-07dc-4b8f-889f-248cd60f2f53)


## Exemplo das Environments (variáveis) "API_REST_gorest.co.in" utilizadas na Collection "Test"

- No Painel à esquerda encontra-se o botão **Environments**, este selecionado irá listar as **Environments do Worksapce** aberto / sendo utilizado.

![04_Environment_02](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/f63aa95b-fcaf-403e-a10c-23bd24e86436)


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



    
