---
title: Obter timeOffReason
description: Obtenha um timeOffReason por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 010cc893a3dc4911e40a77a047cdd51d3777d861
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863668"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="4e629-103">Obter timeOffReason</span><span class="sxs-lookup"><span data-stu-id="4e629-103">Get timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e629-104">Recupere as propriedades e os relacionamentos de um objeto [timeOffReason](../resources/timeoffreason.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="4e629-104">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e629-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e629-105">Permissions</span></span>

<span data-ttu-id="4e629-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e629-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e629-108">Permission type</span></span>      | <span data-ttu-id="4e629-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e629-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e629-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e629-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4e629-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e629-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e629-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e629-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e629-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e629-113">Not supported.</span></span>    |
|<span data-ttu-id="4e629-114">Application</span><span class="sxs-lookup"><span data-stu-id="4e629-114">Application</span></span> | <span data-ttu-id="4e629-115">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="4e629-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="4e629-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="4e629-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="4e629-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="4e629-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4e629-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="4e629-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4e629-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e629-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="4e629-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e629-120">Request headers</span></span>

| <span data-ttu-id="4e629-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e629-121">Header</span></span>       | <span data-ttu-id="4e629-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4e629-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e629-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e629-123">Authorization</span></span>  | <span data-ttu-id="4e629-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e629-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e629-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e629-126">Request body</span></span>
<span data-ttu-id="4e629-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e629-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e629-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e629-128">Response</span></span>

<span data-ttu-id="4e629-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e629-129">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e629-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e629-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4e629-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e629-131">Request</span></span>

<span data-ttu-id="4e629-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e629-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4e629-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e629-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4e629-134">C#</span><span class="sxs-lookup"><span data-stu-id="4e629-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e629-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e629-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4e629-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e629-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4e629-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e629-137">Response</span></span>

<span data-ttu-id="4e629-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4e629-138">The following is an example of the response.</span></span> 

><span data-ttu-id="4e629-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e629-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
