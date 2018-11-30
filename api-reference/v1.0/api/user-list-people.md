---
title: Listar pessoas
description: Recupere uma coleção de objetos person ordenados por relevância para o usuário, o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.
ms.openlocfilehash: 89bc3fefbc190df60151f65eb265f02196754d3d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005039"
---
# <a name="list-people"></a><span data-ttu-id="119eb-103">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="119eb-103">List people</span></span>

<span data-ttu-id="119eb-104">Recupere uma coleção de objetos [person](../resources/person.md) ordenados por relevância para o [usuário](../resources/user.md), o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="119eb-104">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="119eb-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="119eb-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="119eb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="119eb-107">Permissions</span></span>

<span data-ttu-id="119eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="119eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="119eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="119eb-110">Permission type</span></span>      | <span data-ttu-id="119eb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="119eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="119eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="119eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="119eb-113">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="119eb-113">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="119eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="119eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="119eb-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="119eb-115">People.Read</span></span>    |
|<span data-ttu-id="119eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="119eb-116">Application</span></span> | <span data-ttu-id="119eb-117">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="119eb-117">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="119eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="119eb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="119eb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="119eb-119">Optional query parameters</span></span>

<span data-ttu-id="119eb-120">Este método oferece suporte aos [ parâmetros de consulta OData ](/graph/query-parameters) para personalizar a resposta, como mostrado nos exemplos no artigo [Obter informações relevantes sobre pessoas](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="119eb-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="119eb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="119eb-121">Name</span></span>|<span data-ttu-id="119eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="119eb-122">Value</span></span>|<span data-ttu-id="119eb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="119eb-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="119eb-124">$filter</span><span class="sxs-lookup"><span data-stu-id="119eb-124">$filter</span></span>|<span data-ttu-id="119eb-125">string</span><span class="sxs-lookup"><span data-stu-id="119eb-125">string</span></span>|<span data-ttu-id="119eb-126">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="119eb-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="119eb-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="119eb-127">$orderby</span></span>|<span data-ttu-id="119eb-128">string</span><span class="sxs-lookup"><span data-stu-id="119eb-128">string</span></span>|<span data-ttu-id="119eb-129">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="119eb-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="119eb-130">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="119eb-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="119eb-131">$search</span><span class="sxs-lookup"><span data-stu-id="119eb-131">$search</span></span>|<span data-ttu-id="119eb-132">string</span><span class="sxs-lookup"><span data-stu-id="119eb-132">string</span></span>|<span data-ttu-id="119eb-133">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="119eb-133">Search for people by name or alias.</span></span> <span data-ttu-id="119eb-134">Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="119eb-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="119eb-135">Parâmetro funciona apenas para a pesquisa de pessoas de relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários.</span><span class="sxs-lookup"><span data-stu-id="119eb-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="119eb-136">Também oferece suporte a `topic` palavra-chave para localizar pessoas com base em tópicos extraídos de conversas de email com essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="119eb-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="119eb-137">Consulte a seção de *executar uma pesquisa difusa* em [obter as informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para obter informações e exemplos.</span><span class="sxs-lookup"><span data-stu-id="119eb-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="119eb-138">$select</span><span class="sxs-lookup"><span data-stu-id="119eb-138">$select</span></span>|<span data-ttu-id="119eb-139">string</span><span class="sxs-lookup"><span data-stu-id="119eb-139">string</span></span>|<span data-ttu-id="119eb-p105">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="119eb-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="119eb-142">$skip</span><span class="sxs-lookup"><span data-stu-id="119eb-142">$skip</span></span>|<span data-ttu-id="119eb-143">inteiro</span><span class="sxs-lookup"><span data-stu-id="119eb-143">int</span></span>|<span data-ttu-id="119eb-p106">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="119eb-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="119eb-146">$top</span><span class="sxs-lookup"><span data-stu-id="119eb-146">$top</span></span>|<span data-ttu-id="119eb-147">inteiro</span><span class="sxs-lookup"><span data-stu-id="119eb-147">int</span></span>|<span data-ttu-id="119eb-148">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="119eb-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="119eb-149">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="119eb-149">Request headers</span></span>

| <span data-ttu-id="119eb-150">Nome</span><span class="sxs-lookup"><span data-stu-id="119eb-150">Name</span></span>      |<span data-ttu-id="119eb-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="119eb-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="119eb-152">Autorização</span><span class="sxs-lookup"><span data-stu-id="119eb-152">Authorization</span></span>  | <span data-ttu-id="119eb-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="119eb-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="119eb-155">Aceitar</span><span class="sxs-lookup"><span data-stu-id="119eb-155">Accept</span></span> | <span data-ttu-id="119eb-156">application/json</span><span class="sxs-lookup"><span data-stu-id="119eb-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="119eb-157">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="119eb-157">Request body</span></span>

<span data-ttu-id="119eb-158">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="119eb-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="119eb-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="119eb-159">Response</span></span>

<span data-ttu-id="119eb-p108">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [person](../resources/person.md) no corpo da resposta. A resposta pode conter um objeto person ou uma coleção de objetos person.</span><span class="sxs-lookup"><span data-stu-id="119eb-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="119eb-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="119eb-162">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="119eb-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="119eb-163">Request</span></span>

<span data-ttu-id="119eb-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="119eb-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="119eb-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="119eb-165">Response</span></span>

<span data-ttu-id="119eb-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="119eb-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="119eb-167">Para ver mais exemplos, confira o artigo [Obter informações relevantes sobre as pessoas](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="119eb-167">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
