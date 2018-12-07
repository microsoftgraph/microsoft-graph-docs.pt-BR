---
title: Usar a API de Pessoas no Microsoft Graph para obter informações sobre as pessoas mais relevantes para você
description: Os aplicativos do Microsoft Graph podem usar a API de Pessoas para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório de uma organização e as pessoas de comunicações recentes (como emails e Skype). Além de gerar essas informações, a API de Pessoas também fornece suporte para pesquisa de correspondência difusa e a capacidade de recuperar a lista de usuários relevantes para outro usuário na organização do usuário conectado.
ms.date: 12/04/2018
ms.openlocfilehash: b01ca4538c3155bbb30224b1f92d6e7ae55c5878
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156051"
---
# <a name="use-the-people-api-in-microsoft-graph-to-get-information-about-the-people-most-relevant-to-you"></a><span data-ttu-id="83043-106">Usar a API de Pessoas no Microsoft Graph para obter informações sobre as pessoas mais relevantes para você</span><span class="sxs-lookup"><span data-stu-id="83043-106">Use the People API in Microsoft Graph to get information about the people most relevant to you</span></span>

<span data-ttu-id="83043-p102">Os aplicativos do Microsoft Graph podem usar a API de Pessoas para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório de uma organização e as pessoas de comunicações recentes (como emails e Skype). Além de gerar essas informações, a API de Pessoas também fornece suporte para pesquisa de correspondência difusa e a capacidade de recuperar a lista de usuários relevantes para outro usuário na organização do usuário conectado. A API de Pessoas é particularmente útil para cenários de seleção de pessoas, como ao redigir um email ou criar uma reunião. Por exemplo, você pode usar a API de Pessoas em cenários de redação de emails.</span><span class="sxs-lookup"><span data-stu-id="83043-p102">Microsoft Graph applications can use the People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. People can be local contacts, contacts from social networking or from an organization’s directory, and people from recent communications (such as email and Skype). Along with generating this insight, the People API also provides fuzzy matching search support and the ability to retrieve the list of users relevant to another user in the signed-in user's organization. The People API is particularly useful for people picking scenarios, such as composing an email or creating a meeting. For example, you can use the People API in email compose scenarios.</span></span>

## <a name="authorization"></a><span data-ttu-id="83043-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="83043-113">Authorization</span></span>

<span data-ttu-id="83043-114">Para chamar a API de Pessoas no Microsoft Graph, seu aplicativo precisará das permissões adequadas:</span><span class="sxs-lookup"><span data-stu-id="83043-114">To call the People API in Microsoft Graph, your app will need the appropriate permissions:</span></span>

* <span data-ttu-id="83043-p103">People.Read – use para fazer chamadas gerais da API de Pessoas; por exemplo, `https://graph.microsoft.com/v1.0/me/people/`. People.Read requer o consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="83043-p103">People.Read - Use to make general People API calls; for example, `https://graph.microsoft.com/v1.0/me/people/`. People.Read requires end user consent.</span></span>
* <span data-ttu-id="83043-117">People.Read.All - necessária para recuperar as pessoas mais relevantes para um usuário especificado nas chamadas (`https://graph.microsoft.com/v1.0/users('{id}')/people`) da organização do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="83043-117">People.Read.All - Required to retrieve the people most relevant to a specified user in the signed-in user’s organization (`https://graph.microsoft.com/v1.0/users('{id}')/people`'{id}')/people) calls. People.Read.All requires admin consent.</span></span> <span data-ttu-id="83043-118">People.Read.All requer o consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="83043-118">People.Read.All requires admin consent.</span></span>

## <a name="browse-people"></a><span data-ttu-id="83043-119">Procurar pessoas</span><span class="sxs-lookup"><span data-stu-id="83043-119">Browse people</span></span>

<span data-ttu-id="83043-p105">As solicitações nesta seção obtém as pessoas mais relevantes para o usuário conectado (`/me`) ou para um usuário específico na organização do usuário conectado. Essas solicitações exigem a permissão People.Read ou People.Read.All, respectivamente. Por padrão, cada resposta retorna 10 registros, mas você pode alterar isso usando o parâmetro de consulta *$top*.</span><span class="sxs-lookup"><span data-stu-id="83043-p105">The requests in this section get the people most relevant to the signed-in user (`/me`), or to a specific user in the signed-in user’s organization. These requests require the People.Read or People.Read.All permission respectively. By default, each response returns 10 records, but you can change this by using the *$top* query parameter.</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="83043-123">Obter uma coleção de pessoas relevantes</span><span class="sxs-lookup"><span data-stu-id="83043-123">Get a collection of relevant people</span></span>

<span data-ttu-id="83043-124">A solicitação a seguir obtém as pessoas mais relevantes para o usuário conectado (`/me`), com base nos padrões de comunicação e colaboração e nas relações comerciais.</span><span class="sxs-lookup"><span data-stu-id="83043-124">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="83043-p106">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro de consulta *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="83043-p106">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye",
      "givenName": "Lorrie",
      "surname": "Frye",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Paralegal",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "20/1109",
      "profession": "",
      "userPrincipalName": "LorrieF@contoso.onmicrosoft.com",
      "imAddress": "sip:LorrieF@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 980 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
      "displayName": "Maynard Denman",
      "givenName": "Maynard",
      "surname": "Denman",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Web Marketing Manager",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "20/1101",
      "profession": "",
      "userPrincipalName": "MaynardD@contoso.onmicrosoft.com",
      "imAddress": "sip:MaynardD@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "MaynardD@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 918 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
      "displayName": "Darrel Halsey",
      "givenName": "Darrel",
      "surname": "Halsey",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Attorney",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "14/1102",
      "profession": "",
      "userPrincipalName": "DarrelH@contoso.onmicrosoft.com",
      "imAddress": "sip:DarrelH@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "DarrelH@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 205 555 0103"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="request-a-subsequent-page-of-people"></a><span data-ttu-id="83043-129">Solicitar uma página subsequente de pessoas</span><span class="sxs-lookup"><span data-stu-id="83043-129">Request a subsequent page of people</span></span>

<span data-ttu-id="83043-p107">Se a primeira resposta não contiver a lista completa das pessoas relevantes, você poderá fazer uma segunda solicitação usando *$top* e *$skip* para solicitar páginas adicionais de informações. Se a solicitação anterior tiver informações adicionais, a solicitação a seguir obterá a próxima página de pessoas do servidor.</span><span class="sxs-lookup"><span data-stu-id="83043-p107">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=3&$skip=10
```

<span data-ttu-id="83043-p108">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro de consulta *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="83043-p108">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1F28616D-BDFE-4080-8F06-03366A851688",
      "displayName": "Felix Coppola",
      "givenName": "Felix",
      "surname": "Coppola",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "CVP Legal",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "19/2109",
      "profession": "",
      "userPrincipalName": "FelixC@contoso.onmicrosoft.com",
      "imAddress": "sip:FelixC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "FelixC@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 309 555 0104"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "8A3FC021-6DBB-44AC-8884-B7B500CC260A",
      "displayName": "Lenora Rowland",
      "givenName": "Lenora",
      "surname": "Rowland",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Marketing Assistant",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "18/1106",
      "profession": "",
      "userPrincipalName": "LenoraR@contoso.onmicrosoft.com",
      "imAddress": "sip:LenoraR@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "LenoraR@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 954 555 0118"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "032C9919-4DF9-4715-8C46-4D0FAE7B3EB2",
      "displayName": "Manuel Collette",
      "givenName": "Manuel",
      "surname": "Collette",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Accountant II",
      "companyName": null,
      "yomiCompany": "",
      "department": "Finance",
      "officeLocation": "98/2202",
      "profession": "",
      "userPrincipalName": "ManuelC@contoso.onmicrosoft.com",
      "imAddress": "sip:ManuelC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "ManuelC@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+20 255501070"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="sort-the-response"></a><span data-ttu-id="83043-136">Classificar a resposta</span><span class="sxs-lookup"><span data-stu-id="83043-136">Sort the response</span></span>

<span data-ttu-id="83043-p109">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta ao usar o parâmetro *$orderby*. Essa consulta seleciona as pessoas mais relevantes para você, classifica-as por **displayName** e, em seguida, retorna as primeiras 10 pessoas na lista classificada.</span><span class="sxs-lookup"><span data-stu-id="83043-p109">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter. This query selects the people most relevant to you, sorts them by their **displayName**, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$orderby=displayName
```

<span data-ttu-id="83043-p110">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso ao usar o parâmetro *$top*. O exemplo a seguir usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="83043-p110">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. The following example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "818E29A1-E6BB-4EDA-AB20-8230B4B1E290",
      "displayName": "Adriana Ramos",
      "givenName": "Adriana",
      "surname": "Ramos",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Product Marketing Manager",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "18/2111",
      "profession": "",
      "userPrincipalName": "AdrianaR@contoso.onmicrosoft.com",
      "imAddress": "sip:AdrianaR@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "AdrianaR@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 425 555 0109"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "62633BAA-1CB9-4FA2-9B8F-55AB1840B69D",
      "displayName": "Alyce Cooley",
      "givenName": "Alyce",
      "surname": "Cooley",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Marketing Assistant",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "131/1104",
      "profession": "",
      "userPrincipalName": "AlyceC@contoso.onmicrosoft.com",
      "imAddress": "sip:AlyceC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "AlyceC@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 858 555 0110"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "6BB54D2C-EF20-48DA-ADD9-AE757DD30C4E",
      "displayName": "Alyssa Clarke",
      "givenName": "Alyssa",
      "surname": "Clarke",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Corporate Security Officer",
      "companyName": null,
      "yomiCompany": "",
      "department": "Operations",
      "officeLocation": "24/1106",
      "profession": "",
      "userPrincipalName": "AlyssaC@contoso.onmicrosoft.com",
      "imAddress": "sip:AlyssaC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "AlyssaC@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 262 555 0106"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="change-the-number-of-people-and-fields-returned"></a><span data-ttu-id="83043-144">Alterar o número de pessoas e campos retornados</span><span class="sxs-lookup"><span data-stu-id="83043-144">Change the number of people and fields returned</span></span>

<span data-ttu-id="83043-145">Você pode alterar o número de pessoas retornadas na resposta definindo o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="83043-145">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="83043-p111">O exemplo a seguir solicita as 1.000 pessoas mais relevantes para `/me`. A solicitação também limita a quantidade de dados enviados de volta do servidor solicitando somente o **displayName** da pessoa.</span><span class="sxs-lookup"><span data-stu-id="83043-p111">The following example requests the 1,000 people most relevant to `/me`. The request also limits the amount of data sent back from the server by requesting only the **displayName** of the person.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=1000&$Select=displayName
```

<span data-ttu-id="83043-148">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="83043-148">The following example shows the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye"
    },
    {
      "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
      "displayName": "Maynard Denman"
    },
    {
      "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
      "displayName": "Darrel Halsey"
    },
    {
      "id": "E3C5B235-DE15-4566-B7B1-7A8E32426540",
      "displayName": "Roscoe Seidel"
    },
    {
      "id": "6BB54D2C-EF20-48DA-ADD9-AE757DD30C4E",
      "displayName": "Alyssa Clarke"
    },
    {
      "id": "818E29A1-E6BB-4EDA-AB20-8230B4B1E290",
      "displayName": "Adriana Ramos"
    },
    {
      "id": "62633BAA-1CB9-4FA2-9B8F-55AB1840B69D",
      "displayName": "Alyce Cooley"
    },
    {
      "id": "6BB9CC1F-418D-4DDF-AB0C-6A1C4ABCDBF4",
      "displayName": "Wayne Leeper"
    },
    {
      "id": "E7D40AC5-0078-4575-B1F3-F738124C4BC9",
      "displayName": "Jan Travis"
    },
    {
      "id": "6F99D1CC-4FCC-49E4-9160-E8AB01BF3E83",
      "displayName": "Charlotte Delacruz"
    },
    {
      "id": "1F28616D-BDFE-4080-8F06-03366A851688",
      "displayName": "Felix Coppola"
    },
    {
      "id": "8A3FC021-6DBB-44AC-8884-B7B500CC260A",
      "displayName": "Lenora Rowland"
    },
    {
      "id": "032C9919-4DF9-4715-8C46-4D0FAE7B3EB2",
      "displayName": "Manuel Collette"
    }
  ]
}
```

### <a name="select-the-fields-to-return"></a><span data-ttu-id="83043-149">Selecione os campos para retornar</span><span class="sxs-lookup"><span data-stu-id="83043-149">Select the fields to return</span></span>

<span data-ttu-id="83043-p112">Você pode limitar a quantidade de dados retornados do servidor usando o parâmetro *$select* para escolher um ou mais campos. O campo `@odata.id` sempre é retornado.</span><span class="sxs-lookup"><span data-stu-id="83043-p112">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields. The `@odata.id` field is always returned.</span></span>

<span data-ttu-id="83043-152">O exemplo a seguir limita a resposta ao **displayName** e **scoredEmailAddresses** das 10 pessoas mais relevantes.</span><span class="sxs-lookup"><span data-stu-id="83043-152">The following example limits the response to the **displayName** and **scoredEmailAddresses** of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses
```

<span data-ttu-id="83043-p113">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="83043-p113">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    },
    {
      "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
      "displayName": "Maynard Denman",
      "scoredEmailAddresses": [
        {
          "address": "MaynardD@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    },
    {
      "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
      "displayName": "Darrel Halsey",
      "scoredEmailAddresses": [
        {
          "address": "DarrelH@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    }
  ]
}
```

### <a name="use-a-filter-to-limit-the-response"></a><span data-ttu-id="83043-157">Usar um filtro para limitar a resposta</span><span class="sxs-lookup"><span data-stu-id="83043-157">Use a filter to limit the response</span></span>

<span data-ttu-id="83043-158">Você pode usar o parâmetro *$filter* para limitar a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="83043-158">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="83043-159">A consulta a seguir limita a resposta a instâncias **person** com a propriedade **personType** com as atribuições de **person** como **classe** e **organizationUser** como **subclasse**.</span><span class="sxs-lookup"><span data-stu-id="83043-159">The following query limits the response to **person** instances with the **personType** property being assigned **person** as **class** and **organizationUser** as **subclass**.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$filter=personType/class eq 'Person' and personType/subclass eq 'OrganizationUser'
```

<span data-ttu-id="83043-p114">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="83043-p114">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye",
      "givenName": "Lorrie",
      "surname": "Frye",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Paralegal",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "20/1109",
      "profession": "",
      "userPrincipalName": "LorrieF@contoso.onmicrosoft.com",
      "imAddress": "sip:LorrieF@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 980 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
      "displayName": "Maynard Denman",
      "givenName": "Maynard",
      "surname": "Denman",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Web Marketing Manager",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "20/1101",
      "profession": "",
      "userPrincipalName": "MaynardD@contoso.onmicrosoft.com",
      "imAddress": "sip:MaynardD@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "MaynardD@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 918 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
      "displayName": "Darrel Halsey",
      "givenName": "Darrel",
      "surname": "Halsey",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Attorney",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "14/1102",
      "profession": "",
      "userPrincipalName": "DarrelH@contoso.onmicrosoft.com",
      "imAddress": "sip:DarrelH@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "DarrelH@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 205 555 0103"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="83043-164">Selecionar os campos a serem retornados em uma resposta filtrada</span><span class="sxs-lookup"><span data-stu-id="83043-164">Select the fields to return in a filtered response</span></span>

<span data-ttu-id="83043-165">Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="83043-165">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="83043-p115">O exemplo a seguir obtém **displayName** e **scoredEmailAddresses** das pessoas cujo nome de exibição corresponde ao nome especificado. Neste exemplo, somente as pessoas cujo nome para exibição corresponde a "Lorrie Frye" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="83043-p115">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="83043-168">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="83043-168">The following example shows the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    }
  ]
}
```

### <a name="browse-another-users-relevant-people"></a><span data-ttu-id="83043-169">Procurar pessoas relevantes de outro usuário</span><span class="sxs-lookup"><span data-stu-id="83043-169">Browse another user’s relevant people</span></span>

<span data-ttu-id="83043-170">A solicitação a seguir obtém as pessoas mais relevantes para outra pessoa na organização do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="83043-170">The following request gets the people most relevant to another person in the signed-in user's organization.</span></span> <span data-ttu-id="83043-171">Esta solicitação requer a permissão People.Read.All.</span><span class="sxs-lookup"><span data-stu-id="83043-171">This request requires the People.Read.All permission.</span></span> <span data-ttu-id="83043-172">Os parâmetros de consulta descritos nas seções acima também se aplicam.</span><span class="sxs-lookup"><span data-stu-id="83043-172">All the query parameters described in the above sections apply as well.</span></span>

<span data-ttu-id="83043-173">Neste exemplo, as pessoas relevantes de Vinícius Monte são exibidas.</span><span class="sxs-lookup"><span data-stu-id="83043-173">In this example, Roscoe Seidel's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="83043-p117">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro *$top*. O exemplo abaixo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="83043-p117">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. The example below uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "56155636-703F-47F2-B657-C83F01F49BBC",
      "displayName": "Clifton Clemente",
      "givenName": "Clifton",
      "surname": "Clemente",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Director",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "19/2106",
      "profession": "",
      "userPrincipalName": "CliftonC@contoso.onmicrosoft.com",
      "imAddress": "sip:CliftonC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "CliftonC@contoso.onmicrosoft.com",
          "relevanceScore": 20
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 309 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "6BF27D5A-AB4F-4C43-BED0-7DAD9EB0C1C4",
      "displayName": "Sheree Mitchell",
      "givenName": "Sheree",
      "surname": "Mitchell",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Product Manager",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "20/2107",
      "profession": "",
      "userPrincipalName": "ShereeM@contoso.onmicrosoft.com",
      "imAddress": "sip:ShereeM@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "ShereeM@contoso.onmicrosoft.com",
          "relevanceScore": 10
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 918 555 0107"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "B3E5302D-EAF0-4E8B-8C6C-A2AE64B4B163",
      "displayName": "Vincent Matney",
      "givenName": "Vincent",
      "surname": "Matney",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "CVP Engineering",
      "companyName": null,
      "yomiCompany": "",
      "department": "Engineering",
      "officeLocation": "23/2102",
      "profession": "",
      "userPrincipalName": "VincentM@contoso.onmicrosoft.com",
      "imAddress": "sip:VincentM@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "VincentM@contoso.onmicrosoft.com",
          "relevanceScore": 10
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 502 555 0102"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

## <a name="search-people"></a><span data-ttu-id="83043-178">Pesquisar pessoas</span><span class="sxs-lookup"><span data-stu-id="83043-178">Search people</span></span>

<span data-ttu-id="83043-p118">As solicitações nesta seção permitem procurar pessoas relevantes para o usuário conectado (`/me`) e para outros usuários na organização do usuário conectado. Essas solicitações requerem a permissão People.Read, com exceção da pesquisa de pessoas relevantes de outros usuários, que exige People.Read.All. Por padrão, cada resposta retorna 10 registros, mas você pode alterar isso usando o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="83043-p118">The requests in this section allow you to search for people relevant to the signed-in user (`/me`) and other users in the signed-in user’s organization. These requests require the People.Read permission, with the exception of searching other users’ relevant people, which requires People.Read.All. By default, each response returns 10 records, but you can change this by using the *$top* parameter.</span></span>

### <a name="use-search-to-select-people"></a><span data-ttu-id="83043-182">Usar a pesquisa para selecionar pessoas</span><span class="sxs-lookup"><span data-stu-id="83043-182">Use search to select people</span></span>

<span data-ttu-id="83043-183">Use o parâmetro *$search* para selecionar as pessoas que atendem a determinado conjunto de critérios.</span><span class="sxs-lookup"><span data-stu-id="83043-183">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="83043-184">A consulta de pesquisa a seguir retorna pessoas relevantes para `/me` cujo **displayName** ou \*emailAddress" tem uma palavra que começa com a letra "j".</span><span class="sxs-lookup"><span data-stu-id="83043-184">The following search query returns people relevant to `/me` whose **displayName** or \*emailAddress" has a word that begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search=j
```

<span data-ttu-id="83043-p119">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="83043-p119">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "E3C5B235-DE15-4566-B7B1-7A8E32426540",
      "displayName": "Jan Travis",
      "givenName": "Jan",
      "surname": "Travis",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "VP Sales",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "19/3123",
      "profession": "",
      "userPrincipalName": "JanT@contoso.onmicrosoft.com",
      "imAddress": "sip:JanT@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "JanT@contoso.onmicrosoft.com",
          "relevanceScore": -12.297347783416837
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 732 555 0102"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "C43BF05E-5B6B-4DCF-B2FC-0837B09E0FA9",
      "displayName": "Jacob Cazares (TAILSPIN)",
      "givenName": null,
      "surname": null,
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": null,
      "companyName": null,
      "yomiCompany": "",
      "department": null,
      "officeLocation": null,
      "profession": "",
      "userPrincipalName": "",
      "imAddress": null,
      "scoredEmailAddresses": [
        {
          "address": "JacobC@tailspintoys.com",
          "relevanceScore": -12.298154282019846
        }
      ],
      "phones": [],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "PersonalContact"
      }
    },
    {
      "id": "6BB9CC1F-418D-4DDF-AB0C-6A1C4ABCDBF4",
      "displayName": "Jewell Montgomery",
      "givenName": "Jewell",
      "surname": "Montgomery",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": null,
      "companyName": null,
      "yomiCompany": "",
      "department": null,
      "officeLocation": null,
      "profession": "",
      "userPrincipalName": "JewellM@contoso.onmicrosoft.com",
      "imAddress": null,
      "scoredEmailAddresses": [
        {
          "address": "JewellM@contoso.onmicrosoft.com",
          "relevanceScore": -12.531408487977451
        }
      ],
      "phones": [],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="perform-a-fuzzy-search"></a><span data-ttu-id="83043-189">Realizar uma pesquisa difusa</span><span class="sxs-lookup"><span data-stu-id="83043-189">Perform a fuzzy search</span></span>

<span data-ttu-id="83043-190">As pesquisas implementam um algoritmo de correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="83043-190">Searches implement a fuzzy matching algorithm.</span></span> <span data-ttu-id="83043-191">Retornarão resultados com base em uma correspondência exata e também em Inferências sobre a intenção da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="83043-191">They will return results based on an exact match and also on inferences about the intent of the search.</span></span> <span data-ttu-id="83043-192">Por exemplo, imagine que um usuário com o nome de exibição "Carlos Lima" e o endereço de email carloslim@example.com que esteja no conjunto **pessoas** do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="83043-192">For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="83043-193">Todas as pesquisas a seguir retornarão esse usuário Carlos como um dos resultados.</span><span class="sxs-lookup"><span data-stu-id="83043-193">All of the following searches will return this user Tyler as one of the results.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler"                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle"              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search="tiler"                //fuzzy match with Tyler's name
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"            //matches Tyler's name. Note the quotes to enclose the space.
```
