---
title: Substituir timeOffReason
description: Substitua um timeOffReason existente.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ee87ff78baa7ae9b1fd5cf4428b99a167c960fc5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050231"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="7e7e5-103">Substituir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="7e7e5-103">Replace timeOffReason</span></span>

<span data-ttu-id="7e7e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e7e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e7e5-105">Substitua um [timeOffReason](../resources/timeoffreason.md)existente.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-105">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="7e7e5-106">Se o [timeOffReason especificado](../resources/timeoffreason.md) não existir, este método retornará `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="7e7e5-106">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e7e5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e7e5-107">Permissions</span></span>

<span data-ttu-id="7e7e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e7e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e7e5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e7e5-110">Permission type</span></span>      | <span data-ttu-id="7e7e5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e7e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e7e5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e7e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7e7e5-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e7e5-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e7e5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e7e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e7e5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-115">Not supported.</span></span>    |
|<span data-ttu-id="7e7e5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e7e5-116">Application</span></span> | <span data-ttu-id="7e7e5-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e7e5-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="7e7e5-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7e7e5-119">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7e7e5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e7e5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="7e7e5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e7e5-121">Request headers</span></span>

| <span data-ttu-id="7e7e5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e7e5-122">Header</span></span>       | <span data-ttu-id="7e7e5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7e7e5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e7e5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e7e5-124">Authorization</span></span>  | <span data-ttu-id="7e7e5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7e7e5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e7e5-127">Content-Type</span></span>  | <span data-ttu-id="7e7e5-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e7e5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e7e5-130">Request body</span></span>

<span data-ttu-id="7e7e5-131">No corpo da solicitação, fornece uma representação JSON de um [objeto timeOffReason.](../resources/timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="7e7e5-131">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7e7e5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e7e5-132">Response</span></span>

<span data-ttu-id="7e7e5-133">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-133">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e7e5-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e7e5-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e7e5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e7e5-135">Request</span></span>

<span data-ttu-id="7e7e5-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7e7e5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e7e5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-put"
}-->
```http
PUT https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="7e7e5-138">C#</span><span class="sxs-lookup"><span data-stu-id="7e7e5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e7e5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e7e5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e7e5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e7e5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e7e5-141">Java</span><span class="sxs-lookup"><span data-stu-id="7e7e5-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="7e7e5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e7e5-142">Response</span></span>

<span data-ttu-id="7e7e5-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-143">The following is an example of the response.</span></span> 

><span data-ttu-id="7e7e5-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e7e5-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

