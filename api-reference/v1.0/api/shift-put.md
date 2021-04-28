---
title: Substituir turno
description: Substitua um turno existente.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 888932c4732bca7f15a5eb61327cda9bb554b762
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034893"
---
# <a name="replace-shift"></a><span data-ttu-id="bff9a-103">Substituir turno</span><span class="sxs-lookup"><span data-stu-id="bff9a-103">Replace shift</span></span>

<span data-ttu-id="bff9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bff9a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bff9a-105">Substitua um turno [existente](../resources/shift.md).</span><span class="sxs-lookup"><span data-stu-id="bff9a-105">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="bff9a-106">Se o turno [especificado](../resources/shift.md) não existir, este método retornará `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="bff9a-106">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="bff9a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bff9a-107">Permissions</span></span>

<span data-ttu-id="bff9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bff9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bff9a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bff9a-110">Permission type</span></span>      | <span data-ttu-id="bff9a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bff9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bff9a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bff9a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bff9a-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bff9a-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bff9a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bff9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bff9a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bff9a-115">Not supported.</span></span>    |
|<span data-ttu-id="bff9a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bff9a-116">Application</span></span> | <span data-ttu-id="bff9a-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bff9a-117">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bff9a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bff9a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="bff9a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bff9a-119">Request headers</span></span>

| <span data-ttu-id="bff9a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bff9a-120">Header</span></span>       | <span data-ttu-id="bff9a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bff9a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bff9a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bff9a-122">Authorization</span></span>  | <span data-ttu-id="bff9a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bff9a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bff9a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bff9a-125">Content-Type</span></span>  | <span data-ttu-id="bff9a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bff9a-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bff9a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bff9a-128">Request body</span></span>

<span data-ttu-id="bff9a-129">No corpo da solicitação, fornece uma representação JSON de um [objeto shift.](../resources/shift.md)</span><span class="sxs-lookup"><span data-stu-id="bff9a-129">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bff9a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bff9a-130">Response</span></span>

<span data-ttu-id="bff9a-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bff9a-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bff9a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bff9a-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bff9a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bff9a-133">Request</span></span>

<span data-ttu-id="bff9a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bff9a-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bff9a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bff9a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-put"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
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
# <a name="c"></a>[<span data-ttu-id="bff9a-136">C#</span><span class="sxs-lookup"><span data-stu-id="bff9a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bff9a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bff9a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bff9a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bff9a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bff9a-139">Java</span><span class="sxs-lookup"><span data-stu-id="bff9a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="bff9a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bff9a-140">Response</span></span>

<span data-ttu-id="bff9a-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bff9a-141">The following is an example of the response.</span></span> 

><span data-ttu-id="bff9a-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bff9a-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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

