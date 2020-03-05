---
title: Obter timeOffReason
description: Obtenha um timeOffReason por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cb9c436537e233c14e4f9d9eb1a2c6cb01cc6fe2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452285"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="73f5d-103">Obter timeOffReason</span><span class="sxs-lookup"><span data-stu-id="73f5d-103">Get timeOffReason</span></span>

<span data-ttu-id="73f5d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="73f5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73f5d-105">Recupere as propriedades e os relacionamentos de um objeto [timeOffReason](../resources/timeoffreason.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="73f5d-105">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="73f5d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="73f5d-106">Permissions</span></span>

<span data-ttu-id="73f5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73f5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73f5d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73f5d-109">Permission type</span></span>      | <span data-ttu-id="73f5d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73f5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73f5d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73f5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73f5d-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73f5d-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="73f5d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73f5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73f5d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73f5d-114">Not supported.</span></span>    |
|<span data-ttu-id="73f5d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73f5d-115">Application</span></span> | <span data-ttu-id="73f5d-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="73f5d-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="73f5d-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="73f5d-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="73f5d-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="73f5d-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="73f5d-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="73f5d-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="73f5d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73f5d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="73f5d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73f5d-121">Request headers</span></span>

| <span data-ttu-id="73f5d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73f5d-122">Header</span></span>       | <span data-ttu-id="73f5d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="73f5d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73f5d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="73f5d-124">Authorization</span></span>  | <span data-ttu-id="73f5d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73f5d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73f5d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73f5d-127">Request body</span></span>
<span data-ttu-id="73f5d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73f5d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73f5d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="73f5d-129">Response</span></span>

<span data-ttu-id="73f5d-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73f5d-130">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73f5d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73f5d-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="73f5d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73f5d-132">Request</span></span>

<span data-ttu-id="73f5d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73f5d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73f5d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="73f5d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="73f5d-135">C#</span><span class="sxs-lookup"><span data-stu-id="73f5d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73f5d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73f5d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73f5d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73f5d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73f5d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="73f5d-138">Response</span></span>

<span data-ttu-id="73f5d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73f5d-139">The following is an example of the response.</span></span> 

><span data-ttu-id="73f5d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73f5d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Get a timeOffReason by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
