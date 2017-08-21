# <a name="list-people"></a><span data-ttu-id="c4cf8-101">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="c4cf8-101">List people</span></span>

<span data-ttu-id="c4cf8-102">Recupere uma coleção de objetos [person](../resources/person.md) ordenados por relevância para o [usuário](../resources/user.md), o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="c4cf8-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4cf8-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4cf8-105">Prerequisites</span></span>
<span data-ttu-id="c4cf8-106">Os seguintes **escopos** são necessários para executar esta API: *People.Read* *People.Read.All*</span><span class="sxs-lookup"><span data-stu-id="c4cf8-106">The following **scopes** are required to execute this API: *People.Read* *People.Read.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="c4cf8-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4cf8-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4cf8-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4cf8-108">Optional query parameters</span></span>
|<span data-ttu-id="c4cf8-109">Nome</span><span class="sxs-lookup"><span data-stu-id="c4cf8-109">Name</span></span>|<span data-ttu-id="c4cf8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c4cf8-110">Value</span></span>|<span data-ttu-id="c4cf8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4cf8-111">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="c4cf8-112">$filter</span><span class="sxs-lookup"><span data-stu-id="c4cf8-112">$filter</span></span>|<span data-ttu-id="c4cf8-113">string</span><span class="sxs-lookup"><span data-stu-id="c4cf8-113">string</span></span>|<span data-ttu-id="c4cf8-114">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-114">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="c4cf8-115">$orderby</span><span class="sxs-lookup"><span data-stu-id="c4cf8-115">$orderby</span></span>|<span data-ttu-id="c4cf8-116">string</span><span class="sxs-lookup"><span data-stu-id="c4cf8-116">string</span></span>|<span data-ttu-id="c4cf8-p102">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta ao usar o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p102">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="c4cf8-119">$search</span><span class="sxs-lookup"><span data-stu-id="c4cf8-119">$search</span></span>|<span data-ttu-id="c4cf8-120">string</span><span class="sxs-lookup"><span data-stu-id="c4cf8-120">string</span></span>|<span data-ttu-id="c4cf8-p103">Pesquisar pessoas por nome ou alias. Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p103">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="c4cf8-123">$select</span><span class="sxs-lookup"><span data-stu-id="c4cf8-123">$select</span></span>|<span data-ttu-id="c4cf8-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4cf8-124">string</span></span>|<span data-ttu-id="c4cf8-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="c4cf8-127">$skip</span><span class="sxs-lookup"><span data-stu-id="c4cf8-127">$skip</span></span>|<span data-ttu-id="c4cf8-128">int</span><span class="sxs-lookup"><span data-stu-id="c4cf8-128">int</span></span>|<span data-ttu-id="c4cf8-p105">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="c4cf8-131">$top</span><span class="sxs-lookup"><span data-stu-id="c4cf8-131">$top</span></span>|<span data-ttu-id="c4cf8-132">int</span><span class="sxs-lookup"><span data-stu-id="c4cf8-132">int</span></span>|<span data-ttu-id="c4cf8-133">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-133">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c4cf8-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4cf8-134">Request headers</span></span>
| <span data-ttu-id="c4cf8-135">Nome</span><span class="sxs-lookup"><span data-stu-id="c4cf8-135">Name</span></span>      |<span data-ttu-id="c4cf8-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4cf8-136">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4cf8-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4cf8-137">Authorization</span></span>  | <span data-ttu-id="c4cf8-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4cf8-140">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4cf8-140">Accept</span></span> | <span data-ttu-id="c4cf8-141">application/json</span><span class="sxs-lookup"><span data-stu-id="c4cf8-141">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4cf8-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4cf8-142">Request body</span></span>
<span data-ttu-id="c4cf8-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-143">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c4cf8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4cf8-144">Response</span></span>
<span data-ttu-id="c4cf8-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [person](../resources/person.md) no corpo da resposta. A resposta pode conter um objeto person ou uma coleção de objetos person.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p107">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span> 
## <a name="examples"></a><span data-ttu-id="c4cf8-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4cf8-147">Examples</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="c4cf8-148">Obter uma coleção de pessoas relevantes</span><span class="sxs-lookup"><span data-stu-id="c4cf8-148">Get a collection of relevant people</span></span> 

<span data-ttu-id="c4cf8-149">A solicitação a seguir obtém as pessoas mais relevantes para o usuário conectado (`/me`), com base nos padrões de comunicação e colaboração e nas relações comerciais.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-149">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="c4cf8-p108">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro de consulta *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p108">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

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
### <a name="search-other-users-relevant-people"></a><span data-ttu-id="c4cf8-154">Pesquisar pessoas relevantes de outro usuário</span><span class="sxs-lookup"><span data-stu-id="c4cf8-154">Search other user’s relevant people</span></span>

<span data-ttu-id="c4cf8-p109">A solicitação a seguir obtém as pessoas mais relevantes para outra pessoa na organização do usuário conectado. Esta solicitação requer a permissão People.Read.All. Neste exemplo, as pessoas relevantes de Roscoe Seidel são exibidas.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p109">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="c4cf8-p110">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso ao usar o parâmetro *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-p110">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
