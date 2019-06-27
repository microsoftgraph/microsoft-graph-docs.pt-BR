---
title: Obter timeOffReason
description: Obtenha um timeOffReason por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20ee24e4c3fb5c859c35a4e9196c1d8c6eb0b79f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270564"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="0f3b8-103">Obter timeOffReason</span><span class="sxs-lookup"><span data-stu-id="0f3b8-103">Get timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f3b8-104">Recupere as propriedades e os relacionamentos de um objeto [timeOffReason](../resources/timeoffreason.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-104">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f3b8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f3b8-105">Permissions</span></span>

<span data-ttu-id="0f3b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f3b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f3b8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f3b8-108">Permission type</span></span>      | <span data-ttu-id="0f3b8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f3b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f3b8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f3b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f3b8-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f3b8-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f3b8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f3b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f3b8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-113">Not supported.</span></span>    |
|<span data-ttu-id="0f3b8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f3b8-114">Application</span></span> | <span data-ttu-id="0f3b8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-115">Not supported.</span></span> |

> <span data-ttu-id="0f3b8-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0f3b8-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0f3b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f3b8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="0f3b8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f3b8-119">Request headers</span></span>

| <span data-ttu-id="0f3b8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f3b8-120">Header</span></span>       | <span data-ttu-id="0f3b8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0f3b8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f3b8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f3b8-122">Authorization</span></span>  | <span data-ttu-id="0f3b8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0f3b8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f3b8-125">Content-Type</span></span>  | <span data-ttu-id="0f3b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f3b8-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f3b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f3b8-127">Request body</span></span>
<span data-ttu-id="0f3b8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f3b8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f3b8-129">Response</span></span>

<span data-ttu-id="0f3b8-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-130">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f3b8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f3b8-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0f3b8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f3b8-132">Request</span></span>

<span data-ttu-id="0f3b8-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="0f3b8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f3b8-134">Response</span></span>

<span data-ttu-id="0f3b8-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-135">The following is an example of the response.</span></span> 

><span data-ttu-id="0f3b8-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f3b8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0f3b8-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0f3b8-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0f3b8-139">C#</span><span class="sxs-lookup"><span data-stu-id="0f3b8-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoffreason-get-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f3b8-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="0f3b8-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoffreason-get-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0f3b8-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0f3b8-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/timeoffreason-get-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
