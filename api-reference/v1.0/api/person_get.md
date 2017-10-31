# <a name="get-person"></a>Obter pessoa

Recupere as propriedades e os relacionamentos de um objeto [person](../resources/person.md).

Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).
 

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | People.Read, People.Read.All    |
|Delegado (conta pessoal da Microsoft) | People.Read    |
|Aplicativo | People.Read.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
|Nome|Valor|Descrição|
|:---------------|:--------|:-------|
|$filter|string|Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.|
|$orderby|string|Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.|
|$search|string|Pesquisar pessoas por nome ou alias. Suporta correspondência difusa.|
|$select|string|Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.|
|$skip|int|Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.|
|$top|int|Número de resultados a ser retornado.|

## <a name="parameters"></a>Parâmetros
| Parâmetro	 |Tipo       |Descrição|
|:----------|:----------|:----------|
|property_value|String     |O valor da propriedade estendida a ser correspondida. Obrigatório onde listado na seção **Solicitação HTTP**.|
|person_property|String    |A propriedade person para fazer a correspondência. Obrigatório onde listado na seção **Solicitação HTTP**.|

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [person](../resources/person.md) no corpo da resposta. A resposta pode conter uma instância person ou uma coleção de instâncias person. 
## <a name="examples"></a>Exemplos
### <a name="perform-a-search"></a>Realizar uma pesquisa 
A solicitação a seguir faz uma pesquisa por uma pessoa denominada Clara Barbosa. 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

O exemplo a seguir mostra a resposta. 

<!-- {
  "blockType": "response",
  "name": "get_person",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": [
               {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
       }
   ]
}
```
### <a name="select-the-fields-to-return-in-a-filtered-response"></a>Selecionar os campos a serem retornados em uma resposta filtrada 
Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo. 

O exemplo a seguir obtém **displayName** e **scoredEmailAddresses** das pessoas cujo nome de exibição corresponde ao nome especificado. Neste exemplo, somente as pessoas cujo nome para exibição corresponde a "Lorrie Frye" são retornadas.

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

O seguinte é a URL corretamente codificada para o pedido de exemplo.

<!-- {
  "blockType": "request",
  "name": "get_person_select_and_filter"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName%20eq%20'Lorrie Frye'
```

O exemplo a seguir mostra a resposta. 

<!-- {
  "blockType": "response",
  "name": "get_person_select_and_filter",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

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
                    "relevanceScore": 8.0
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get person",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
