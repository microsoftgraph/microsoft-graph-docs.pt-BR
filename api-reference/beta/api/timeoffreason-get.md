---
title: Obter timeOffReason
description: Obtenha um timeOffReason por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 73f5f920a6fbd7f56465ff3f35457c2108ca0323
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154413"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="87c65-103">Obter timeOffReason</span><span class="sxs-lookup"><span data-stu-id="87c65-103">Get timeOffReason</span></span>

<span data-ttu-id="87c65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87c65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87c65-105">Recupere as propriedades e os relacionamentos de um objeto [timeOffReason](../resources/timeoffreason.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="87c65-105">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="87c65-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87c65-106">Permissions</span></span>

<span data-ttu-id="87c65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87c65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87c65-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87c65-109">Permission type</span></span>      | <span data-ttu-id="87c65-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87c65-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c65-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87c65-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87c65-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87c65-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="87c65-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87c65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87c65-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87c65-114">Not supported.</span></span>    |
|<span data-ttu-id="87c65-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87c65-115">Application</span></span> | <span data-ttu-id="87c65-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="87c65-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="87c65-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="87c65-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="87c65-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="87c65-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="87c65-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="87c65-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="87c65-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87c65-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87c65-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87c65-121">Optional query parameters</span></span>

<span data-ttu-id="87c65-122">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87c65-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87c65-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87c65-123">Request headers</span></span>

| <span data-ttu-id="87c65-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87c65-124">Header</span></span>       | <span data-ttu-id="87c65-125">Valor</span><span class="sxs-lookup"><span data-stu-id="87c65-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87c65-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="87c65-126">Authorization</span></span>  | <span data-ttu-id="87c65-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87c65-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87c65-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87c65-129">Request body</span></span>
<span data-ttu-id="87c65-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87c65-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87c65-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="87c65-131">Response</span></span>

<span data-ttu-id="87c65-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87c65-132">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87c65-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87c65-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="87c65-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87c65-134">Request</span></span>

<span data-ttu-id="87c65-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87c65-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87c65-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="87c65-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="87c65-137">C#</span><span class="sxs-lookup"><span data-stu-id="87c65-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87c65-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87c65-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87c65-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87c65-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="87c65-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="87c65-140">Response</span></span>

<span data-ttu-id="87c65-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87c65-141">The following is an example of the response.</span></span> 

><span data-ttu-id="87c65-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87c65-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
