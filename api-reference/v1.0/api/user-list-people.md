---
title: Listar pessoas
description: Recupere uma coleção de objetos person ordenados por relevância para o usuário, o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.
author: dkershaw10
localization_priority: Priority
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0ae6dd0d81435626b4205eba581576002ef35de4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992080"
---
# <a name="list-people"></a><span data-ttu-id="a8750-103">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="a8750-103">List people</span></span>

<span data-ttu-id="a8750-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8750-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8750-105">Recupere uma coleção de objetos [person](../resources/person.md) ordenados por relevância para o [usuário](../resources/user.md), o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="a8750-105">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="a8750-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="a8750-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8750-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8750-108">Permissions</span></span>

<span data-ttu-id="a8750-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8750-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8750-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8750-111">Permission type</span></span>      | <span data-ttu-id="a8750-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8750-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8750-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8750-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a8750-114">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8750-114">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="a8750-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8750-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8750-116">People.Read</span><span class="sxs-lookup"><span data-stu-id="a8750-116">People.Read</span></span>    |
|<span data-ttu-id="a8750-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8750-117">Application</span></span> | <span data-ttu-id="a8750-118">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8750-118">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8750-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8750-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8750-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8750-120">Optional query parameters</span></span>

<span data-ttu-id="a8750-121">Este método oferece suporte aos [ parâmetros de consulta OData ](/graph/query-parameters) para personalizar a resposta, como mostrado nos exemplos no artigo [Obter informações relevantes sobre pessoas](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="a8750-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="a8750-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a8750-122">Name</span></span>|<span data-ttu-id="a8750-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a8750-123">Value</span></span>|<span data-ttu-id="a8750-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8750-124">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="a8750-125">$filter</span><span class="sxs-lookup"><span data-stu-id="a8750-125">$filter</span></span>|<span data-ttu-id="a8750-126">string</span><span class="sxs-lookup"><span data-stu-id="a8750-126">string</span></span>|<span data-ttu-id="a8750-127">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="a8750-127">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="a8750-128">$orderby</span><span class="sxs-lookup"><span data-stu-id="a8750-128">$orderby</span></span>|<span data-ttu-id="a8750-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8750-129">string</span></span>|<span data-ttu-id="a8750-130">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="a8750-130">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="a8750-131">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="a8750-131">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="a8750-132">$search</span><span class="sxs-lookup"><span data-stu-id="a8750-132">$search</span></span>|<span data-ttu-id="a8750-133">string</span><span class="sxs-lookup"><span data-stu-id="a8750-133">string</span></span>|<span data-ttu-id="a8750-134">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="a8750-134">Search for people by name or alias.</span></span> <span data-ttu-id="a8750-135">Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="a8750-135">Supports Fuzzy matching.</span></span> <span data-ttu-id="a8750-136">O parâmetro só funciona para pesquisar pessoas relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários.</span><span class="sxs-lookup"><span data-stu-id="a8750-136">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="a8750-137">Também dá suporte a `topic` palavra-chave para encontrar pessoas com base em tópicos extraídos a partir de conversas de email com essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="a8750-137">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="a8750-138">Confira a seção \*Realizar uma pesquisa difusa \* em [Obter informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para informações e exemplos.</span><span class="sxs-lookup"><span data-stu-id="a8750-138">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="a8750-139">$select</span><span class="sxs-lookup"><span data-stu-id="a8750-139">$select</span></span>|<span data-ttu-id="a8750-140">string</span><span class="sxs-lookup"><span data-stu-id="a8750-140">string</span></span>|<span data-ttu-id="a8750-p105">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="a8750-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="a8750-143">$skip</span><span class="sxs-lookup"><span data-stu-id="a8750-143">$skip</span></span>|<span data-ttu-id="a8750-144">int</span><span class="sxs-lookup"><span data-stu-id="a8750-144">int</span></span>|<span data-ttu-id="a8750-p106">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="a8750-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="a8750-147">$top</span><span class="sxs-lookup"><span data-stu-id="a8750-147">$top</span></span>|<span data-ttu-id="a8750-148">int</span><span class="sxs-lookup"><span data-stu-id="a8750-148">int</span></span>|<span data-ttu-id="a8750-149">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="a8750-149">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="a8750-150">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8750-150">Request headers</span></span>

| <span data-ttu-id="a8750-151">Nome</span><span class="sxs-lookup"><span data-stu-id="a8750-151">Name</span></span>      |<span data-ttu-id="a8750-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8750-152">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a8750-153">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8750-153">Authorization</span></span>  | <span data-ttu-id="a8750-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8750-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8750-156">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8750-156">Accept</span></span> | <span data-ttu-id="a8750-157">application/json</span><span class="sxs-lookup"><span data-stu-id="a8750-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8750-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8750-158">Request body</span></span>

<span data-ttu-id="a8750-159">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8750-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8750-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8750-160">Response</span></span>

<span data-ttu-id="a8750-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [person](../resources/person.md) no corpo da resposta. A resposta pode conter um objeto person ou uma coleção de objetos person.</span><span class="sxs-lookup"><span data-stu-id="a8750-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="a8750-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8750-163">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="a8750-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8750-164">Request</span></span>

<span data-ttu-id="a8750-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8750-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8750-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8750-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/people
```
# <a name="c"></a>[<span data-ttu-id="a8750-167">C#</span><span class="sxs-lookup"><span data-stu-id="a8750-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8750-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8750-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8750-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8750-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8750-170">Java</span><span class="sxs-lookup"><span data-stu-id="a8750-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a8750-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8750-171">Response</span></span>

<span data-ttu-id="a8750-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8750-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="a8750-173">Para ver mais exemplos, confira o artigo [Obter informações relevantes sobre as pessoas](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="a8750-173">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

