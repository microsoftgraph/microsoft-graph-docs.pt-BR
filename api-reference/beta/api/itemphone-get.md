---
title: Obter itemPhone
description: Recupere as propriedades e as relações de um objeto itemPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0dd5f2941fe01fd15000c90dec6df2410b388c62
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954524"
---
# <a name="get-itemphonenumber"></a><span data-ttu-id="20924-103">Obter itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="20924-103">Get itemPhoneNumber</span></span>

<span data-ttu-id="20924-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20924-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20924-105">Recupere as propriedades e as relações de um [objeto itemPhone](../resources/itemphone.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="20924-105">Retrieve the properties and relationships of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="20924-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20924-106">Permissions</span></span>

<span data-ttu-id="20924-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20924-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20924-109">Permission type</span></span>                        | <span data-ttu-id="20924-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20924-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="20924-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20924-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="20924-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20924-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="20924-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20924-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20924-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20924-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="20924-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20924-115">Application</span></span>                            | <span data-ttu-id="20924-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20924-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="20924-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20924-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/phones/{id}
GET /users/{userId}/profile/phones/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20924-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20924-118">Optional query parameters</span></span>

<span data-ttu-id="20924-119">Este método dá suporte `$select` ao parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="20924-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="20924-120">Especifique uma lista de propriedades para incluir na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="20924-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="20924-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="20924-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20924-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20924-122">Request headers</span></span>
|<span data-ttu-id="20924-123">Nome</span><span class="sxs-lookup"><span data-stu-id="20924-123">Name</span></span>|<span data-ttu-id="20924-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="20924-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20924-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="20924-125">Authorization</span></span>|<span data-ttu-id="20924-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20924-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20924-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20924-128">Request body</span></span>
<span data-ttu-id="20924-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20924-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20924-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="20924-130">Response</span></span>

<span data-ttu-id="20924-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [itemPhone](../resources/itemphone.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20924-131">If successful, this method returns a `200 OK` response code and an [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20924-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20924-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20924-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20924-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="20924-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="20924-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemphone_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/phones/{id}
```
# <a name="c"></a>[<span data-ttu-id="20924-135">C#</span><span class="sxs-lookup"><span data-stu-id="20924-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemphone-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20924-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20924-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemphone-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20924-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20924-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemphone-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20924-138">Java</span><span class="sxs-lookup"><span data-stu-id="20924-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-itemphone-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="20924-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="20924-139">Response</span></span>
<span data-ttu-id="20924-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="20924-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


