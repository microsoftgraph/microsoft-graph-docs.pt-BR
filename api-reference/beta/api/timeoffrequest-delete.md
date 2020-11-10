---
title: Excluir timeOffRequest
description: Excluir um objeto timeOffRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f185c8a9e4c3d0b3bb4f8286e0c4f7252e13692e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981340"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="42450-103">Excluir timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="42450-103">Delete timeOffRequest</span></span>

<span data-ttu-id="42450-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42450-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42450-105">Excluir um objeto [timeOffRequest](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="42450-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42450-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42450-106">Permissions</span></span>

<span data-ttu-id="42450-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42450-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42450-109">Permission type</span></span>                        | <span data-ttu-id="42450-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42450-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="42450-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42450-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42450-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42450-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="42450-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42450-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42450-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42450-114">Not supported.</span></span> |
|<span data-ttu-id="42450-115">Application</span><span class="sxs-lookup"><span data-stu-id="42450-115">Application</span></span> | <span data-ttu-id="42450-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="42450-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="42450-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="42450-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="42450-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42450-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="42450-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42450-119">Request headers</span></span>

| <span data-ttu-id="42450-120">Nome</span><span class="sxs-lookup"><span data-stu-id="42450-120">Name</span></span>          | <span data-ttu-id="42450-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="42450-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="42450-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42450-122">Authorization</span></span> | <span data-ttu-id="42450-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42450-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42450-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42450-125">Request body</span></span>

<span data-ttu-id="42450-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42450-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42450-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="42450-127">Response</span></span>

<span data-ttu-id="42450-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42450-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42450-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42450-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42450-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42450-131">Request</span></span>

<span data-ttu-id="42450-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42450-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42450-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="42450-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="42450-134">C#</span><span class="sxs-lookup"><span data-stu-id="42450-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42450-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42450-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42450-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42450-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42450-137">Java</span><span class="sxs-lookup"><span data-stu-id="42450-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-timeoffrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42450-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="42450-138">Response</span></span>

<span data-ttu-id="42450-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42450-139">The following is an example of the response.</span></span>

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


