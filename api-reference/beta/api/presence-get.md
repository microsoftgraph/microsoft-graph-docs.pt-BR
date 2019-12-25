---
title: Obter presença
description: Obtenha as informações de presença de um usuário.
author: VinodRavichandran
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: fa059a7399762444d73a13305b5bec722830a1c0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867683"
---
# <a name="get-presence"></a><span data-ttu-id="e13f0-103">Obter presença</span><span class="sxs-lookup"><span data-stu-id="e13f0-103">Get presence</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e13f0-104">Obtenha as informações de [presença](../resources/presence.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e13f0-104">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="e13f0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e13f0-105">Permissions</span></span>
<span data-ttu-id="e13f0-106">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="e13f0-106">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="e13f0-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e13f0-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e13f0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e13f0-108">Permission type</span></span> | <span data-ttu-id="e13f0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e13f0-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="e13f0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e13f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e13f0-111">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="e13f0-111">Presence.Read, Presence.Read.All</span></span>                         |
| <span data-ttu-id="e13f0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e13f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e13f0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e13f0-113">Not Supported.</span></span>                         |
| <span data-ttu-id="e13f0-114">Application</span><span class="sxs-lookup"><span data-stu-id="e13f0-114">Application</span></span>                            | <span data-ttu-id="e13f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e13f0-115">Not Supported.</span></span>                                  |

## <a name="http-requests"></a><span data-ttu-id="e13f0-116">Solicitações HTTP</span><span class="sxs-lookup"><span data-stu-id="e13f0-116">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
```

## <a name="request-headers"></a><span data-ttu-id="e13f0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e13f0-117">Request Headers</span></span>
| <span data-ttu-id="e13f0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e13f0-118">Name</span></span>          | <span data-ttu-id="e13f0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e13f0-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e13f0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e13f0-120">Authorization</span></span> | <span data-ttu-id="e13f0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e13f0-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e13f0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e13f0-123">Request body</span></span>

<span data-ttu-id="e13f0-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e13f0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e13f0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13f0-125">Response</span></span>
<span data-ttu-id="e13f0-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Presence](../resources/presence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e13f0-126">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e13f0-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e13f0-127">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="e13f0-128">Exemplo 1: obter suas próprias informações de presença</span><span class="sxs-lookup"><span data-stu-id="e13f0-128">Example 1: Get your own presence information</span></span>

<span data-ttu-id="e13f0-129">O exemplo a seguir mostra como obter suas próprias informações de presença.</span><span class="sxs-lookup"><span data-stu-id="e13f0-129">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="e13f0-130">Esta operação requer a permissão Presence. Read.</span><span class="sxs-lookup"><span data-stu-id="e13f0-130">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="e13f0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e13f0-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e13f0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e13f0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e13f0-133">C#</span><span class="sxs-lookup"><span data-stu-id="e13f0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e13f0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e13f0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e13f0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e13f0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e13f0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13f0-136">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="e13f0-137">Exemplo 2: obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="e13f0-137">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="e13f0-138">O exemplo a seguir mostra como obter as informações de presença de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e13f0-138">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="e13f0-139">Esta operação requer a permissão Presence. Read. All.</span><span class="sxs-lookup"><span data-stu-id="e13f0-139">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="e13f0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e13f0-140">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e13f0-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e13f0-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e13f0-142">C#</span><span class="sxs-lookup"><span data-stu-id="e13f0-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e13f0-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e13f0-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e13f0-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e13f0-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e13f0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13f0-145">Response</span></span>

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
