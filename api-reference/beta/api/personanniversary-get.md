---
title: Obter personAnniversary
description: Recupere as propriedades e os relacionamentos de um objeto personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 63d04f78789f1ef7ad35cf4b03636bfc30cecba7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968453"
---
# <a name="get-personanniversary"></a><span data-ttu-id="46a94-103">Obter personAnniversary</span><span class="sxs-lookup"><span data-stu-id="46a94-103">Get personAnniversary</span></span>

<span data-ttu-id="46a94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46a94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46a94-105">Recupere as propriedades e os relacionamentos de um objeto [personAnniversary](../resources/personanniversary.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="46a94-105">Retrieve the properties and relationships of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="46a94-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46a94-106">Permissions</span></span>

<span data-ttu-id="46a94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46a94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46a94-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46a94-109">Permission type</span></span>                        | <span data-ttu-id="46a94-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46a94-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="46a94-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46a94-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="46a94-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="46a94-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="46a94-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46a94-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46a94-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="46a94-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="46a94-115">Application</span><span class="sxs-lookup"><span data-stu-id="46a94-115">Application</span></span>                            | <span data-ttu-id="46a94-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="46a94-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="46a94-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46a94-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/anniversaries/{id}
GET /users/{id | userPrincipalName}/profile/anniversaries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46a94-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46a94-118">Optional query parameters</span></span>

<span data-ttu-id="46a94-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="46a94-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="46a94-120">Especifique uma lista de propriedades a serem incluídas na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="46a94-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="46a94-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="46a94-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46a94-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46a94-122">Request headers</span></span>

| <span data-ttu-id="46a94-123">Nome</span><span class="sxs-lookup"><span data-stu-id="46a94-123">Name</span></span>           |<span data-ttu-id="46a94-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="46a94-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="46a94-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="46a94-125">Authorization</span></span>  | <span data-ttu-id="46a94-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46a94-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="46a94-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46a94-128">Request body</span></span>

<span data-ttu-id="46a94-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46a94-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46a94-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="46a94-130">Response</span></span>

<span data-ttu-id="46a94-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [personAnniversary](../resources/personanniversary.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46a94-131">If successful, this method returns a `200 OK` response code and the requested [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46a94-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46a94-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46a94-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46a94-133">Request</span></span>

<span data-ttu-id="46a94-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46a94-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46a94-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="46a94-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personanniversary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
```
# <a name="c"></a>[<span data-ttu-id="46a94-136">C#</span><span class="sxs-lookup"><span data-stu-id="46a94-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46a94-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46a94-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46a94-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46a94-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46a94-139">Java</span><span class="sxs-lookup"><span data-stu-id="46a94-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-personanniversary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="46a94-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="46a94-140">Response</span></span>

<span data-ttu-id="46a94-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46a94-141">The following is an example of the response.</span></span>

> <span data-ttu-id="46a94-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46a94-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
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
  "type": "birthday",
  "date": "Date"
}
```


