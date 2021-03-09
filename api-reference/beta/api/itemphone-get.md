---
title: Obter itemPhone
description: Recupere as propriedades e as relações de um objeto itemPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0622fef3be1d34c6bac46601eb42af2d2420d2c6
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577419"
---
# <a name="get-itemphonenumber"></a><span data-ttu-id="5fdd8-103">Obter itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="5fdd8-103">Get itemPhoneNumber</span></span>

<span data-ttu-id="5fdd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fdd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fdd8-105">Recupere as propriedades e as relações de um [objeto itemPhone](../resources/itemphone.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="5fdd8-105">Retrieve the properties and relationships of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5fdd8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fdd8-106">Permissions</span></span>

<span data-ttu-id="5fdd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fdd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5fdd8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fdd8-109">Permission type</span></span>                        | <span data-ttu-id="5fdd8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fdd8-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="5fdd8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fdd8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5fdd8-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fdd8-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5fdd8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fdd8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fdd8-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fdd8-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5fdd8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fdd8-115">Application</span></span>                            | <span data-ttu-id="5fdd8-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fdd8-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="5fdd8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fdd8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/phones/{id}
GET /users/{userId}/profile/phones/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fdd8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5fdd8-118">Optional query parameters</span></span>

<span data-ttu-id="5fdd8-119">Este método dá suporte `$select` ao parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="5fdd8-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="5fdd8-120">Especifique uma lista de propriedades para incluir na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="5fdd8-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="5fdd8-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="5fdd8-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fdd8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fdd8-122">Request headers</span></span>
|<span data-ttu-id="5fdd8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5fdd8-123">Name</span></span>|<span data-ttu-id="5fdd8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fdd8-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5fdd8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fdd8-125">Authorization</span></span>|<span data-ttu-id="5fdd8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fdd8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fdd8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fdd8-128">Request body</span></span>
<span data-ttu-id="5fdd8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5fdd8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fdd8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fdd8-130">Response</span></span>

<span data-ttu-id="5fdd8-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [itemPhone](../resources/itemphone.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fdd8-131">If successful, this method returns a `200 OK` response code and an [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5fdd8-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5fdd8-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5fdd8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fdd8-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="5fdd8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fdd8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemphone"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/phones/{id}
```
# <a name="c"></a>[<span data-ttu-id="5fdd8-135">C#</span><span class="sxs-lookup"><span data-stu-id="5fdd8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fdd8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fdd8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fdd8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fdd8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5fdd8-138">Java</span><span class="sxs-lookup"><span data-stu-id="5fdd8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-itemphone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5fdd8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fdd8-139">Response</span></span>
<span data-ttu-id="5fdd8-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5fdd8-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
  "displayName": "Car Phone",
  "type": "other",
  "number": "+7 499 342 22 13"
}
```


