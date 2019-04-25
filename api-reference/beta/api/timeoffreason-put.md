---
title: Substituir timeOffReason
description: Substitua um timeOffReason existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8c37304d6556bfcee47a0bb631933f29cd8b3986
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548201"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="3c96d-103">Substituir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="3c96d-103">Replace timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c96d-104">Substitua um [timeOffReason](../resources/timeoffreason.md)existente.</span><span class="sxs-lookup"><span data-stu-id="3c96d-104">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="3c96d-105">Se o [timeOffReason](../resources/timeoffreason.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="3c96d-105">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c96d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c96d-106">Permissions</span></span>

<span data-ttu-id="3c96d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c96d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c96d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c96d-109">Permission type</span></span>      | <span data-ttu-id="3c96d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c96d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c96d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c96d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c96d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c96d-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c96d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c96d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c96d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c96d-114">Not supported.</span></span>    |
|<span data-ttu-id="3c96d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c96d-115">Application</span></span> | <span data-ttu-id="3c96d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c96d-116">Not supported.</span></span> |

> <span data-ttu-id="3c96d-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="3c96d-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3c96d-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="3c96d-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c96d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c96d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="3c96d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c96d-120">Request headers</span></span>

| <span data-ttu-id="3c96d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c96d-121">Header</span></span>       | <span data-ttu-id="3c96d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3c96d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c96d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c96d-123">Authorization</span></span>  | <span data-ttu-id="3c96d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c96d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3c96d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c96d-126">Content-Type</span></span>  | <span data-ttu-id="3c96d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3c96d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c96d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c96d-128">Request body</span></span>

<span data-ttu-id="3c96d-129">No corpo da solicitação, forneça uma representação JSON de um objeto [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="3c96d-129">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3c96d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c96d-130">Response</span></span>

<span data-ttu-id="3c96d-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c96d-131">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c96d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c96d-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3c96d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c96d-133">Request</span></span>

<span data-ttu-id="3c96d-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c96d-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="3c96d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c96d-135">Response</span></span>

<span data-ttu-id="3c96d-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c96d-136">The following is an example of the response.</span></span> 

><span data-ttu-id="3c96d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c96d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Replace an existing timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
