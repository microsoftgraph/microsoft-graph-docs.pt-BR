---
title: Listar pessoas
description: Recupere uma lista de objetos person ordenados por relevância para o usuário, o que é determinado pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 8df99c32c43e947863c4a7713c984b99fbd4bb73
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053353"
---
# <a name="list-people"></a><span data-ttu-id="90e67-103">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="90e67-103">List people</span></span>

<span data-ttu-id="90e67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90e67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90e67-105">Recupere uma lista de [objetos](../resources/person.md) de pessoa ordenados por sua relevância para o usuário [,](../resources/user.md)que é determinado pelos padrões de comunicação e colaboração do usuário e pelas relações comerciais.</span><span class="sxs-lookup"><span data-stu-id="90e67-105">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="90e67-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="90e67-106">Permissions</span></span>

<span data-ttu-id="90e67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90e67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90e67-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90e67-109">Permission type</span></span>      | <span data-ttu-id="90e67-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90e67-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90e67-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90e67-111">Delegated (work or school account)</span></span> | <span data-ttu-id="90e67-112">People.Read</span><span class="sxs-lookup"><span data-stu-id="90e67-112">People.Read</span></span>    |
|<span data-ttu-id="90e67-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90e67-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90e67-114">People.Read</span><span class="sxs-lookup"><span data-stu-id="90e67-114">People.Read</span></span>    |
|<span data-ttu-id="90e67-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90e67-115">Application</span></span> | <span data-ttu-id="90e67-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90e67-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90e67-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90e67-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90e67-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="90e67-118">Optional query parameters</span></span>

<span data-ttu-id="90e67-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="90e67-119">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="90e67-120">Nome</span><span class="sxs-lookup"><span data-stu-id="90e67-120">Name</span></span>|<span data-ttu-id="90e67-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90e67-121">Value</span></span>|<span data-ttu-id="90e67-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="90e67-122">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="90e67-123">$filter</span><span class="sxs-lookup"><span data-stu-id="90e67-123">$filter</span></span>|<span data-ttu-id="90e67-124">string</span><span class="sxs-lookup"><span data-stu-id="90e67-124">string</span></span>|<span data-ttu-id="90e67-125">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="90e67-125">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="90e67-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="90e67-126">$orderby</span></span>|<span data-ttu-id="90e67-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90e67-127">string</span></span>|<span data-ttu-id="90e67-128">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="90e67-128">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="90e67-129">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="90e67-129">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="90e67-130">$search</span><span class="sxs-lookup"><span data-stu-id="90e67-130">$search</span></span>|<span data-ttu-id="90e67-131">string</span><span class="sxs-lookup"><span data-stu-id="90e67-131">string</span></span>|<span data-ttu-id="90e67-132">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="90e67-132">Search for people by name or alias.</span></span> <span data-ttu-id="90e67-133">Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="90e67-133">Supports Fuzzy matching.</span></span> <span data-ttu-id="90e67-134">O parâmetro só funciona para pesquisar pessoas relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários.</span><span class="sxs-lookup"><span data-stu-id="90e67-134">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="90e67-135">Também dá suporte a `topic` palavra-chave para encontrar pessoas com base em tópicos extraídos a partir de conversas de email com essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="90e67-135">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="90e67-136">Confira a seção *Realizar uma pesquisa difusa* em [Obter informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para informações e exemplos.</span><span class="sxs-lookup"><span data-stu-id="90e67-136">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="90e67-137">$select</span><span class="sxs-lookup"><span data-stu-id="90e67-137">$select</span></span>|<span data-ttu-id="90e67-138">string</span><span class="sxs-lookup"><span data-stu-id="90e67-138">string</span></span>|<span data-ttu-id="90e67-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="90e67-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="90e67-141">$skip</span><span class="sxs-lookup"><span data-stu-id="90e67-141">$skip</span></span>|<span data-ttu-id="90e67-142">int</span><span class="sxs-lookup"><span data-stu-id="90e67-142">int</span></span>|<span data-ttu-id="90e67-p105">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="90e67-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="90e67-145">$top</span><span class="sxs-lookup"><span data-stu-id="90e67-145">$top</span></span>|<span data-ttu-id="90e67-146">int</span><span class="sxs-lookup"><span data-stu-id="90e67-146">int</span></span>|<span data-ttu-id="90e67-147">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="90e67-147">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="90e67-148">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90e67-148">Request headers</span></span>

| <span data-ttu-id="90e67-149">Nome</span><span class="sxs-lookup"><span data-stu-id="90e67-149">Name</span></span>      |<span data-ttu-id="90e67-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="90e67-150">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90e67-151">Autorização</span><span class="sxs-lookup"><span data-stu-id="90e67-151">Authorization</span></span>  | <span data-ttu-id="90e67-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90e67-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90e67-154">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90e67-154">Accept</span></span> | <span data-ttu-id="90e67-155">application/json</span><span class="sxs-lookup"><span data-stu-id="90e67-155">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="90e67-156">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90e67-156">Request body</span></span>

<span data-ttu-id="90e67-157">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90e67-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90e67-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="90e67-158">Response</span></span>

<span data-ttu-id="90e67-159">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [person](../resources/person.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90e67-159">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90e67-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90e67-160">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="90e67-161">Procurar</span><span class="sxs-lookup"><span data-stu-id="90e67-161">Browse</span></span>

<span data-ttu-id="90e67-162">As solicitações nesta seção têm as pessoas mais relevantes para o usuário ( ), com base na `/me` comunicação, colaboração e relações comerciais.</span><span class="sxs-lookup"><span data-stu-id="90e67-162">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="90e67-163">Por padrão, cada resposta retorna 10 registros, mas você pode alterar esse número usando o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="90e67-163">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="90e67-164">Essas solicitações exigem a permissão People.Read.</span><span class="sxs-lookup"><span data-stu-id="90e67-164">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="90e67-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90e67-165">Request</span></span>

<span data-ttu-id="90e67-166">A seguir, um exemplo da solicitação padrão.</span><span class="sxs-lookup"><span data-stu-id="90e67-166">The following is an example of the default request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90e67-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="90e67-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/people
```
# <a name="c"></a>[<span data-ttu-id="90e67-168">C#</span><span class="sxs-lookup"><span data-stu-id="90e67-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90e67-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90e67-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90e67-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90e67-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90e67-171">Java</span><span class="sxs-lookup"><span data-stu-id="90e67-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90e67-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="90e67-172">Response</span></span>

<span data-ttu-id="90e67-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90e67-173">The following is an example of the response.</span></span>
><span data-ttu-id="90e67-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="90e67-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="90e67-175">Solicitação de uma página subsequente de pessoas</span><span class="sxs-lookup"><span data-stu-id="90e67-175">Requesting a subsequent page of people</span></span>

<span data-ttu-id="90e67-p108">Se a primeira resposta não contiver a lista completa das pessoas relevantes, você poderá fazer uma segunda solicitação usando *$top* e *$skip* para solicitar páginas adicionais de informações. Se a solicitação anterior tiver informações adicionais, a solicitação a seguir obterá a próxima página de pessoas do servidor.</span><span class="sxs-lookup"><span data-stu-id="90e67-p108">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="90e67-178">Classificar a resposta</span><span class="sxs-lookup"><span data-stu-id="90e67-178">Sort the response</span></span>

<span data-ttu-id="90e67-179">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="90e67-179">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="90e67-180">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="90e67-180">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="90e67-181">Essa consulta seleciona as pessoas mais relevantes para você classificando-as pelo nome de exibição e retorna as dez primeiras pessoas da lista classificada.</span><span class="sxs-lookup"><span data-stu-id="90e67-181">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="90e67-182">Alteração do número de pessoas e dos campos retornados</span><span class="sxs-lookup"><span data-stu-id="90e67-182">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="90e67-183">Você pode alterar o número de pessoas retornadas na resposta definindo o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="90e67-183">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="90e67-184">O exemplo a seguir solicita as 1.000 pessoas mais relevantes para `/me` .</span><span class="sxs-lookup"><span data-stu-id="90e67-184">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="90e67-185">A solicitação também limita a quantidade de dados enviados de volta do servidor solicitando apenas o nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="90e67-185">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="90e67-186">Seleção dos campos que devem ser retornados</span><span class="sxs-lookup"><span data-stu-id="90e67-186">Selecting the fields to return</span></span>

<span data-ttu-id="90e67-187">Você pode limitar a quantidade de dados retornados do servidor usando o parâmetro *$select* para escolher um ou mais campos.</span><span class="sxs-lookup"><span data-stu-id="90e67-187">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="90e67-188">O campo *@odata.id* é sempre retornado.</span><span class="sxs-lookup"><span data-stu-id="90e67-188">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="90e67-189">O exemplo a seguir limita a resposta para *DisplayName* e *EmailAddress* das 10 pessoas mais relevantes.</span><span class="sxs-lookup"><span data-stu-id="90e67-189">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="90e67-190">Uso de um filtro para limitar a resposta</span><span class="sxs-lookup"><span data-stu-id="90e67-190">Using a filter to limit the response</span></span>

<span data-ttu-id="90e67-191">Você pode usar o parâmetro *$filter* para limitar a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="90e67-191">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="90e67-192">A consulta a seguir limita a resposta a pessoas com a origem "Directory".</span><span class="sxs-lookup"><span data-stu-id="90e67-192">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="90e67-193">Selecionando os campos para retornar em uma resposta filtrada</span><span class="sxs-lookup"><span data-stu-id="90e67-193">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="90e67-194">Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="90e67-194">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="90e67-195">O exemplo a seguir obtém *DisplayName* e *EmailAddress* de pessoas cujo nome de exibição é igual ao nome especificado.</span><span class="sxs-lookup"><span data-stu-id="90e67-195">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="90e67-196">Neste exemplo, somente as pessoas cujo nome de exibição é igual a "Nestor Kellum" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="90e67-196">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="90e67-197">Pesquisar pessoas</span><span class="sxs-lookup"><span data-stu-id="90e67-197">Search people</span></span>

<span data-ttu-id="90e67-198">As solicitações nesta seção também obterão as pessoas mais relevantes para o usuário de sessão ( `/me` ).</span><span class="sxs-lookup"><span data-stu-id="90e67-198">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="90e67-199">As solicitações de pesquisa exigem a permissão People.Read.</span><span class="sxs-lookup"><span data-stu-id="90e67-199">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="90e67-200">Usando a pesquisa para selecionar pessoas</span><span class="sxs-lookup"><span data-stu-id="90e67-200">Using search to select people</span></span>

<span data-ttu-id="90e67-201">Use o parâmetro *$search* para selecionar as pessoas que atendem a determinado conjunto de critérios.</span><span class="sxs-lookup"><span data-stu-id="90e67-201">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="90e67-202">A consulta de pesquisa a seguir retorna pessoas `/me` relevantes para cuja GivenName ou Sobrenome começa com a letra "j".</span><span class="sxs-lookup"><span data-stu-id="90e67-202">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="90e67-203">Uso da pesquisa para especificar um tópico relevante</span><span class="sxs-lookup"><span data-stu-id="90e67-203">Using search to specify a relevant topic</span></span>

<span data-ttu-id="90e67-204">A solicitação a seguir retorna pessoas relevantes cujo nome contém "ma" e que têm uma associação `/me` com "planejamento de recursos".</span><span class="sxs-lookup"><span data-stu-id="90e67-204">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="90e67-205">Execução de uma pesquisa difusa</span><span class="sxs-lookup"><span data-stu-id="90e67-205">Performing a fuzzy search</span></span>

<span data-ttu-id="90e67-206">A solicitação a seguir faz uma pesquisa para uma pessoa chamada "Hermaini Hall".</span><span class="sxs-lookup"><span data-stu-id="90e67-206">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="90e67-207">Como há uma pessoa chamada "Herminia Hull" relevante para o usuário in-loco, as informações de "Herminia Hull" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="90e67-207">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="90e67-208">Pessoas relacionadas</span><span class="sxs-lookup"><span data-stu-id="90e67-208">Related people</span></span>

<span data-ttu-id="90e67-209">A solicitação a seguir obtém as pessoas mais relevantes para outra pessoa na organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="90e67-209">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="90e67-210">Essa solicitação requer a permissão User.ReadBasic.All para People.Read.All.</span><span class="sxs-lookup"><span data-stu-id="90e67-210">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="90e67-211">Neste exemplo, as pessoas relevantes de Nestor Kellum são exibidas.</span><span class="sxs-lookup"><span data-stu-id="90e67-211">In this example, Nestor Kellum's relevant people are displayed.</span></span>

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


