# <a name="use-the-people-api-in-microsoft-graph-to-get-information-about-the-people-most-relevant-to-you"></a>Usar a API de Pessoas no Microsoft Graph para obter informações sobre as pessoas mais relevantes para você
Os aplicativos do Microsoft Graph podem usar a API de Pessoas para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório de uma organização e as pessoas de comunicações recentes (como emails e Skype). Além de gerar essas informações, a API de Pessoas também fornece suporte para pesquisa de correspondência difusa e a capacidade de recuperar a lista de usuários relevantes para outro usuário na organização do usuário conectado. A API de Pessoas é particularmente útil para cenários de seleção de pessoas, como ao redigir um email ou criar uma reunião. Por exemplo, você pode usar a API de Pessoas em cenários de redação de emails.
 
## <a name="authorization"></a>Autorização
Para chamar a API de Pessoas no Microsoft Graph, seu aplicativo precisará das permissões adequadas: 

* People.Read - use para fazer chamadas gerais da API de Pessoas; por exemplo, https://graph.microsoft.com/v1.0/me/people/. People.Read requer o consentimento do usuário final.
* People.Read.All - necessária para recuperar as pessoas mais relevantes para um usuário especificado nas chamadas da organização do usuário conectado (https://graph.microsoft.com/v1.0/users('{id}')/people). People.Read.All requer o consentimento do administrador.
## <a name="browse-people"></a>Procurar pessoas
As solicitações nesta seção obtém as pessoas mais relevantes para o usuário conectado (`/me`). Essas solicitações requerem a permissão People.Read. Por padrão, cada resposta retorna 10 registros, mas você pode alterar isso usando o parâmetro de consulta *$top*. 
### <a name="get-a-collection-of-relevant-people"></a>Obter uma coleção de pessoas relevantes 
A solicitação a seguir obtém as pessoas mais relevantes para o usuário conectado (`/me`), com base nos padrões de comunicação e colaboração e nas relações comerciais. 

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro de consulta *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.

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
            "userPrincipalName": "Lorrief@contoso.onmicrosoft.com",
            "imAddress": "sip:Lorrief@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Maynardd@contoso.onmicrosoft.com",
            "imAddress": "sip:Maynardd@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Darrelh@contoso.onmicrosoft.com",
            "imAddress": "sip:Darrelh@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
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
### <a name="request-a-subsequent-page-of-people"></a>Solicitar uma página subsequente de pessoas
Se a primeira resposta não contiver a lista completa das pessoas relevantes, você poderá fazer uma segunda solicitação usando *$top* e *$skip* para solicitar páginas adicionais de informações. Se a solicitação anterior tiver informações adicionais, a solicitação a seguir obterá a próxima página de pessoas do servidor.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=3&$skip=10
```

O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro de consulta *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.

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
            "userPrincipalName": "Felixc@contoso.onmicrosoft.com",
            "imAddress": "sip:Felixc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Felixc@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Lenorar@contoso.onmicrosoft.com",
            "imAddress": "sip:Lenorar@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lenorar@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Manuelc@contoso.onmicrosoft.com",
            "imAddress": "sip:Manuelc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Manuelc@contoso.onmicrosoft.com",
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
### <a name="sort-the-response"></a>Classificar a resposta 
Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta ao usar o parâmetro *$orderby*. Essa consulta seleciona as pessoas mais relevantes para você, classifica-as por **displayName** e, em seguida, retorna as primeiras 10 pessoas na lista classificada.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$orderby=displayName
```

O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso ao usar o parâmetro *$top*. O exemplo a seguir usa *$top* para limitar a resposta a três registros.

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
            "userPrincipalName": "Adrianar@contoso.onmicrosoft.com",
            "imAddress": "sip:Adrianar@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Adrianar@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Alycec@contoso.onmicrosoft.com",
            "imAddress": "sip:Alycec@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Alycec@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Alyssac@contoso.onmicrosoft.com",
            "imAddress": "sip:Alyssac@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Alyssac@contoso.onmicrosoft.com",
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
### <a name="change-the-number-of-people-and-fields-returned"></a>Alterar o número de pessoas e campos retornados 
Você pode alterar o número de pessoas retornadas na resposta definindo o parâmetro *$top*. 

O exemplo a seguir solicita as 1.000 pessoas mais relevantes para `/me`. A solicitação também limita a quantidade de dados enviados de volta do servidor solicitando somente o **displayName** da pessoa.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=1000&$Select=displayName
```

O exemplo a seguir mostra a resposta. 

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
        },
      ... etc
}
```
### <a name="select-the-fields-to-return"></a>Selecione os campos para retornar
Você pode limitar a quantidade de dados retornados do servidor usando o parâmetro *$select* para escolher um ou mais campos. O campo `@odata.id` sempre é retornado.

O exemplo a seguir limita a resposta ao **displayName** e **scoredEmailAddresses** das 10 pessoas mais relevantes.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses
```

O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.

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
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        }
    ]
}
```
### <a name="use-a-filter-to-limit-the-response"></a>Usar um filtro para limitar a resposta 
Você pode usar o parâmetro *$filter* para limitar a resposta apenas às pessoas cujo registro contém os critérios especificados. 

A consulta a seguir limita a resposta a instâncias **person** com a propriedade **personType** com as atribuições de **person** como **classe** e **organizationUser** como **subclasse**.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$filter=personType/class eq 'Person' and personType/subclass eq 'OrganizationUser'
```

O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.

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
            "userPrincipalName": "Lorrief@contoso.onmicrosoft.com",
            "imAddress": "sip:Lorrief@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Maynardd@contoso.onmicrosoft.com",
            "imAddress": "sip:Maynardd@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Darrelh@contoso.onmicrosoft.com",
            "imAddress": "sip:Darrelh@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a>Selecionar os campos a serem retornados em uma resposta filtrada 
Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo. 

O exemplo a seguir obtém **displayName** e **scoredEmailAddresses** das pessoas cujo nome de exibição corresponde ao nome especificado. Neste exemplo, somente as pessoas cujo nome para exibição corresponde a "Lorrie Frye" são retornadas. 

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

O exemplo a seguir mostra a resposta. 

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
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        }
    ]
}
```
## <a name="search-people"></a>Pesquisar pessoas
As solicitações nesta seção permitem procurar pessoas relevantes para o usuário conectado (`/me`) e para outros usuários na organização do usuário conectado. Essas solicitações requerem a permissão People.Read, com exceção da pesquisa de pessoas relevantes de outros usuários, que exige People.Read.All. Por padrão, cada resposta retorna 10 registros, mas você pode alterar isso usando o parâmetro *$top*. 
### <a name="use-search-to-select-people"></a>Usar a pesquisa para selecionar pessoas 
Use o parâmetro *$search* para selecionar as pessoas que atendem a determinado conjunto de critérios. 

A consulta de pesquisa a seguir retorna pessoas relevantes para `/me` cujo **displayName** ou *emailAddress" tem uma palavra que começa com a letra "j".

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search=j
```

O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.

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
            "userPrincipalName": "jant@contoso.onmicrosoft.com",
            "imAddress": "sip:jant@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "jant@contoso.onmicrosoft.com",
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
                    "address": "jacobc@tailspintoys.com",
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
            "userPrincipalName": "jewellm@contoso.onmicrosoft.com",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "jewellm@contoso.onmicrosoft.com",
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
### <a name="perform-a-fuzzy-search"></a>Realizar uma pesquisa difusa 

As pesquisas implementam um algoritmo de correspondência difusa. Retornarão resultados com base em uma correspondência exata e também em Inferências sobre a intenção da pesquisa. Por exemplo, imagine que um usuário com o nome de exibição "Carlos Lima" e o endereço de email carloslim@example.com que esteja no conjunto **pessoas** do usuário conectado. Todas as pesquisas a seguir retornarão esse usuário Carlos como um dos resultados.

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

Também é possível executar pesquisas para pessoas relevantes para o usuário conectado e que tenham manifestado interesse em se comunicar com esse usuário sobre tópicos como pizzas no exemplo a seguir:

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

Os tópicos neste contexto são apenas palavras que os usuários usaram com mais frequência nas conversas de email. A Microsoft extrai essas palavras e cria um índice para esses dados para facilitar pesquisas difusas. 

A frase de pesquisa está entre aspas, e os tópicos nesses dados são extraídos dos contextos. Por exemplo, ao pesquisar por "windows" na seguinte consulta:

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:windows" 
```
temos uma busca difusa no índice de dados do tópico, e os resultados podem incluir instâncias que significam o sistema operacional Windows, uma abertura em uma parede ou outras definições.

Finalmente, é possível combinar pesquisas de pessoas e pesquisas de tópicos na mesma solicitação combinando os dois tipos de expressão de pesquisa.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```

Essa solicitação realiza basicamente duas pesquisas: uma pesquisa difusa em relação às propriedades **displayName** e **emailAddress** de pessoas relevantes ao usuário conectado e uma pesquisa pontual por "pizza" em relação às pessoas relevantes ao usuário. Os resultados são classificados, ordenados e retornados. A pesquisa não é restritiva. Você pode obter resultados que contenham pessoas com correspondência difusa "car", que estejam interessadas em "pizza" ou ambos.

### <a name="search-other-users-relevant-people"></a>Pesquisar pessoas relevantes de outro usuário
A solicitação a seguir obtém as pessoas mais relevantes para outra pessoa na organização do usuário conectado. Esta solicitação requer a permissão People.Read.All. Neste exemplo, as pessoas relevantes de Roscoe Seidel são exibidas.

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro *$top*. O exemplo abaixo usa *$top* para limitar a resposta a três registros.

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
            "userPrincipalName": "Cliftonc@contoso.onmicrosoft.com",
            "imAddress": "sip:Cliftonc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Cliftonc@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Shereem@contoso.onmicrosoft.com",
            "imAddress": "sip:shereem@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Shereem@contoso.onmicrosoft.com",
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
            "userPrincipalName": "Vincentm@contoso.onmicrosoft.com",
            "imAddress": "sip:vincentm@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Vincentm@contoso.onmicrosoft.com",
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