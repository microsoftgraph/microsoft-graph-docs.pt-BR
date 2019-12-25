---
title: Substituir timeOffReason
description: Substitua um timeOffReason existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cee6d0392ee56a985da2a9419f3446caf61cbc6a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863640"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="df833-103">Substituir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="df833-103">Replace timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df833-104">Substitua um [timeOffReason](../resources/timeoffreason.md)existente.</span><span class="sxs-lookup"><span data-stu-id="df833-104">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="df833-105">Se o [timeOffReason](../resources/timeoffreason.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="df833-105">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="df833-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df833-106">Permissions</span></span>

<span data-ttu-id="df833-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df833-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df833-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df833-109">Permission type</span></span>      | <span data-ttu-id="df833-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df833-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df833-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df833-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df833-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df833-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="df833-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df833-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df833-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df833-114">Not supported.</span></span>    |
|<span data-ttu-id="df833-115">Application</span><span class="sxs-lookup"><span data-stu-id="df833-115">Application</span></span> | <span data-ttu-id="df833-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="df833-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="df833-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="df833-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="df833-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="df833-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="df833-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="df833-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="df833-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df833-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="df833-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df833-121">Request headers</span></span>

| <span data-ttu-id="df833-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df833-122">Header</span></span>       | <span data-ttu-id="df833-123">Valor</span><span class="sxs-lookup"><span data-stu-id="df833-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df833-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="df833-124">Authorization</span></span>  | <span data-ttu-id="df833-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df833-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df833-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df833-127">Content-Type</span></span>  | <span data-ttu-id="df833-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df833-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df833-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df833-130">Request body</span></span>

<span data-ttu-id="df833-131">No corpo da solicitação, forneça uma representação JSON de um objeto [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="df833-131">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df833-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="df833-132">Response</span></span>

<span data-ttu-id="df833-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df833-133">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df833-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df833-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="df833-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df833-135">Request</span></span>

<span data-ttu-id="df833-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df833-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="df833-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="df833-137">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="df833-138">C#</span><span class="sxs-lookup"><span data-stu-id="df833-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df833-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df833-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df833-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df833-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="df833-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="df833-141">Response</span></span>

<span data-ttu-id="df833-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df833-142">The following is an example of the response.</span></span> 

><span data-ttu-id="df833-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df833-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
