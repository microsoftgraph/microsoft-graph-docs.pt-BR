---
title: Obter presença
description: Obtenha as informações de presença de um usuário.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: cdb211e85f3e995801bb7583a8aa043cb2d6a133
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913083"
---
# <a name="get-presence"></a><span data-ttu-id="e1eea-103">Obter presença</span><span class="sxs-lookup"><span data-stu-id="e1eea-103">Get presence</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1eea-104">Obtenha as informações de [presença](../resources/presence.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e1eea-104">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1eea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1eea-105">Permissions</span></span>
<span data-ttu-id="e1eea-106">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="e1eea-106">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="e1eea-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1eea-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1eea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1eea-108">Permission type</span></span> | <span data-ttu-id="e1eea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1eea-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="e1eea-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1eea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1eea-111">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1eea-111">Presence.Read, Presence.Read.All</span></span>                         |
| <span data-ttu-id="e1eea-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1eea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1eea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1eea-113">Not Supported.</span></span>                         |
| <span data-ttu-id="e1eea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1eea-114">Application</span></span>                            | <span data-ttu-id="e1eea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1eea-115">Not Supported.</span></span>                                  |

## <a name="http-requests"></a><span data-ttu-id="e1eea-116">Solicitações HTTP</span><span class="sxs-lookup"><span data-stu-id="e1eea-116">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
```

## <a name="request-headers"></a><span data-ttu-id="e1eea-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1eea-117">Request Headers</span></span>
| <span data-ttu-id="e1eea-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e1eea-118">Name</span></span>          | <span data-ttu-id="e1eea-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1eea-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e1eea-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1eea-120">Authorization</span></span> | <span data-ttu-id="e1eea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1eea-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e1eea-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1eea-123">Request body</span></span>

<span data-ttu-id="e1eea-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1eea-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1eea-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1eea-125">Response</span></span>
<span data-ttu-id="e1eea-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Presence](../resources/presence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1eea-126">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1eea-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e1eea-127">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="e1eea-128">Exemplo 1: obter suas próprias informações de presença</span><span class="sxs-lookup"><span data-stu-id="e1eea-128">Example 1: Get your own presence information</span></span>

<span data-ttu-id="e1eea-129">O exemplo a seguir mostra como obter suas próprias informações de presença.</span><span class="sxs-lookup"><span data-stu-id="e1eea-129">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="e1eea-130">Esta operação requer a permissão Presence. Read.</span><span class="sxs-lookup"><span data-stu-id="e1eea-130">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="e1eea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1eea-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e1eea-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1eea-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1eea-133">C#</span><span class="sxs-lookup"><span data-stu-id="e1eea-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1eea-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1eea-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1eea-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1eea-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e1eea-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1eea-136">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="e1eea-137">Exemplo 2: obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="e1eea-137">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="e1eea-138">O exemplo a seguir mostra como obter as informações de presença de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="e1eea-138">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="e1eea-139">Esta operação requer a permissão Presence. Read. All.</span><span class="sxs-lookup"><span data-stu-id="e1eea-139">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="e1eea-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1eea-140">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e1eea-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1eea-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1eea-142">C#</span><span class="sxs-lookup"><span data-stu-id="e1eea-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1eea-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1eea-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1eea-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1eea-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e1eea-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1eea-145">Response</span></span>

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
