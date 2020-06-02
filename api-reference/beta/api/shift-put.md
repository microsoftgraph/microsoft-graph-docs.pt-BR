---
title: Substituir Shift
description: Substitua um turno existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: efe7180b352ae29bc64f663fa9122d670378dff5
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "42453325"
---
# <a name="replace-shift"></a><span data-ttu-id="8cc9c-103">Substituir Shift</span><span class="sxs-lookup"><span data-stu-id="8cc9c-103">Replace shift</span></span>

<span data-ttu-id="8cc9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc9c-105">Substitua um [turno](../resources/shift.md)existente.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-105">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="8cc9c-106">Se o [turno](../resources/shift.md) especificado não existir, este método retornará `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="8cc9c-106">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc9c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cc9c-107">Permissions</span></span>

<span data-ttu-id="8cc9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc9c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc9c-110">Permission type</span></span>      | <span data-ttu-id="8cc9c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cc9c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cc9c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc9c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8cc9c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc9c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8cc9c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc9c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc9c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-115">Not supported.</span></span>    |
|<span data-ttu-id="8cc9c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc9c-116">Application</span></span> | <span data-ttu-id="8cc9c-117">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="8cc9c-117">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="8cc9c-118">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="8cc9c-119">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8cc9c-120">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8cc9c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc9c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="8cc9c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc9c-122">Request headers</span></span>

| <span data-ttu-id="8cc9c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cc9c-123">Header</span></span>       | <span data-ttu-id="8cc9c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8cc9c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8cc9c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc9c-125">Authorization</span></span>  | <span data-ttu-id="8cc9c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8cc9c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cc9c-128">Content-Type</span></span>  | <span data-ttu-id="8cc9c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8cc9c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc9c-131">Request body</span></span>

<span data-ttu-id="8cc9c-132">No corpo da solicitação, forneça uma representação JSON de um objeto [Shift](../resources/shift.md) .</span><span class="sxs-lookup"><span data-stu-id="8cc9c-132">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8cc9c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc9c-133">Response</span></span>

<span data-ttu-id="8cc9c-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-134">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc9c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc9c-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8cc9c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc9c-136">Request</span></span>

<span data-ttu-id="8cc9c-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8cc9c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc9c-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8cc9c-139">C#</span><span class="sxs-lookup"><span data-stu-id="8cc9c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cc9c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cc9c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cc9c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cc9c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8cc9c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc9c-142">Response</span></span>

<span data-ttu-id="8cc9c-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-143">The following is an example of the response.</span></span> 

><span data-ttu-id="8cc9c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc9c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
