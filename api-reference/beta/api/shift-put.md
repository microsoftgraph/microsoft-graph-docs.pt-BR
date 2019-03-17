---
title: Substituir Shift
description: Substitua um turno existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d8614739757e3962e671440a9a893b9b06d6761f
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657844"
---
# <a name="replace-shift"></a><span data-ttu-id="18841-103">Substituir Shift</span><span class="sxs-lookup"><span data-stu-id="18841-103">Replace shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18841-104">Substitua um [turno](../resources/shift.md)existente.</span><span class="sxs-lookup"><span data-stu-id="18841-104">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="18841-105">Se o [turno](../resources/shift.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="18841-105">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="18841-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="18841-106">Permissions</span></span>

<span data-ttu-id="18841-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18841-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18841-109">Permission type</span></span>      | <span data-ttu-id="18841-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18841-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18841-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18841-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18841-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18841-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="18841-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18841-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18841-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18841-114">Not supported.</span></span>    |
|<span data-ttu-id="18841-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18841-115">Application</span></span> | <span data-ttu-id="18841-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18841-116">Not supported.</span></span> |

> <span data-ttu-id="18841-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="18841-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="18841-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="18841-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="18841-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18841-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="18841-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18841-120">Request headers</span></span>

| <span data-ttu-id="18841-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18841-121">Header</span></span>       | <span data-ttu-id="18841-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18841-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18841-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18841-123">Authorization</span></span>  | <span data-ttu-id="18841-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18841-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18841-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18841-126">Content-Type</span></span>  | <span data-ttu-id="18841-127">application/json</span><span class="sxs-lookup"><span data-stu-id="18841-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18841-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18841-128">Request body</span></span>

<span data-ttu-id="18841-129">No corpo da solicitação, forneça uma representação JSON de um objeto [Shift](../resources/shift.md) .</span><span class="sxs-lookup"><span data-stu-id="18841-129">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="18841-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="18841-130">Response</span></span>

<span data-ttu-id="18841-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18841-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18841-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18841-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="18841-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18841-133">Request</span></span>

<span data-ttu-id="18841-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18841-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
Content-type: application/json
Prefer: return=representation

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

#### <a name="response"></a><span data-ttu-id="18841-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="18841-135">Response</span></span>

<span data-ttu-id="18841-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18841-136">The following is an example of the response.</span></span> 

><span data-ttu-id="18841-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18841-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "string",
  "userId": "string",
  "schedulingGroupId": "string",
  "sharedShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "draftShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "createdDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedBy": {
    "user": {
      "id": "string",
      "displayName": "string"
    },
    "application": {
      "id": "string",
      "displayName": "string"
    },
    "device": {
      "id": "string",
      "displayName": "string"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/shift-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
