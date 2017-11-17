# <a name="list-people"></a><span data-ttu-id="d704c-101">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="d704c-101">List people</span></span>

<span data-ttu-id="d704c-102">Recupere uma coleção de objetos [person](../resources/person.md) ordenados por relevância para o [usuário](../resources/user.md), o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="d704c-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="d704c-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="d704c-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d704c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d704c-105">Permissions</span></span>
<span data-ttu-id="d704c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d704c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="d704c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d704c-108">Permission type</span></span>      | <span data-ttu-id="d704c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d704c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d704c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d704c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d704c-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="d704c-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="d704c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d704c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d704c-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="d704c-113">People.Read</span></span>    |
|<span data-ttu-id="d704c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d704c-114">Application</span></span> | <span data-ttu-id="d704c-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="d704c-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d704c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d704c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d704c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d704c-117">Optional query parameters</span></span>
|<span data-ttu-id="d704c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d704c-118">Name</span></span>|<span data-ttu-id="d704c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="d704c-119">Value</span></span>|<span data-ttu-id="d704c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d704c-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="d704c-121">$filter</span><span class="sxs-lookup"><span data-stu-id="d704c-121">$filter</span></span>|<span data-ttu-id="d704c-122">string</span><span class="sxs-lookup"><span data-stu-id="d704c-122">string</span></span>|<span data-ttu-id="d704c-123">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="d704c-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="d704c-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="d704c-124">$orderby</span></span>|<span data-ttu-id="d704c-125">string</span><span class="sxs-lookup"><span data-stu-id="d704c-125">string</span></span>|<span data-ttu-id="d704c-p103">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta ao usar o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="d704c-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="d704c-128">$search</span><span class="sxs-lookup"><span data-stu-id="d704c-128">$search</span></span>|<span data-ttu-id="d704c-129">string</span><span class="sxs-lookup"><span data-stu-id="d704c-129">string</span></span>|<span data-ttu-id="d704c-p104">Pesquisar pessoas por nome ou alias. Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="d704c-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="d704c-132">$select</span><span class="sxs-lookup"><span data-stu-id="d704c-132">$select</span></span>|<span data-ttu-id="d704c-133">string</span><span class="sxs-lookup"><span data-stu-id="d704c-133">string</span></span>|<span data-ttu-id="d704c-p105">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="d704c-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="d704c-136">$skip</span><span class="sxs-lookup"><span data-stu-id="d704c-136">$skip</span></span>|<span data-ttu-id="d704c-137">int</span><span class="sxs-lookup"><span data-stu-id="d704c-137">int</span></span>|<span data-ttu-id="d704c-p106">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="d704c-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="d704c-140">$top</span><span class="sxs-lookup"><span data-stu-id="d704c-140">$top</span></span>|<span data-ttu-id="d704c-141">int</span><span class="sxs-lookup"><span data-stu-id="d704c-141">int</span></span>|<span data-ttu-id="d704c-142">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="d704c-142">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d704c-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d704c-143">Request headers</span></span>
| <span data-ttu-id="d704c-144">Nome</span><span class="sxs-lookup"><span data-stu-id="d704c-144">Name</span></span>      |<span data-ttu-id="d704c-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="d704c-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d704c-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="d704c-146">Authorization</span></span>  | <span data-ttu-id="d704c-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d704c-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d704c-149">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d704c-149">Accept</span></span> | <span data-ttu-id="d704c-150">application/json</span><span class="sxs-lookup"><span data-stu-id="d704c-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d704c-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d704c-151">Request body</span></span>
<span data-ttu-id="d704c-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d704c-152">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d704c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d704c-153">Response</span></span>
<span data-ttu-id="d704c-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [person](../resources/person.md) no corpo da resposta. A resposta pode conter um objeto person ou uma coleção de objetos person.</span><span class="sxs-lookup"><span data-stu-id="d704c-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span> 
## <a name="examples"></a><span data-ttu-id="d704c-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d704c-156">Examples</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="d704c-157">Obter uma coleção de pessoas relevantes</span><span class="sxs-lookup"><span data-stu-id="d704c-157">Get a collection of relevant people</span></span> 

<span data-ttu-id="d704c-158">A solicitação a seguir obtém as pessoas mais relevantes para o usuário conectado (`/me`), com base nos padrões de comunicação e colaboração e nas relações comerciais.</span><span class="sxs-lookup"><span data-stu-id="d704c-158">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="d704c-p109">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro de consulta *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="d704c-p109">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_person_collection",
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
                    "relevanceScore": 8.0
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
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
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
                    "relevanceScore": 8.0
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
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
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
                    "relevanceScore": 8.0
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
### <a name="search-other-users-relevant-people"></a><span data-ttu-id="d704c-163">Pesquisar pessoas relevantes de outro usuário</span><span class="sxs-lookup"><span data-stu-id="d704c-163">Search other user’s relevant people</span></span>

<span data-ttu-id="d704c-p110">A solicitação a seguir obtém as pessoas mais relevantes para outra pessoa na organização do usuário conectado. Esta solicitação requer a permissão People.Read.All. Neste exemplo, as pessoas relevantes de Roscoe Seidel são exibidas.</span><span class="sxs-lookup"><span data-stu-id="d704c-p110">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_other_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="d704c-p111">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso ao usar o parâmetro *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="d704c-p111">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_other_person",
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
                    "relevanceScore": 20.0
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
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
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
                    "relevanceScore": 10.0
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
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
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
                    "relevanceScore": 10.0
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
