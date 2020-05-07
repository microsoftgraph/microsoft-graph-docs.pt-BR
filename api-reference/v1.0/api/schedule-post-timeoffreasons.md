---
title: Criar timeOffReason
description: Criar um novo timeOffReason.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 01c73bf703dd0015111d4f235f6dc027f05125ad
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155037"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="4cb0b-103">Criar timeOffReason</span><span class="sxs-lookup"><span data-stu-id="4cb0b-103">Create timeOffReason</span></span>

<span data-ttu-id="4cb0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cb0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cb0b-105">Criar um novo [timeOffReason](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="4cb0b-105">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4cb0b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4cb0b-106">Permissions</span></span>

<span data-ttu-id="4cb0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cb0b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cb0b-109">Permission type</span></span>      | <span data-ttu-id="4cb0b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4cb0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cb0b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cb0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4cb0b-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4cb0b-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4cb0b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cb0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cb0b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-114">Not supported.</span></span>    |
|<span data-ttu-id="4cb0b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cb0b-115">Application</span></span> | <span data-ttu-id="4cb0b-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cb0b-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="4cb0b-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4cb0b-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4cb0b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cb0b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="4cb0b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cb0b-120">Request headers</span></span>

| <span data-ttu-id="4cb0b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4cb0b-121">Header</span></span>       | <span data-ttu-id="4cb0b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4cb0b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4cb0b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4cb0b-123">Authorization</span></span>  | <span data-ttu-id="4cb0b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4cb0b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4cb0b-126">Content-Type</span></span>  | <span data-ttu-id="4cb0b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="4cb0b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cb0b-129">Response</span></span>

<span data-ttu-id="4cb0b-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-130">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cb0b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4cb0b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cb0b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cb0b-132">Request</span></span>

<span data-ttu-id="4cb0b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-post-timeoffreasons"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons
Content-type: application/json

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
---


### <a name="response"></a><span data-ttu-id="4cb0b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cb0b-134">Response</span></span>

<span data-ttu-id="4cb0b-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-135">The following is an example of the response.</span></span> 

><span data-ttu-id="4cb0b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
