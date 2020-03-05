---
title: Substituir timeOffReason
description: Substitua um timeOffReason existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6e28a22e7a49d35d7ae0f06affb0652ad37ce538
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452278"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="3c87a-103">Substituir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="3c87a-103">Replace timeOffReason</span></span>

<span data-ttu-id="3c87a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3c87a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c87a-105">Substitua um [timeOffReason](../resources/timeoffreason.md)existente.</span><span class="sxs-lookup"><span data-stu-id="3c87a-105">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="3c87a-106">Se o [timeOffReason](../resources/timeoffreason.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="3c87a-106">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c87a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c87a-107">Permissions</span></span>

<span data-ttu-id="3c87a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c87a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c87a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c87a-110">Permission type</span></span>      | <span data-ttu-id="3c87a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c87a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c87a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c87a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c87a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c87a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c87a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c87a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c87a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c87a-115">Not supported.</span></span>    |
|<span data-ttu-id="3c87a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c87a-116">Application</span></span> | <span data-ttu-id="3c87a-117">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="3c87a-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="3c87a-118">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="3c87a-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="3c87a-119">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="3c87a-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3c87a-120">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="3c87a-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c87a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c87a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="3c87a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c87a-122">Request headers</span></span>

| <span data-ttu-id="3c87a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c87a-123">Header</span></span>       | <span data-ttu-id="3c87a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3c87a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c87a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c87a-125">Authorization</span></span>  | <span data-ttu-id="3c87a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c87a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3c87a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c87a-128">Content-Type</span></span>  | <span data-ttu-id="3c87a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c87a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c87a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c87a-131">Request body</span></span>

<span data-ttu-id="3c87a-132">No corpo da solicitação, forneça uma representação JSON de um objeto [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="3c87a-132">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3c87a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c87a-133">Response</span></span>

<span data-ttu-id="3c87a-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c87a-134">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c87a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c87a-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3c87a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c87a-136">Request</span></span>

<span data-ttu-id="3c87a-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c87a-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c87a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c87a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="3c87a-139">C#</span><span class="sxs-lookup"><span data-stu-id="3c87a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c87a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c87a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c87a-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c87a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c87a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c87a-142">Response</span></span>

<span data-ttu-id="3c87a-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c87a-143">The following is an example of the response.</span></span> 

><span data-ttu-id="3c87a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c87a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
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
      "displayName": "Alex Wilbur"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
