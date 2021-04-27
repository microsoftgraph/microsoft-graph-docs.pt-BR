---
title: Criar turno
description: Crie um novo turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e74b00a6ec3563d5ee47b13fb4d082d6a0e9bfaf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052730"
---
# <a name="create-shift"></a><span data-ttu-id="a6155-103">Criar turno</span><span class="sxs-lookup"><span data-stu-id="a6155-103">Create shift</span></span>

<span data-ttu-id="a6155-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6155-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6155-105">Crie uma nova [instância de turno](../resources/shift.md) em um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="a6155-105">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6155-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6155-106">Permissions</span></span>

<span data-ttu-id="a6155-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6155-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6155-109">Permission type</span></span>      | <span data-ttu-id="a6155-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6155-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6155-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6155-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6155-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6155-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6155-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6155-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6155-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6155-114">Not supported.</span></span>    |
|<span data-ttu-id="a6155-115">Application</span><span class="sxs-lookup"><span data-stu-id="a6155-115">Application</span></span> | <span data-ttu-id="a6155-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="a6155-116">Schedule.ReadWrite.All\*</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6155-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6155-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="a6155-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6155-118">Request headers</span></span>

| <span data-ttu-id="a6155-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6155-119">Header</span></span>       | <span data-ttu-id="a6155-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a6155-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a6155-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6155-121">Authorization</span></span>  | <span data-ttu-id="a6155-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6155-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a6155-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6155-124">Content-Type</span></span>  | <span data-ttu-id="a6155-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6155-p103">application/json. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a6155-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6155-127">Response</span></span>

<span data-ttu-id="a6155-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6155-128">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6155-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6155-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a6155-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6155-130">Request</span></span>

<span data-ttu-id="a6155-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6155-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6155-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6155-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6155-133">C#</span><span class="sxs-lookup"><span data-stu-id="a6155-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6155-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6155-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6155-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6155-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6155-136">Java</span><span class="sxs-lookup"><span data-stu-id="a6155-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-shifts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a6155-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6155-137">Response</span></span>

<span data-ttu-id="a6155-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6155-138">The following is an example of the response.</span></span> 

><span data-ttu-id="a6155-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a6155-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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


