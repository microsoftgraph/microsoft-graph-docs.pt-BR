---
title: Listar habilidades
description: Recupere uma lista de objetos skillProficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 78f91c8e3ba8a60278c0188bb5990d2aadbd8fb1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037162"
---
# <a name="list-skills"></a><span data-ttu-id="a7520-103">Listar habilidades</span><span class="sxs-lookup"><span data-stu-id="a7520-103">List skills</span></span>

<span data-ttu-id="a7520-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7520-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7520-105">Recupere uma lista de [objetos skillProficiency](../resources/skillproficiency.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="a7520-105">Retrieve a list of [skillProficiency](../resources/skillproficiency.md) objects in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7520-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7520-106">Permissions</span></span>

<span data-ttu-id="a7520-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7520-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7520-109">Permission type</span></span>                        | <span data-ttu-id="a7520-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7520-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="a7520-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7520-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7520-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7520-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a7520-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7520-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7520-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7520-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a7520-115">Application</span><span class="sxs-lookup"><span data-stu-id="a7520-115">Application</span></span>                            | <span data-ttu-id="a7520-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7520-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="a7520-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7520-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills
GET /users/{id | userPrincipalName}/profile/skills
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7520-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a7520-118">Optional query parameters</span></span>

<span data-ttu-id="a7520-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7520-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="a7520-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a7520-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="a7520-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a7520-121">Name</span></span>            |<span data-ttu-id="a7520-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7520-122">Value</span></span>    |<span data-ttu-id="a7520-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7520-123">Description</span></span>                                                                                                                                                                      |
|:---------------|:--------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="a7520-124">$filter</span><span class="sxs-lookup"><span data-stu-id="a7520-124">$filter</span></span>         |<span data-ttu-id="a7520-125">string</span><span class="sxs-lookup"><span data-stu-id="a7520-125">string</span></span>   |<span data-ttu-id="a7520-126">Limita a resposta apenas aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="a7520-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                                  |
|<span data-ttu-id="a7520-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="a7520-127">$orderby</span></span>        |<span data-ttu-id="a7520-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7520-128">string</span></span>   |<span data-ttu-id="a7520-129">Por padrão, os objetos na resposta são classificação pelo valor **createdDateTime** em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="a7520-129">By default, the objects in the response are sorted by their **createdDateTime** value in a query.</span></span> <span data-ttu-id="a7520-130">Você pode alterar a ordem da resposta usando o `$orderby` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a7520-130">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="a7520-131">$select</span><span class="sxs-lookup"><span data-stu-id="a7520-131">$select</span></span>         |<span data-ttu-id="a7520-132">string</span><span class="sxs-lookup"><span data-stu-id="a7520-132">string</span></span>   |<span data-ttu-id="a7520-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="a7520-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                             |
|<span data-ttu-id="a7520-135">$skip</span><span class="sxs-lookup"><span data-stu-id="a7520-135">$skip</span></span>           |<span data-ttu-id="a7520-136">int</span><span class="sxs-lookup"><span data-stu-id="a7520-136">int</span></span>      |<span data-ttu-id="a7520-137">Ignore os primeiros resultados n, úteis para pajamento.</span><span class="sxs-lookup"><span data-stu-id="a7520-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                     |
|<span data-ttu-id="a7520-138">$top</span><span class="sxs-lookup"><span data-stu-id="a7520-138">$top</span></span>            |<span data-ttu-id="a7520-139">int</span><span class="sxs-lookup"><span data-stu-id="a7520-139">int</span></span>      |<span data-ttu-id="a7520-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="a7520-140">Number of results to be returned.</span></span>                                                                                                                                                |

## <a name="request-headers"></a><span data-ttu-id="a7520-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7520-141">Request headers</span></span>

| <span data-ttu-id="a7520-142">Nome</span><span class="sxs-lookup"><span data-stu-id="a7520-142">Name</span></span>           |<span data-ttu-id="a7520-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7520-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a7520-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7520-144">Authorization</span></span>  | <span data-ttu-id="a7520-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7520-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a7520-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7520-147">Content-Type</span></span>   | <span data-ttu-id="a7520-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7520-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7520-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7520-150">Request body</span></span>

<span data-ttu-id="a7520-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7520-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7520-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7520-152">Response</span></span>

<span data-ttu-id="a7520-153">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos skillProficiency](../resources/skillproficiency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7520-153">If successful, this method returns a `200 OK` response code and a collection of [skillProficiency](../resources/skillproficiency.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a7520-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a7520-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7520-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7520-155">Request</span></span>

<span data-ttu-id="a7520-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7520-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7520-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7520-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_skills"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/skills
```
# <a name="c"></a>[<span data-ttu-id="a7520-158">C#</span><span class="sxs-lookup"><span data-stu-id="a7520-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-skills-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7520-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7520-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-skills-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7520-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7520-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-skills-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7520-161">Java</span><span class="sxs-lookup"><span data-stu-id="a7520-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-skills-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a7520-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7520-162">Response</span></span>

<span data-ttu-id="a7520-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7520-163">The following is an example of the response.</span></span>

> <span data-ttu-id="a7520-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a7520-164">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
      "allowedAudiences": "organization",
      "inference": null,
      "createdDateTime": "2020-07-06T06:34:12.2294868Z",
      "createdBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "source": null,
      "categories": [
        "Professional"
      ],
      "displayName": "API Design",
      "proficiency": "advancedProfessional",
      "webUrl": null,
      "collaborationTags": [
        "ableToMentor"
      ]
    }
  ]
}
```


