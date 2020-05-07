---
title: Criar turno
description: Criar um novo turno.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d0a3722be034337d27e2f1984529abea7ac71974
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154463"
---
# <a name="create-shift"></a><span data-ttu-id="749d9-103">Criar turno</span><span class="sxs-lookup"><span data-stu-id="749d9-103">Create shift</span></span>

<span data-ttu-id="749d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="749d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="749d9-105">Criar uma nova instância de [turno](../resources/shift.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="749d9-105">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="749d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="749d9-106">Permissions</span></span>

<span data-ttu-id="749d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="749d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="749d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="749d9-109">Permission type</span></span>      | <span data-ttu-id="749d9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="749d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="749d9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="749d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="749d9-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="749d9-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="749d9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="749d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="749d9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="749d9-114">Not supported.</span></span>    |
|<span data-ttu-id="749d9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="749d9-115">Application</span></span> | <span data-ttu-id="749d9-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="749d9-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="749d9-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="749d9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="749d9-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="749d9-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="749d9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="749d9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="749d9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="749d9-120">Request headers</span></span>

| <span data-ttu-id="749d9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="749d9-121">Header</span></span>       | <span data-ttu-id="749d9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="749d9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="749d9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="749d9-123">Authorization</span></span>  | <span data-ttu-id="749d9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="749d9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="749d9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="749d9-126">Content-Type</span></span>  | <span data-ttu-id="749d9-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="749d9-p104">application/json. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="749d9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="749d9-129">Response</span></span>

<span data-ttu-id="749d9-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="749d9-130">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="749d9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="749d9-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="749d9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="749d9-132">Request</span></span>

<span data-ttu-id="749d9-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="749d9-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-post-shifts"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts
Content-type: application/json

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```
---


#### <a name="response"></a><span data-ttu-id="749d9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="749d9-134">Response</span></span>

<span data-ttu-id="749d9-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="749d9-135">The following is an example of the response.</span></span> 

><span data-ttu-id="749d9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="749d9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
