---
title: Criar timeOffReason
description: Criar um novo timeOffReason.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0f12d104db2748d5277565326b54d083bea8cdee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457580"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="5454e-103">Criar timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5454e-103">Create timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5454e-104">Criar um novo [timeOffReason](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="5454e-104">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5454e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5454e-105">Permissions</span></span>

<span data-ttu-id="5454e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5454e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5454e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5454e-108">Permission type</span></span>      | <span data-ttu-id="5454e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5454e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5454e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5454e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5454e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5454e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5454e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5454e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5454e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5454e-113">Not supported.</span></span>    |
|<span data-ttu-id="5454e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5454e-114">Application</span></span> | <span data-ttu-id="5454e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5454e-115">Not supported.</span></span> |

> <span data-ttu-id="5454e-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="5454e-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5454e-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="5454e-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5454e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5454e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="5454e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5454e-119">Request headers</span></span>

| <span data-ttu-id="5454e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5454e-120">Header</span></span>       | <span data-ttu-id="5454e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5454e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5454e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5454e-122">Authorization</span></span>  | <span data-ttu-id="5454e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5454e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5454e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5454e-125">Content-Type</span></span>  | <span data-ttu-id="5454e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5454e-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="5454e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5454e-127">Response</span></span>

<span data-ttu-id="5454e-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5454e-128">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5454e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5454e-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5454e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5454e-130">Request</span></span>

<span data-ttu-id="5454e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5454e-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5454e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5454e-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5454e-133">C#</span><span class="sxs-lookup"><span data-stu-id="5454e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5454e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="5454e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5454e-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5454e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5454e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5454e-136">Response</span></span>

<span data-ttu-id="5454e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5454e-137">The following is an example of the response.</span></span> 

><span data-ttu-id="5454e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5454e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
