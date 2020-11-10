---
title: Obter skillProficiency
description: Recupere as propriedades e os relacionamentos de um objeto skillproficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b7a4039240a91db30ceb0a3c6f2f13817ed26f67
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973143"
---
# <a name="get-skillproficiency"></a><span data-ttu-id="6d8c1-103">Obter skillProficiency</span><span class="sxs-lookup"><span data-stu-id="6d8c1-103">Get skillProficiency</span></span>

<span data-ttu-id="6d8c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d8c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d8c1-105">Recupere as propriedades e os relacionamentos de um objeto [skillproficiency](../resources/skillproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-105">Retrieve the properties and relationships of a [skillproficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d8c1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d8c1-106">Permissions</span></span>

<span data-ttu-id="6d8c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d8c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d8c1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d8c1-109">Permission type</span></span>                        | <span data-ttu-id="6d8c1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d8c1-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="6d8c1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d8c1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d8c1-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6d8c1-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6d8c1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d8c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d8c1-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6d8c1-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6d8c1-115">Application</span><span class="sxs-lookup"><span data-stu-id="6d8c1-115">Application</span></span>                            | <span data-ttu-id="6d8c1-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6d8c1-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="6d8c1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d8c1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills/{id}
GET /users/{id | userPrincipalName}/profile/skills/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d8c1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d8c1-118">Optional query parameters</span></span>

<span data-ttu-id="6d8c1-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="6d8c1-120">Especifique uma lista de propriedades a serem incluídas na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="6d8c1-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d8c1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d8c1-122">Request headers</span></span>

| <span data-ttu-id="6d8c1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6d8c1-123">Name</span></span>           | <span data-ttu-id="6d8c1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d8c1-124">Description</span></span>                  |
|:---------------|:-----------------------------|
| <span data-ttu-id="6d8c1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d8c1-125">Authorization</span></span>  | <span data-ttu-id="6d8c1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-p103">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="6d8c1-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d8c1-128">Content-Type</span></span>   | <span data-ttu-id="6d8c1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-p104">application/json. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="6d8c1-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d8c1-131">Request body</span></span>

<span data-ttu-id="6d8c1-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d8c1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d8c1-133">Response</span></span>

<span data-ttu-id="6d8c1-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [skillProficiency](../resources/skillproficiency.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-134">If successful, this method returns a `200 OK` response code and the requested [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d8c1-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6d8c1-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d8c1-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d8c1-136">Request</span></span>

<span data-ttu-id="6d8c1-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d8c1-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d8c1-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_skillproficiency"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/skills/{id}
```
# <a name="c"></a>[<span data-ttu-id="6d8c1-139">C#</span><span class="sxs-lookup"><span data-stu-id="6d8c1-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d8c1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d8c1-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d8c1-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d8c1-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d8c1-142">Java</span><span class="sxs-lookup"><span data-stu-id="6d8c1-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-skillproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d8c1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d8c1-143">Response</span></span>

<span data-ttu-id="6d8c1-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-144">The following is an example of the response.</span></span>

> <span data-ttu-id="6d8c1-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d8c1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```


