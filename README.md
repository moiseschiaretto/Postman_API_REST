## Projeto "Postman"
- Autor Moisés Ademir Chiaretto
  
- Descrição das explicações de cada item da 'estrutura da Collection" **Test** desenvolvida'.
  
- **Postman v11.0.12**

![01_Logo_Postman](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/9a62ed55-bcd1-4297-abc6-380c7dc6153d)

![02_API_REST](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/13f3c6ca-d172-4a75-baa9-f57e3afedc4f)



## Estrutura da Collection "Test"

![03_Estutura_da_Collection_Environment_02](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/8c279a83-4494-4576-8f43-5a0da403c5ad)



## Exemplo das Environments (variáveis) "API_REST_gorest.co.in" utilizadas na Collection "Test"

- No canto superior direito do Postman encontra-se o botão **"Environment quick look"**, conforme a imagem abaixo.
- Este botão serve para criar as **"Environments ou Variáveis"** a serem utilizadas nas **"requests"** da Collection "Test", facilitando assim uma possível alteração de URL, Endppoint, por exemplo.

![04_Environment](https://github.com/moiseschiaretto/Postman_API_REST/assets/84775466/b5013695-93b0-436e-89a6-3fa1698c5437)


## Método, URL e Endpoint

- Selecionar qual o verbo HTTP, ou seja, o método a ser utilizado, no exemplo da imagem abaixo é o método **GET.**

- Informar a URL e o Endpoint, porém não da forma abaixo:

    - https://gorest.co.in/public/v2/users
 
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


## Guia Body


## Guia Scripts



    
