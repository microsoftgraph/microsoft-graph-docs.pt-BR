---
title: Criar timeOffReason
description: Criar um novo timeOffReason.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1e4867fb06326b4a8f84cc711fd2d1a1e5219618
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051211"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="92116-103">Criar timeOffReason</span><span class="sxs-lookup"><span data-stu-id="92116-103">Create timeOffReason</span></span>

<span data-ttu-id="92116-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92116-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92116-105">Criar um novo [timeOffReason](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="92116-105">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="92116-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92116-106">Permissions</span></span>

<span data-ttu-id="92116-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92116-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92116-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92116-109">Permission type</span></span>      | <span data-ttu-id="92116-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92116-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92116-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92116-111">Delegated (work or school account)</span></span> | <span data-ttu-id="92116-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92116-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="92116-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92116-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92116-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92116-114">Not supported.</span></span>    |
|<span data-ttu-id="92116-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92116-115">Application</span></span> | <span data-ttu-id="92116-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92116-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="92116-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="92116-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="92116-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="92116-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="92116-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92116-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="92116-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92116-120">Request headers</span></span>

| <span data-ttu-id="92116-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92116-121">Header</span></span>       | <span data-ttu-id="92116-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92116-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92116-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92116-123">Authorization</span></span>  | <span data-ttu-id="92116-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92116-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="92116-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92116-126">Content-Type</span></span>  | <span data-ttu-id="92116-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92116-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="92116-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="92116-129">Response</span></span>

<span data-ttu-id="92116-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92116-130">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92116-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92116-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="92116-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92116-132">Request</span></span>

<span data-ttu-id="92116-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92116-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="92116-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="92116-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-timeoffreasons"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons
Content-type: application/json

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="92116-135">C#</span><span class="sxs-lookup"><span data-stu-id="92116-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92116-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92116-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92116-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92116-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92116-138">Java</span><span class="sxs-lookup"><span data-stu-id="92116-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-timeoffreasons-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="92116-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="92116-139">Response</span></span>

<span data-ttu-id="92116-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92116-140">The following is an example of the response.</span></span> 

><span data-ttu-id="92116-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92116-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

