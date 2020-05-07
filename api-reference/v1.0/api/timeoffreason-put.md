---
title: Substituir timeOffReason
description: Substitua um timeOffReason existente.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3719ac2dedc45854bab2b2f82bde19fe1af2f6d2
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155002"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="59b4e-103">Substituir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="59b4e-103">Replace timeOffReason</span></span>

<span data-ttu-id="59b4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59b4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59b4e-105">Substitua um [timeOffReason](../resources/timeoffreason.md)existente.</span><span class="sxs-lookup"><span data-stu-id="59b4e-105">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="59b4e-106">Se o [timeOffReason](../resources/timeoffreason.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="59b4e-106">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="59b4e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="59b4e-107">Permissions</span></span>

<span data-ttu-id="59b4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59b4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59b4e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59b4e-110">Permission type</span></span>      | <span data-ttu-id="59b4e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59b4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59b4e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59b4e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59b4e-113">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="59b4e-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="59b4e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59b4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59b4e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59b4e-115">Not supported.</span></span>    |
|<span data-ttu-id="59b4e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59b4e-116">Application</span></span> | <span data-ttu-id="59b4e-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59b4e-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="59b4e-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="59b4e-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="59b4e-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="59b4e-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="59b4e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59b4e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="59b4e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59b4e-121">Request headers</span></span>

| <span data-ttu-id="59b4e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59b4e-122">Header</span></span>       | <span data-ttu-id="59b4e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="59b4e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59b4e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="59b4e-124">Authorization</span></span>  | <span data-ttu-id="59b4e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59b4e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59b4e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59b4e-127">Content-Type</span></span>  | <span data-ttu-id="59b4e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59b4e-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59b4e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59b4e-130">Request body</span></span>

<span data-ttu-id="59b4e-131">No corpo da solicitação, forneça uma representação JSON de um objeto [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="59b4e-131">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="59b4e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="59b4e-132">Response</span></span>

<span data-ttu-id="59b4e-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59b4e-133">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59b4e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59b4e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="59b4e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59b4e-135">Request</span></span>

<span data-ttu-id="59b4e-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59b4e-136">The following is an example of the request.</span></span>

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
---


### <a name="response"></a><span data-ttu-id="59b4e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="59b4e-137">Response</span></span>

<span data-ttu-id="59b4e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59b4e-138">The following is an example of the response.</span></span> 

><span data-ttu-id="59b4e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59b4e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
