---
title: Obter presença
description: Obtenha as informações de presença de um usuário.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: f993c68b9858523a621f23bc182f6f6113c50366
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863332"
---
# <a name="get-presence"></a><span data-ttu-id="4beb5-103">Obter presença</span><span class="sxs-lookup"><span data-stu-id="4beb5-103">Get presence</span></span>

<span data-ttu-id="4beb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4beb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4beb5-105">Obtenha as informações de [presença](../resources/presence.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4beb5-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="4beb5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4beb5-106">Permissions</span></span>
<span data-ttu-id="4beb5-107">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="4beb5-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="4beb5-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4beb5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4beb5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4beb5-109">Permission type</span></span> | <span data-ttu-id="4beb5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4beb5-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="4beb5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4beb5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4beb5-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="4beb5-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="4beb5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4beb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4beb5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4beb5-114">Not Supported.</span></span>                        |
| <span data-ttu-id="4beb5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4beb5-115">Application</span></span>                            | <span data-ttu-id="4beb5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4beb5-116">Not Supported.</span></span>                        |

## <a name="http-requests"></a><span data-ttu-id="4beb5-117">Solicitações HTTP</span><span class="sxs-lookup"><span data-stu-id="4beb5-117">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="4beb5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4beb5-118">Request Headers</span></span>
| <span data-ttu-id="4beb5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4beb5-119">Name</span></span>          | <span data-ttu-id="4beb5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4beb5-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4beb5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4beb5-121">Authorization</span></span> | <span data-ttu-id="4beb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4beb5-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4beb5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4beb5-124">Request body</span></span>

<span data-ttu-id="4beb5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4beb5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4beb5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4beb5-126">Response</span></span>
<span data-ttu-id="4beb5-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Presence](../resources/presence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4beb5-127">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4beb5-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4beb5-128">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="4beb5-129">Exemplo 1: obter suas próprias informações de presença</span><span class="sxs-lookup"><span data-stu-id="4beb5-129">Example 1: Get your own presence information</span></span>

<span data-ttu-id="4beb5-130">O exemplo a seguir mostra como obter suas próprias informações de presença.</span><span class="sxs-lookup"><span data-stu-id="4beb5-130">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="4beb5-131">Esta operação requer a permissão Presence. Read.</span><span class="sxs-lookup"><span data-stu-id="4beb5-131">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4beb5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4beb5-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4beb5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4beb5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="c"></a>[<span data-ttu-id="4beb5-134">C#</span><span class="sxs-lookup"><span data-stu-id="4beb5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4beb5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4beb5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4beb5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4beb5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4beb5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4beb5-137">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="4beb5-138">Exemplo 2: obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="4beb5-138">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="4beb5-139">O exemplo a seguir mostra como obter as informações de presença de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="4beb5-139">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="4beb5-140">Esta operação requer a permissão Presence. Read. All.</span><span class="sxs-lookup"><span data-stu-id="4beb5-140">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4beb5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4beb5-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4beb5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4beb5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="4beb5-143">C#</span><span class="sxs-lookup"><span data-stu-id="4beb5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4beb5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4beb5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4beb5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4beb5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4beb5-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="4beb5-146">Response</span></span>

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

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="4beb5-147">Exemplo 3: obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="4beb5-147">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="4beb5-148">O exemplo a seguir mostra como obter as informações de presença de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="4beb5-148">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="4beb5-149">Esta operação requer a permissão Presence. Read. All.</span><span class="sxs-lookup"><span data-stu-id="4beb5-149">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4beb5-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4beb5-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4beb5-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="4beb5-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```
# <a name="c"></a>[<span data-ttu-id="4beb5-152">C#</span><span class="sxs-lookup"><span data-stu-id="4beb5-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4beb5-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4beb5-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4beb5-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4beb5-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4beb5-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="4beb5-155">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
            "availability": "Away",
            "activity": "BeRightBack"
        }
    ]
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
