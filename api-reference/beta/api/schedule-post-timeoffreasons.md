---
title: Criar timeOffReason
description: Criar um novo timeOffReason.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35299b61e6a26710453a825442a0c136c33d3ba2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974949"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="1c92e-103">Criar timeOffReason</span><span class="sxs-lookup"><span data-stu-id="1c92e-103">Create timeOffReason</span></span>

<span data-ttu-id="1c92e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c92e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c92e-105">Criar um novo [timeOffReason](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="1c92e-105">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c92e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c92e-106">Permissions</span></span>

<span data-ttu-id="1c92e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c92e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c92e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c92e-109">Permission type</span></span>      | <span data-ttu-id="1c92e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c92e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c92e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c92e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c92e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c92e-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1c92e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c92e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c92e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c92e-114">Not supported.</span></span>    |
|<span data-ttu-id="1c92e-115">Application</span><span class="sxs-lookup"><span data-stu-id="1c92e-115">Application</span></span> | <span data-ttu-id="1c92e-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="1c92e-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="1c92e-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="1c92e-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="1c92e-118">**Observação** : esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1c92e-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="1c92e-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1c92e-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1c92e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c92e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="1c92e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c92e-121">Request headers</span></span>

| <span data-ttu-id="1c92e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c92e-122">Header</span></span>       | <span data-ttu-id="1c92e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1c92e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c92e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c92e-124">Authorization</span></span>  | <span data-ttu-id="1c92e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c92e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1c92e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c92e-127">Content-Type</span></span>  | <span data-ttu-id="1c92e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c92e-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="1c92e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c92e-130">Response</span></span>

<span data-ttu-id="1c92e-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c92e-131">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c92e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c92e-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1c92e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c92e-133">Request</span></span>

<span data-ttu-id="1c92e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c92e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c92e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c92e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-timeoffreasons"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
Content-type: application/json

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="1c92e-136">C#</span><span class="sxs-lookup"><span data-stu-id="1c92e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c92e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c92e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c92e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c92e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c92e-139">Java</span><span class="sxs-lookup"><span data-stu-id="1c92e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-timeoffreasons-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c92e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c92e-140">Response</span></span>

<span data-ttu-id="1c92e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c92e-141">The following is an example of the response.</span></span> 

><span data-ttu-id="1c92e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c92e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


