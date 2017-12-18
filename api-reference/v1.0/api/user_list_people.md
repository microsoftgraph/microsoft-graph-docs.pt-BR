# <a name="list-people"></a><span data-ttu-id="23b79-101">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="23b79-101">List people</span></span>

<span data-ttu-id="23b79-102">Recupere uma coleção de objetos [person](../resources/person.md) ordenados por relevância para o [usuário](../resources/user.md), o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="23b79-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="23b79-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="23b79-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="23b79-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="23b79-105">Permissions</span></span>
<span data-ttu-id="23b79-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="23b79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23b79-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23b79-108">Permission type</span></span>      | <span data-ttu-id="23b79-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23b79-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23b79-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23b79-110">Delegated (work or school account)</span></span> | <span data-ttu-id="23b79-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="23b79-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="23b79-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23b79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23b79-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="23b79-113">People.Read</span></span>    |
|<span data-ttu-id="23b79-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23b79-114">Application</span></span> | <span data-ttu-id="23b79-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="23b79-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23b79-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23b79-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23b79-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23b79-117">Optional query parameters</span></span>
<span data-ttu-id="23b79-118">Este método dá suporte a [Parâmetros de consulta OData](../../../concepts/people_example.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23b79-118">This method supports the [OData Query Parameters](../../../concepts/people_example.md) to help customize the response.</span></span>

|<span data-ttu-id="23b79-119">Nome</span><span class="sxs-lookup"><span data-stu-id="23b79-119">Name</span></span>|<span data-ttu-id="23b79-120">Valor</span><span class="sxs-lookup"><span data-stu-id="23b79-120">Value</span></span>|<span data-ttu-id="23b79-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="23b79-121">Description</span></span>| 
|:---------------|:--------|:-------| 
|<span data-ttu-id="23b79-122">$filter</span><span class="sxs-lookup"><span data-stu-id="23b79-122">$filter</span></span>|<span data-ttu-id="23b79-123">string</span><span class="sxs-lookup"><span data-stu-id="23b79-123">string</span></span>|<span data-ttu-id="23b79-124">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="23b79-124">Limits the response to only those people whose record contains the specified criteria.</span></span>| 
|<span data-ttu-id="23b79-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="23b79-125">$orderby</span></span>|<span data-ttu-id="23b79-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23b79-126">string</span></span>|<span data-ttu-id="23b79-127">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="23b79-127">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the $orderby parameter.</span></span> <span data-ttu-id="23b79-128">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="23b79-128">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>| 
|<span data-ttu-id="23b79-129">$search</span><span class="sxs-lookup"><span data-stu-id="23b79-129">$search</span></span>|<span data-ttu-id="23b79-130">string</span><span class="sxs-lookup"><span data-stu-id="23b79-130">string</span></span>|<span data-ttu-id="23b79-131">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="23b79-131">Search for people by name or alias. Supports fuzzy matching.</span></span> <span data-ttu-id="23b79-132">Suporta correspondência difusa</span><span class="sxs-lookup"><span data-stu-id="23b79-132">Supports Fuzzy matching</span></span>| 
|<span data-ttu-id="23b79-133">$select</span><span class="sxs-lookup"><span data-stu-id="23b79-133">$select</span></span>|<span data-ttu-id="23b79-134">string</span><span class="sxs-lookup"><span data-stu-id="23b79-134">string</span></span>|<span data-ttu-id="23b79-p105">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="23b79-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>| 
|<span data-ttu-id="23b79-137">$skip</span><span class="sxs-lookup"><span data-stu-id="23b79-137">$skip</span></span>|<span data-ttu-id="23b79-138">int</span><span class="sxs-lookup"><span data-stu-id="23b79-138">int</span></span>|<span data-ttu-id="23b79-p106">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="23b79-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>| 
|<span data-ttu-id="23b79-141">$top</span><span class="sxs-lookup"><span data-stu-id="23b79-141">$top</span></span>|<span data-ttu-id="23b79-142">int</span><span class="sxs-lookup"><span data-stu-id="23b79-142">int</span></span>|<span data-ttu-id="23b79-143">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="23b79-143">Number of results to be returned.</span></span>| 

## <a name="request-headers"></a><span data-ttu-id="23b79-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23b79-144">Request headers</span></span>
| <span data-ttu-id="23b79-145">Nome</span><span class="sxs-lookup"><span data-stu-id="23b79-145">Name</span></span>      |<span data-ttu-id="23b79-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="23b79-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23b79-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="23b79-147">Authorization</span></span>  | <span data-ttu-id="23b79-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23b79-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23b79-150">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23b79-150">Accept</span></span> | <span data-ttu-id="23b79-151">application/json</span><span class="sxs-lookup"><span data-stu-id="23b79-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="23b79-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23b79-152">Request body</span></span>
<span data-ttu-id="23b79-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23b79-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23b79-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="23b79-154">Response</span></span>
<span data-ttu-id="23b79-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [person](../resources/person.md) no corpo da resposta. A resposta pode conter um objeto person ou uma coleção de objetos person.</span><span class="sxs-lookup"><span data-stu-id="23b79-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="23b79-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="23b79-157">Examples</span></span>
#### <a name="request"></a><span data-ttu-id="23b79-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23b79-158">Request</span></span>
<span data-ttu-id="23b79-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23b79-159">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="23b79-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="23b79-160">Response</span></span>
<span data-ttu-id="23b79-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23b79-161">Here is an example of the response.</span></span>

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
Content-length: 1370

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
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
                    "address": "Marketing@contoso.com",
                    "relevanceScore": 30.0
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Group",
                "subclass": "UnifiedGroup"
            }
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "IsaiahL@contoso.com",
            "imAddress": "sip:isaiahl@contoso.com",
            "scoredEmailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "relevanceScore": 20.0
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
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

<span data-ttu-id="23b79-162">Para ver mais exemplos, confira o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="23b79-162">For more examples, see the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
