# <a name="list-people"></a><span data-ttu-id="362f6-101">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="362f6-101">List people</span></span>

<span data-ttu-id="362f6-102">Recupere uma coleção de objetos [person](../resources/person.md) ordenados por relevância para o [usuário](../resources/user.md), o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="362f6-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="362f6-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="362f6-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="362f6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="362f6-105">Permissions</span></span>

<span data-ttu-id="362f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="362f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="362f6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="362f6-108">Permission type</span></span>      | <span data-ttu-id="362f6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="362f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="362f6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="362f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="362f6-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="362f6-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="362f6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="362f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="362f6-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="362f6-113">People.Read</span></span>    |
|<span data-ttu-id="362f6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="362f6-114">Application</span></span> | <span data-ttu-id="362f6-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="362f6-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="362f6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="362f6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="362f6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="362f6-117">Optional query parameters</span></span>

<span data-ttu-id="362f6-118">Este método oferece suporte aos [ parâmetros de consulta OData ](../../../concepts/query_parameters.md) para personalizar a resposta, como mostrado nos exemplos no artigo [Obter informações relevantes sobre pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="362f6-118">This method supports the [OData query parameters](../../../concepts/query_parameters.md) to help customize the response, as shown in the examples in the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

|<span data-ttu-id="362f6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="362f6-119">Name</span></span>|<span data-ttu-id="362f6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="362f6-120">Value</span></span>|<span data-ttu-id="362f6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="362f6-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="362f6-122">$filter</span><span class="sxs-lookup"><span data-stu-id="362f6-122">$filter</span></span>|<span data-ttu-id="362f6-123">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="362f6-123">string</span></span>|<span data-ttu-id="362f6-124">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="362f6-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="362f6-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="362f6-125">$orderby</span></span>|<span data-ttu-id="362f6-126">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="362f6-126">string</span></span>|<span data-ttu-id="362f6-127">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="362f6-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="362f6-128">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="362f6-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="362f6-129">$search</span><span class="sxs-lookup"><span data-stu-id="362f6-129">$search</span></span>|<span data-ttu-id="362f6-130">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="362f6-130">string</span></span>|<span data-ttu-id="362f6-131">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="362f6-131">Search for people by name or alias.</span></span> <span data-ttu-id="362f6-132">Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="362f6-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="362f6-133">O parâmetro funciona apenas para pesquisar pessoas relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários.</span><span class="sxs-lookup"><span data-stu-id="362f6-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="362f6-134">Também oferece suporte à palavra-chave `topic` para localizar pessoas com base em tópicos extraídos de conversas de e-mail com essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="362f6-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="362f6-135">Consulte a seção *Executar uma pesquisa difusa* em [Obter informações relevantes sobre pessoas](../../../concepts/people_example.md#perform-a-fuzzy-search) para mais informações e exemplos.</span><span class="sxs-lookup"><span data-stu-id="362f6-135">See the *Perform a fuzzy search* section at [Get relevant information about people](../../../concepts/people_example.md#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="362f6-136">$select</span><span class="sxs-lookup"><span data-stu-id="362f6-136">$select</span></span>|<span data-ttu-id="362f6-137">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="362f6-137">string</span></span>|<span data-ttu-id="362f6-p105">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="362f6-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="362f6-140">$skip</span><span class="sxs-lookup"><span data-stu-id="362f6-140">$skip</span></span>|<span data-ttu-id="362f6-141">int</span><span class="sxs-lookup"><span data-stu-id="362f6-141">int</span></span>|<span data-ttu-id="362f6-p106">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="362f6-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="362f6-144">$top</span><span class="sxs-lookup"><span data-stu-id="362f6-144">$top</span></span>|<span data-ttu-id="362f6-145">int</span><span class="sxs-lookup"><span data-stu-id="362f6-145">int</span></span>|<span data-ttu-id="362f6-146">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="362f6-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="362f6-147">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="362f6-147">Request headers</span></span>

| <span data-ttu-id="362f6-148">Nome</span><span class="sxs-lookup"><span data-stu-id="362f6-148">Name</span></span>      |<span data-ttu-id="362f6-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="362f6-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="362f6-150">Autorização</span><span class="sxs-lookup"><span data-stu-id="362f6-150">Authorization</span></span>  | <span data-ttu-id="362f6-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="362f6-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="362f6-153">Aceitar</span><span class="sxs-lookup"><span data-stu-id="362f6-153">Accept</span></span> | <span data-ttu-id="362f6-154">application/json</span><span class="sxs-lookup"><span data-stu-id="362f6-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="362f6-155">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="362f6-155">Request body</span></span>

<span data-ttu-id="362f6-156">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="362f6-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="362f6-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="362f6-157">Response</span></span>

<span data-ttu-id="362f6-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [person](../resources/person.md) no corpo da resposta. A resposta pode conter um objeto person ou uma coleção de objetos person.</span><span class="sxs-lookup"><span data-stu-id="362f6-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="362f6-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="362f6-160">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="362f6-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="362f6-161">Request</span></span>

<span data-ttu-id="362f6-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="362f6-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="362f6-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="362f6-163">Response</span></span>

<span data-ttu-id="362f6-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="362f6-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="362f6-165">Para ver mais exemplos, confira o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="362f6-165">For more examples, see the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
