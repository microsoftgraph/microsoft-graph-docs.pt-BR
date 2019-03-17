---
title: Criar turno
description: Criar um novo turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ae7ff2f598373d58b2a01b678dbb70ae8e290b2d
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657543"
---
# <a name="create-shift"></a><span data-ttu-id="a09ec-103">Criar turno</span><span class="sxs-lookup"><span data-stu-id="a09ec-103">Create shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a09ec-104">Criar uma nova instância de [turno](../resources/shift.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="a09ec-104">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a09ec-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a09ec-105">Permissions</span></span>

<span data-ttu-id="a09ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a09ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a09ec-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a09ec-108">Permission type</span></span>      | <span data-ttu-id="a09ec-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a09ec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a09ec-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a09ec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a09ec-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09ec-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a09ec-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a09ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a09ec-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a09ec-113">Not supported.</span></span>    |
|<span data-ttu-id="a09ec-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a09ec-114">Application</span></span> | <span data-ttu-id="a09ec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a09ec-115">Not supported.</span></span> |

> <span data-ttu-id="a09ec-116">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a09ec-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a09ec-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="a09ec-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a09ec-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a09ec-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="a09ec-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a09ec-119">Request headers</span></span>

| <span data-ttu-id="a09ec-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a09ec-120">Header</span></span>       | <span data-ttu-id="a09ec-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a09ec-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a09ec-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a09ec-122">Authorization</span></span>  | <span data-ttu-id="a09ec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a09ec-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a09ec-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a09ec-125">Content-Type</span></span>  | <span data-ttu-id="a09ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a09ec-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="a09ec-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a09ec-127">Response</span></span>

<span data-ttu-id="a09ec-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a09ec-128">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a09ec-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a09ec-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a09ec-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a09ec-130">Request</span></span>

<span data-ttu-id="a09ec-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a09ec-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-post-shifts"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts
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

#### <a name="response"></a><span data-ttu-id="a09ec-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a09ec-132">Response</span></span>

<span data-ttu-id="a09ec-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a09ec-133">The following is an example of the response.</span></span> 

><span data-ttu-id="a09ec-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a09ec-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/schedule-post-shifts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
