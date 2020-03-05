---
title: Obter presença
description: Obtenha as informações de presença de um usuário.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 2e73cfcb18fa11b6d4a66f11e5e5bdc0f4802168
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455443"
---
# <a name="get-presence"></a><span data-ttu-id="4477d-103">Obter presença</span><span class="sxs-lookup"><span data-stu-id="4477d-103">Get presence</span></span>

<span data-ttu-id="4477d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4477d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4477d-105">Obtenha as informações de [presença](../resources/presence.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4477d-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="4477d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4477d-106">Permissions</span></span>
<span data-ttu-id="4477d-107">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="4477d-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="4477d-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4477d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4477d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4477d-109">Permission type</span></span> | <span data-ttu-id="4477d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4477d-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="4477d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4477d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4477d-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="4477d-112">Presence.Read, Presence.Read.All</span></span>                         |
| <span data-ttu-id="4477d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4477d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4477d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4477d-114">Not Supported.</span></span>                         |
| <span data-ttu-id="4477d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4477d-115">Application</span></span>                            | <span data-ttu-id="4477d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4477d-116">Not Supported.</span></span>                                  |

## <a name="http-requests"></a><span data-ttu-id="4477d-117">Solicitações HTTP</span><span class="sxs-lookup"><span data-stu-id="4477d-117">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
```

## <a name="request-headers"></a><span data-ttu-id="4477d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4477d-118">Request Headers</span></span>
| <span data-ttu-id="4477d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4477d-119">Name</span></span>          | <span data-ttu-id="4477d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4477d-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4477d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4477d-121">Authorization</span></span> | <span data-ttu-id="4477d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4477d-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4477d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4477d-124">Request body</span></span>

<span data-ttu-id="4477d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4477d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4477d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4477d-126">Response</span></span>
<span data-ttu-id="4477d-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Presence](../resources/presence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4477d-127">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4477d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4477d-128">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="4477d-129">Exemplo 1: obter suas próprias informações de presença</span><span class="sxs-lookup"><span data-stu-id="4477d-129">Example 1: Get your own presence information</span></span>

<span data-ttu-id="4477d-130">O exemplo a seguir mostra como obter suas próprias informações de presença.</span><span class="sxs-lookup"><span data-stu-id="4477d-130">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="4477d-131">Esta operação requer a permissão Presence. Read.</span><span class="sxs-lookup"><span data-stu-id="4477d-131">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4477d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4477d-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4477d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4477d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="c"></a>[<span data-ttu-id="4477d-134">C#</span><span class="sxs-lookup"><span data-stu-id="4477d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4477d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4477d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4477d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4477d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4477d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4477d-137">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="4477d-138">Exemplo 2: obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="4477d-138">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="4477d-139">O exemplo a seguir mostra como obter as informações de presença de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="4477d-139">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="4477d-140">Esta operação requer a permissão Presence. Read. All.</span><span class="sxs-lookup"><span data-stu-id="4477d-140">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4477d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4477d-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4477d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4477d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="4477d-143">C#</span><span class="sxs-lookup"><span data-stu-id="4477d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4477d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4477d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4477d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4477d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4477d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="4477d-146">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
