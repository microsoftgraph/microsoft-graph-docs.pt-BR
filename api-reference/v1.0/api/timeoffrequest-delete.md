---
title: Excluir timeOffRequest
description: Excluir um objeto timeOffRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 89ec693d533e39075bde89992eaba55ebd8656e4
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215882"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="e5807-103">Excluir timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="e5807-103">Delete timeOffRequest</span></span>

<span data-ttu-id="e5807-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5807-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5807-105">Excluir um objeto [timeOffRequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="e5807-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5807-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5807-106">Permissions</span></span>

<span data-ttu-id="e5807-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5807-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5807-109">Permission type</span></span>                        | <span data-ttu-id="e5807-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5807-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="e5807-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5807-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e5807-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e5807-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5807-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5807-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5807-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5807-114">Not supported.</span></span>    |
|<span data-ttu-id="e5807-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5807-115">Application</span></span> | <span data-ttu-id="e5807-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5807-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="e5807-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="e5807-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e5807-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="e5807-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e5807-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5807-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="e5807-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5807-120">Request headers</span></span>

| <span data-ttu-id="e5807-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e5807-121">Name</span></span>          | <span data-ttu-id="e5807-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5807-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e5807-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5807-123">Authorization</span></span> | <span data-ttu-id="e5807-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5807-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5807-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5807-126">Request body</span></span>

<span data-ttu-id="e5807-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5807-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5807-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5807-128">Response</span></span>

<span data-ttu-id="e5807-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5807-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5807-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e5807-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5807-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5807-132">Request</span></span>

<span data-ttu-id="e5807-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5807-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5807-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5807-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="e5807-135">C#</span><span class="sxs-lookup"><span data-stu-id="e5807-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5807-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5807-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5807-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5807-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5807-138">Java</span><span class="sxs-lookup"><span data-stu-id="e5807-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-timeoffrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="e5807-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5807-139">Response</span></span>

<span data-ttu-id="e5807-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5807-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
