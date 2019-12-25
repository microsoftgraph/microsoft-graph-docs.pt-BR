---
title: Substituir Shift
description: Substitua um turno existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 729441e7379c98270ab5df6c0ac10dbd920d308b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870908"
---
# <a name="replace-shift"></a><span data-ttu-id="95af7-103">Substituir Shift</span><span class="sxs-lookup"><span data-stu-id="95af7-103">Replace shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95af7-104">Substitua um [turno](../resources/shift.md)existente.</span><span class="sxs-lookup"><span data-stu-id="95af7-104">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="95af7-105">Se o [turno](../resources/shift.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="95af7-105">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="95af7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="95af7-106">Permissions</span></span>

<span data-ttu-id="95af7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95af7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95af7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95af7-109">Permission type</span></span>      | <span data-ttu-id="95af7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95af7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95af7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95af7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="95af7-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95af7-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="95af7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95af7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95af7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95af7-114">Not supported.</span></span>    |
|<span data-ttu-id="95af7-115">Application</span><span class="sxs-lookup"><span data-stu-id="95af7-115">Application</span></span> | <span data-ttu-id="95af7-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="95af7-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="95af7-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="95af7-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="95af7-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="95af7-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="95af7-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="95af7-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="95af7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95af7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="95af7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95af7-121">Request headers</span></span>

| <span data-ttu-id="95af7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95af7-122">Header</span></span>       | <span data-ttu-id="95af7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="95af7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95af7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="95af7-124">Authorization</span></span>  | <span data-ttu-id="95af7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95af7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95af7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95af7-127">Content-Type</span></span>  | <span data-ttu-id="95af7-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95af7-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95af7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95af7-130">Request body</span></span>

<span data-ttu-id="95af7-131">No corpo da solicitação, forneça uma representação JSON de um objeto [Shift](../resources/shift.md) .</span><span class="sxs-lookup"><span data-stu-id="95af7-131">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="95af7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="95af7-132">Response</span></span>

<span data-ttu-id="95af7-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95af7-133">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95af7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95af7-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="95af7-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95af7-135">Request</span></span>

<span data-ttu-id="95af7-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="95af7-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="95af7-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="95af7-137">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="95af7-138">C#</span><span class="sxs-lookup"><span data-stu-id="95af7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95af7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95af7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="95af7-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95af7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95af7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="95af7-141">Response</span></span>

<span data-ttu-id="95af7-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="95af7-142">The following is an example of the response.</span></span> 

><span data-ttu-id="95af7-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95af7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
