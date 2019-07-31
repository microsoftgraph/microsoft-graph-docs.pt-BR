---
title: Listar pessoas
description: Recupere uma lista de objetos Person ordenados por sua relevância para o usuário, que é determinado pelos padrões de comunicação e colaboração do usuário e relações comerciais.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: f2909dd1d14c7d10aa3aeba2ec9dd5c4224e0bd2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987576"
---
# <a name="list-people"></a><span data-ttu-id="e0c75-103">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="e0c75-103">List people</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0c75-104">Recupere uma lista de objetos [Person](../resources/person.md) ordenados por sua relevância para o [usuário](../resources/user.md), que é determinado pelos padrões de comunicação e colaboração do usuário e relações comerciais.</span><span class="sxs-lookup"><span data-stu-id="e0c75-104">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0c75-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0c75-105">Permissions</span></span>

<span data-ttu-id="e0c75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0c75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0c75-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0c75-108">Permission type</span></span>      | <span data-ttu-id="e0c75-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0c75-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0c75-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0c75-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0c75-111">People.Read</span><span class="sxs-lookup"><span data-stu-id="e0c75-111">People.Read</span></span>    |
|<span data-ttu-id="e0c75-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0c75-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0c75-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="e0c75-113">People.Read</span></span>    |
|<span data-ttu-id="e0c75-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0c75-114">Application</span></span> | <span data-ttu-id="e0c75-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0c75-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0c75-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0c75-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0c75-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0c75-117">Optional query parameters</span></span>

<span data-ttu-id="e0c75-118">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0c75-118">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="e0c75-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e0c75-119">Name</span></span>|<span data-ttu-id="e0c75-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e0c75-120">Value</span></span>|<span data-ttu-id="e0c75-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0c75-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="e0c75-122">$filter</span><span class="sxs-lookup"><span data-stu-id="e0c75-122">$filter</span></span>|<span data-ttu-id="e0c75-123">string</span><span class="sxs-lookup"><span data-stu-id="e0c75-123">string</span></span>|<span data-ttu-id="e0c75-124">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="e0c75-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="e0c75-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="e0c75-125">$orderby</span></span>|<span data-ttu-id="e0c75-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0c75-126">string</span></span>|<span data-ttu-id="e0c75-127">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="e0c75-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="e0c75-128">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="e0c75-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="e0c75-129">$search</span><span class="sxs-lookup"><span data-stu-id="e0c75-129">$search</span></span>|<span data-ttu-id="e0c75-130">string</span><span class="sxs-lookup"><span data-stu-id="e0c75-130">string</span></span>|<span data-ttu-id="e0c75-131">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="e0c75-131">Search for people by name or alias.</span></span> <span data-ttu-id="e0c75-132">Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="e0c75-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="e0c75-133">O parâmetro só funciona para pesquisar pessoas relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários.</span><span class="sxs-lookup"><span data-stu-id="e0c75-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="e0c75-134">Também dá suporte a `topic` palavra-chave para encontrar pessoas com base em tópicos extraídos a partir de conversas de email com essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="e0c75-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="e0c75-135">Confira a seção \*Realizar uma pesquisa difusa \* em [Obter informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para informações e exemplos.</span><span class="sxs-lookup"><span data-stu-id="e0c75-135">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="e0c75-136">$select</span><span class="sxs-lookup"><span data-stu-id="e0c75-136">$select</span></span>|<span data-ttu-id="e0c75-137">string</span><span class="sxs-lookup"><span data-stu-id="e0c75-137">string</span></span>|<span data-ttu-id="e0c75-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="e0c75-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="e0c75-140">$skip</span><span class="sxs-lookup"><span data-stu-id="e0c75-140">$skip</span></span>|<span data-ttu-id="e0c75-141">int</span><span class="sxs-lookup"><span data-stu-id="e0c75-141">int</span></span>|<span data-ttu-id="e0c75-p105">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="e0c75-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="e0c75-144">$top</span><span class="sxs-lookup"><span data-stu-id="e0c75-144">$top</span></span>|<span data-ttu-id="e0c75-145">int</span><span class="sxs-lookup"><span data-stu-id="e0c75-145">int</span></span>|<span data-ttu-id="e0c75-146">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="e0c75-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e0c75-147">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c75-147">Request headers</span></span>

| <span data-ttu-id="e0c75-148">Nome</span><span class="sxs-lookup"><span data-stu-id="e0c75-148">Name</span></span>      |<span data-ttu-id="e0c75-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0c75-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0c75-150">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0c75-150">Authorization</span></span>  | <span data-ttu-id="e0c75-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0c75-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0c75-153">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0c75-153">Accept</span></span> | <span data-ttu-id="e0c75-154">application/json</span><span class="sxs-lookup"><span data-stu-id="e0c75-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0c75-155">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c75-155">Request body</span></span>

<span data-ttu-id="e0c75-156">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0c75-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0c75-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c75-157">Response</span></span>

<span data-ttu-id="e0c75-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Person](../resources/person.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0c75-158">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0c75-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e0c75-159">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="e0c75-160">Browse</span><span class="sxs-lookup"><span data-stu-id="e0c75-160">Browse</span></span>

<span data-ttu-id="e0c75-161">As solicitações nesta seção obtêm as pessoas mais relevantes para o usuário conectado (`/me`), com base nas relações de comunicação, colaboração e negócios.</span><span class="sxs-lookup"><span data-stu-id="e0c75-161">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="e0c75-162">Por padrão, cada resposta retorna 10 registros, mas você pode alterar esse número usando o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="e0c75-162">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="e0c75-163">Essas solicitações exigem a permissão People. Read.</span><span class="sxs-lookup"><span data-stu-id="e0c75-163">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="e0c75-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c75-164">Request</span></span>

<span data-ttu-id="e0c75-165">Veja a seguir um exemplo da solicitação padrão.</span><span class="sxs-lookup"><span data-stu-id="e0c75-165">The following is an example of the default request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e0c75-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0c75-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e0c75-167">C#</span><span class="sxs-lookup"><span data-stu-id="e0c75-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0c75-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0c75-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e0c75-169">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e0c75-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e0c75-170">Java</span><span class="sxs-lookup"><span data-stu-id="e0c75-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e0c75-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c75-171">Response</span></span>

<span data-ttu-id="e0c75-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0c75-172">The following is an example of the response.</span></span>
><span data-ttu-id="e0c75-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0c75-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="e0c75-175">Solicitação de uma página subsequente de pessoas</span><span class="sxs-lookup"><span data-stu-id="e0c75-175">Requesting a subsequent page of people</span></span>

<span data-ttu-id="e0c75-p109">Se a primeira resposta não contiver a lista completa das pessoas relevantes, você poderá fazer uma segunda solicitação usando *$top* e *$skip* para solicitar páginas adicionais de informações. Se a solicitação anterior tiver informações adicionais, a solicitação a seguir obterá a próxima página de pessoas do servidor.</span><span class="sxs-lookup"><span data-stu-id="e0c75-p109">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="e0c75-178">Classificar a resposta</span><span class="sxs-lookup"><span data-stu-id="e0c75-178">Sort the response</span></span>

<span data-ttu-id="e0c75-179">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="e0c75-179">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="e0c75-180">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="e0c75-180">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="e0c75-181">Essa consulta seleciona as pessoas mais relevantes para você classificando-as pelo nome de exibição e retorna as dez primeiras pessoas da lista classificada.</span><span class="sxs-lookup"><span data-stu-id="e0c75-181">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="e0c75-182">Alteração do número de pessoas e dos campos retornados</span><span class="sxs-lookup"><span data-stu-id="e0c75-182">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="e0c75-183">Você pode alterar o número de pessoas retornadas na resposta definindo o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="e0c75-183">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="e0c75-184">O exemplo a seguir solicita as 1.000 pessoas mais relevantes `/me`.</span><span class="sxs-lookup"><span data-stu-id="e0c75-184">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="e0c75-185">A solicitação também limita a quantidade de dados enviados de volta do servidor solicitando apenas o nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="e0c75-185">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="e0c75-186">Seleção dos campos que devem ser retornados</span><span class="sxs-lookup"><span data-stu-id="e0c75-186">Selecting the fields to return</span></span>

<span data-ttu-id="e0c75-187">Você pode limitar a quantidade de dados retornados do servidor usando o parâmetro *$Select* para escolher um ou mais campos.</span><span class="sxs-lookup"><span data-stu-id="e0c75-187">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="e0c75-188">O campo *@odata.id* é sempre retornado.</span><span class="sxs-lookup"><span data-stu-id="e0c75-188">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="e0c75-189">O exemplo a seguir limita a resposta para *DisplayName* e *EmailAddress* das dez pessoas mais relevantes.</span><span class="sxs-lookup"><span data-stu-id="e0c75-189">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="e0c75-190">Uso de um filtro para limitar a resposta</span><span class="sxs-lookup"><span data-stu-id="e0c75-190">Using a filter to limit the response</span></span>

<span data-ttu-id="e0c75-191">Você pode usar o parâmetro *$filter* para limitar a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="e0c75-191">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="e0c75-192">A consulta a seguir limita a resposta a pessoas com o "diretório" de origem.</span><span class="sxs-lookup"><span data-stu-id="e0c75-192">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="e0c75-193">Selecionar os campos a serem retornados em uma resposta filtrada</span><span class="sxs-lookup"><span data-stu-id="e0c75-193">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="e0c75-194">Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e0c75-194">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="e0c75-195">O exemplo a seguir obtém o *DisplayName* e o *EmailAddress* de pessoas cujo nome de exibição é igual ao nome especificado.</span><span class="sxs-lookup"><span data-stu-id="e0c75-195">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="e0c75-196">Neste exemplo, somente as pessoas cujo nome de exibição é igual a "Nestor Kellum" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="e0c75-196">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="e0c75-197">Pesquisar pessoas</span><span class="sxs-lookup"><span data-stu-id="e0c75-197">Search people</span></span>

<span data-ttu-id="e0c75-198">As solicitações nesta seção também obtêm as pessoas mais relevantes para o usuário conectado (`/me`).</span><span class="sxs-lookup"><span data-stu-id="e0c75-198">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="e0c75-199">As solicitações de pesquisa exigem a permissão People. Read.</span><span class="sxs-lookup"><span data-stu-id="e0c75-199">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="e0c75-200">Usando a pesquisa para selecionar pessoas</span><span class="sxs-lookup"><span data-stu-id="e0c75-200">Using search to select people</span></span>

<span data-ttu-id="e0c75-201">Use o parâmetro *$search* para selecionar as pessoas que atendem a determinado conjunto de critérios.</span><span class="sxs-lookup"><span data-stu-id="e0c75-201">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="e0c75-202">A consulta de pesquisa a seguir retorna pessoas `/me` relevantes para o qual o determinadoname ou o sobrenome começa com a letra "j".</span><span class="sxs-lookup"><span data-stu-id="e0c75-202">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="e0c75-203">Uso da pesquisa para especificar um tópico relevante</span><span class="sxs-lookup"><span data-stu-id="e0c75-203">Using search to specify a relevant topic</span></span>

<span data-ttu-id="e0c75-204">A solicitação a seguir retorna pessoas relevantes `/me` para o nome que contém "ma" e que têm uma associação com "planejamento de recursos".</span><span class="sxs-lookup"><span data-stu-id="e0c75-204">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="e0c75-205">Execução de uma pesquisa difusa</span><span class="sxs-lookup"><span data-stu-id="e0c75-205">Performing a fuzzy search</span></span>

<span data-ttu-id="e0c75-206">A solicitação a seguir faz uma pesquisa por uma pessoa chamada "Hermaini Sousa".</span><span class="sxs-lookup"><span data-stu-id="e0c75-206">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="e0c75-207">Como há uma pessoa denominada "Herminia Hull" relevante para o usuário conectado, as informações de "Herminia Hull" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="e0c75-207">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="e0c75-208">Pessoas relacionadas</span><span class="sxs-lookup"><span data-stu-id="e0c75-208">Related people</span></span>

<span data-ttu-id="e0c75-209">A solicitação a seguir obtém as pessoas mais relevantes para outra pessoa na organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="e0c75-209">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="e0c75-210">Essa solicitação exige o User. ReadBasic. All para a permissão People. Read. All.</span><span class="sxs-lookup"><span data-stu-id="e0c75-210">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="e0c75-211">Neste exemplo, as pessoas relevantes do Marcos Kellum são exibidas.</span><span class="sxs-lookup"><span data-stu-id="e0c75-211">In this example, Nestor Kellum's relevant people are displayed.</span></span>

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
  ]
}
-->
