---
title: Listar pessoas
description: Recupere uma lista de objetos Person ordenados por sua relevância para o usuário, que é determinado pelos padrões de comunicação e colaboração do usuário e relações comerciais.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: de07eaa4b3601c91ace9894e55bd4357fbb23881
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637189"
---
# <a name="list-people"></a><span data-ttu-id="b9fd8-103">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="b9fd8-103">List people</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9fd8-104">Recupere uma lista de objetos [Person](../resources/person.md) ordenados por sua relevância para o [usuário](../resources/user.md), que é determinado pelos padrões de comunicação e colaboração do usuário e relações comerciais.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-104">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9fd8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9fd8-105">Permissions</span></span>

<span data-ttu-id="b9fd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9fd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9fd8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9fd8-108">Permission type</span></span>      | <span data-ttu-id="b9fd8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9fd8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9fd8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9fd8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9fd8-111">People.Read</span><span class="sxs-lookup"><span data-stu-id="b9fd8-111">People.Read</span></span>    |
|<span data-ttu-id="b9fd8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9fd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9fd8-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="b9fd8-113">People.Read</span></span>    |
|<span data-ttu-id="b9fd8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9fd8-114">Application</span></span> | <span data-ttu-id="b9fd8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9fd8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9fd8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9fd8-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9fd8-117">Optional query parameters</span></span>

<span data-ttu-id="b9fd8-118">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-118">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="b9fd8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b9fd8-119">Name</span></span>|<span data-ttu-id="b9fd8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b9fd8-120">Value</span></span>|<span data-ttu-id="b9fd8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9fd8-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="b9fd8-122">$filter</span><span class="sxs-lookup"><span data-stu-id="b9fd8-122">$filter</span></span>|<span data-ttu-id="b9fd8-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9fd8-123">string</span></span>|<span data-ttu-id="b9fd8-124">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="b9fd8-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="b9fd8-125">$orderby</span></span>|<span data-ttu-id="b9fd8-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9fd8-126">string</span></span>|<span data-ttu-id="b9fd8-127">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="b9fd8-128">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="b9fd8-129">$search</span><span class="sxs-lookup"><span data-stu-id="b9fd8-129">$search</span></span>|<span data-ttu-id="b9fd8-130">string</span><span class="sxs-lookup"><span data-stu-id="b9fd8-130">string</span></span>|<span data-ttu-id="b9fd8-131">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-131">Search for people by name or alias.</span></span> <span data-ttu-id="b9fd8-132">Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="b9fd8-133">O parâmetro só funciona para pesquisar pessoas relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="b9fd8-134">Também dá suporte a `topic` palavra-chave para encontrar pessoas com base em tópicos extraídos a partir de conversas de email com essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="b9fd8-135">Confira a seção \*Realizar uma pesquisa difusa \* em [Obter informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para informações e exemplos.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-135">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="b9fd8-136">$select</span><span class="sxs-lookup"><span data-stu-id="b9fd8-136">$select</span></span>|<span data-ttu-id="b9fd8-137">string</span><span class="sxs-lookup"><span data-stu-id="b9fd8-137">string</span></span>|<span data-ttu-id="b9fd8-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="b9fd8-140">$skip</span><span class="sxs-lookup"><span data-stu-id="b9fd8-140">$skip</span></span>|<span data-ttu-id="b9fd8-141">int</span><span class="sxs-lookup"><span data-stu-id="b9fd8-141">int</span></span>|<span data-ttu-id="b9fd8-p105">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="b9fd8-144">$top</span><span class="sxs-lookup"><span data-stu-id="b9fd8-144">$top</span></span>|<span data-ttu-id="b9fd8-145">int</span><span class="sxs-lookup"><span data-stu-id="b9fd8-145">int</span></span>|<span data-ttu-id="b9fd8-146">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b9fd8-147">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9fd8-147">Request headers</span></span>

| <span data-ttu-id="b9fd8-148">Nome</span><span class="sxs-lookup"><span data-stu-id="b9fd8-148">Name</span></span>      |<span data-ttu-id="b9fd8-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9fd8-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9fd8-150">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9fd8-150">Authorization</span></span>  | <span data-ttu-id="b9fd8-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9fd8-153">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9fd8-153">Accept</span></span> | <span data-ttu-id="b9fd8-154">application/json</span><span class="sxs-lookup"><span data-stu-id="b9fd8-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9fd8-155">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9fd8-155">Request body</span></span>

<span data-ttu-id="b9fd8-156">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9fd8-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9fd8-157">Response</span></span>

<span data-ttu-id="b9fd8-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Person](../resources/person.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-158">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9fd8-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b9fd8-159">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="b9fd8-160">Browse</span><span class="sxs-lookup"><span data-stu-id="b9fd8-160">Browse</span></span>

<span data-ttu-id="b9fd8-161">As solicitações nesta seção obtêm as pessoas mais relevantes para o usuário conectado (`/me`), com base nas relações de comunicação, colaboração e negócios.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-161">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="b9fd8-162">Por padrão, cada resposta retorna 10 registros, mas você pode alterar esse número usando o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-162">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="b9fd8-163">Essas solicitações exigem a permissão People. Read.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-163">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="b9fd8-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9fd8-164">Request</span></span>

<span data-ttu-id="b9fd8-165">Veja a seguir um exemplo da solicitação padrão.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-165">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="b9fd8-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9fd8-166">Response</span></span>

<span data-ttu-id="b9fd8-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-167">The following is an example of the response.</span></span>
><span data-ttu-id="b9fd8-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

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
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
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
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b9fd8-170">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b9fd8-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b9fd8-171">Basic</span><span class="sxs-lookup"><span data-stu-id="b9fd8-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_person_collection_beta-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9fd8-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9fd8-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_person_collection_beta-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="b9fd8-173">Solicitação de uma página subsequente de pessoas</span><span class="sxs-lookup"><span data-stu-id="b9fd8-173">Requesting a subsequent page of people</span></span>

<span data-ttu-id="b9fd8-p109">Se a primeira resposta não contiver a lista completa das pessoas relevantes, você poderá fazer uma segunda solicitação usando *$top* e *$skip* para solicitar páginas adicionais de informações. Se a solicitação anterior tiver informações adicionais, a solicitação a seguir obterá a próxima página de pessoas do servidor.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-p109">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="b9fd8-176">Classificar a resposta</span><span class="sxs-lookup"><span data-stu-id="b9fd8-176">Sort the response</span></span>

<span data-ttu-id="b9fd8-177">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-177">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="b9fd8-178">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-178">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="b9fd8-179">Essa consulta seleciona as pessoas mais relevantes para você classificando-as pelo nome de exibição e retorna as dez primeiras pessoas da lista classificada.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-179">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="b9fd8-180">Alteração do número de pessoas e dos campos retornados</span><span class="sxs-lookup"><span data-stu-id="b9fd8-180">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="b9fd8-181">Você pode alterar o número de pessoas retornadas na resposta definindo o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-181">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="b9fd8-182">O exemplo a seguir solicita as 1.000 pessoas mais relevantes `/me`.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-182">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="b9fd8-183">A solicitação também limita a quantidade de dados enviados de volta do servidor solicitando apenas o nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-183">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="b9fd8-184">Seleção dos campos que devem ser retornados</span><span class="sxs-lookup"><span data-stu-id="b9fd8-184">Selecting the fields to return</span></span>

<span data-ttu-id="b9fd8-185">Você pode limitar a quantidade de dados retornados do servidor usando o parâmetro *$Select* para escolher um ou mais campos.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-185">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="b9fd8-186">O campo *@odata.id* é sempre retornado.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-186">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="b9fd8-187">O exemplo a seguir limita a resposta para *DisplayName* e *EmailAddress* das dez pessoas mais relevantes.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-187">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="b9fd8-188">Uso de um filtro para limitar a resposta</span><span class="sxs-lookup"><span data-stu-id="b9fd8-188">Using a filter to limit the response</span></span>

<span data-ttu-id="b9fd8-189">Você pode usar o parâmetro *$filter* para limitar a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-189">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="b9fd8-190">A consulta a seguir limita a resposta a pessoas com o "diretório" de origem.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-190">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="b9fd8-191">Selecionar os campos a serem retornados em uma resposta filtrada</span><span class="sxs-lookup"><span data-stu-id="b9fd8-191">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="b9fd8-192">Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-192">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="b9fd8-193">O exemplo a seguir obtém o *DisplayName* e o *EmailAddress* de pessoas cujo nome de exibição é igual ao nome especificado.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-193">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="b9fd8-194">Neste exemplo, somente as pessoas cujo nome de exibição é igual a "Nestor Kellum" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-194">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="b9fd8-195">Pesquisar pessoas</span><span class="sxs-lookup"><span data-stu-id="b9fd8-195">Search people</span></span>

<span data-ttu-id="b9fd8-196">As solicitações nesta seção também obtêm as pessoas mais relevantes para o usuário conectado (`/me`).</span><span class="sxs-lookup"><span data-stu-id="b9fd8-196">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="b9fd8-197">As solicitações de pesquisa exigem a permissão People. Read.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-197">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="b9fd8-198">Usando a pesquisa para selecionar pessoas</span><span class="sxs-lookup"><span data-stu-id="b9fd8-198">Using search to select people</span></span>

<span data-ttu-id="b9fd8-199">Use o parâmetro *$search* para selecionar as pessoas que atendem a determinado conjunto de critérios.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-199">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="b9fd8-200">A consulta de pesquisa a seguir retorna pessoas `/me` relevantes para o qual o determinadoname ou o sobrenome começa com a letra "j".</span><span class="sxs-lookup"><span data-stu-id="b9fd8-200">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="b9fd8-201">Uso da pesquisa para especificar um tópico relevante</span><span class="sxs-lookup"><span data-stu-id="b9fd8-201">Using search to specify a relevant topic</span></span>

<span data-ttu-id="b9fd8-202">A solicitação a seguir retorna pessoas relevantes `/me` para o nome que contém "ma" e que têm uma associação com "planejamento de recursos".</span><span class="sxs-lookup"><span data-stu-id="b9fd8-202">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="b9fd8-203">Execução de uma pesquisa difusa</span><span class="sxs-lookup"><span data-stu-id="b9fd8-203">Performing a fuzzy search</span></span>

<span data-ttu-id="b9fd8-204">A solicitação a seguir faz uma pesquisa por uma pessoa chamada "Hermaini Sousa".</span><span class="sxs-lookup"><span data-stu-id="b9fd8-204">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="b9fd8-205">Como há uma pessoa denominada "Herminia Hull" relevante para o usuário conectado, as informações de "Herminia Hull" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-205">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="b9fd8-206">Pessoas relacionadas</span><span class="sxs-lookup"><span data-stu-id="b9fd8-206">Related people</span></span>

<span data-ttu-id="b9fd8-207">A solicitação a seguir obtém as pessoas mais relevantes para outra pessoa na organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-207">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="b9fd8-208">Essa solicitação exige o User. ReadBasic. All para a permissão People. Read. All.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-208">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="b9fd8-209">Neste exemplo, as pessoas relevantes do Marcos Kellum são exibidas.</span><span class="sxs-lookup"><span data-stu-id="b9fd8-209">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
