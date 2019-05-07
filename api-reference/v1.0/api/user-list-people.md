---
title: Listar pessoas
description: Recupere uma coleção de objetos person ordenados por relevância para o usuário, o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.
author: dkershaw10
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: bc314bfd0e13808ddc400a6acb552db6c34e1e64
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601588"
---
# <a name="list-people"></a><span data-ttu-id="04099-103">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="04099-103">List people</span></span>

<span data-ttu-id="04099-104">Recupere uma coleção de objetos [person](../resources/person.md) ordenados por relevância para o [usuário](../resources/user.md), o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="04099-104">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="04099-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="04099-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="04099-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="04099-107">Permissions</span></span>

<span data-ttu-id="04099-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04099-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04099-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04099-110">Permission type</span></span>      | <span data-ttu-id="04099-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04099-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04099-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04099-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04099-113">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="04099-113">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="04099-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04099-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04099-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="04099-115">People.Read</span></span>    |
|<span data-ttu-id="04099-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04099-116">Application</span></span> | <span data-ttu-id="04099-117">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="04099-117">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04099-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04099-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04099-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04099-119">Optional query parameters</span></span>

<span data-ttu-id="04099-120">Este método oferece suporte aos [ parâmetros de consulta OData ](/graph/query-parameters) para personalizar a resposta, como mostrado nos exemplos no artigo [Obter informações relevantes sobre pessoas](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="04099-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="04099-121">Nome</span><span class="sxs-lookup"><span data-stu-id="04099-121">Name</span></span>|<span data-ttu-id="04099-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04099-122">Value</span></span>|<span data-ttu-id="04099-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="04099-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="04099-124">$filter</span><span class="sxs-lookup"><span data-stu-id="04099-124">$filter</span></span>|<span data-ttu-id="04099-125">string</span><span class="sxs-lookup"><span data-stu-id="04099-125">string</span></span>|<span data-ttu-id="04099-126">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="04099-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="04099-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="04099-127">$orderby</span></span>|<span data-ttu-id="04099-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04099-128">string</span></span>|<span data-ttu-id="04099-129">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="04099-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="04099-130">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="04099-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="04099-131">$search</span><span class="sxs-lookup"><span data-stu-id="04099-131">$search</span></span>|<span data-ttu-id="04099-132">string</span><span class="sxs-lookup"><span data-stu-id="04099-132">string</span></span>|<span data-ttu-id="04099-133">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="04099-133">Search for people by name or alias.</span></span> <span data-ttu-id="04099-134">Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="04099-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="04099-135">O parâmetro só funciona para pesquisar pessoas relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários.</span><span class="sxs-lookup"><span data-stu-id="04099-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="04099-136">Também dá suporte a `topic` palavra-chave para encontrar pessoas com base em tópicos extraídos a partir de conversas de email com essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="04099-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="04099-137">Confira a seção \*Realizar uma pesquisa difusa \* em [Obter informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para informações e exemplos.</span><span class="sxs-lookup"><span data-stu-id="04099-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="04099-138">$select</span><span class="sxs-lookup"><span data-stu-id="04099-138">$select</span></span>|<span data-ttu-id="04099-139">string</span><span class="sxs-lookup"><span data-stu-id="04099-139">string</span></span>|<span data-ttu-id="04099-p105">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="04099-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="04099-142">$skip</span><span class="sxs-lookup"><span data-stu-id="04099-142">$skip</span></span>|<span data-ttu-id="04099-143">int</span><span class="sxs-lookup"><span data-stu-id="04099-143">int</span></span>|<span data-ttu-id="04099-p106">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="04099-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="04099-146">$top</span><span class="sxs-lookup"><span data-stu-id="04099-146">$top</span></span>|<span data-ttu-id="04099-147">int</span><span class="sxs-lookup"><span data-stu-id="04099-147">int</span></span>|<span data-ttu-id="04099-148">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="04099-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="04099-149">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04099-149">Request headers</span></span>

| <span data-ttu-id="04099-150">Nome</span><span class="sxs-lookup"><span data-stu-id="04099-150">Name</span></span>      |<span data-ttu-id="04099-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="04099-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="04099-152">Autorização</span><span class="sxs-lookup"><span data-stu-id="04099-152">Authorization</span></span>  | <span data-ttu-id="04099-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04099-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04099-155">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04099-155">Accept</span></span> | <span data-ttu-id="04099-156">application/json</span><span class="sxs-lookup"><span data-stu-id="04099-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="04099-157">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04099-157">Request body</span></span>

<span data-ttu-id="04099-158">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04099-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04099-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="04099-159">Response</span></span>

<span data-ttu-id="04099-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [person](../resources/person.md) no corpo da resposta. A resposta pode conter um objeto person ou uma coleção de objetos person.</span><span class="sxs-lookup"><span data-stu-id="04099-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="04099-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="04099-162">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="04099-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04099-163">Request</span></span>

<span data-ttu-id="04099-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04099-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="04099-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="04099-165">Response</span></span>

<span data-ttu-id="04099-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04099-166">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="04099-167">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="04099-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="04099-168">C#</span><span class="sxs-lookup"><span data-stu-id="04099-168">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_person_collection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04099-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="04099-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_person_collection-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="04099-170">Para ver mais exemplos, confira o artigo [Obter informações relevantes sobre as pessoas](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="04099-170">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
