---
title: Criar turno
description: Criar um novo turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 638887c06e42347af230f31344e7e7ffa2e96494
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410714"
---
# <a name="create-shift"></a><span data-ttu-id="14dad-103">Criar turno</span><span class="sxs-lookup"><span data-stu-id="14dad-103">Create shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14dad-104">Criar uma nova instância de [turno](../resources/shift.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="14dad-104">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="14dad-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="14dad-105">Permissions</span></span>

<span data-ttu-id="14dad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14dad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14dad-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14dad-108">Permission type</span></span>      | <span data-ttu-id="14dad-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14dad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14dad-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14dad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="14dad-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14dad-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14dad-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14dad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14dad-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14dad-113">Not supported.</span></span>    |
|<span data-ttu-id="14dad-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14dad-114">Application</span></span> | <span data-ttu-id="14dad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14dad-115">Not supported.</span></span> |

> <span data-ttu-id="14dad-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="14dad-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="14dad-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="14dad-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="14dad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14dad-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="14dad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14dad-119">Request headers</span></span>

| <span data-ttu-id="14dad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14dad-120">Header</span></span>       | <span data-ttu-id="14dad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="14dad-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14dad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14dad-122">Authorization</span></span>  | <span data-ttu-id="14dad-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14dad-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="14dad-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14dad-125">Content-Type</span></span>  | <span data-ttu-id="14dad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14dad-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="14dad-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="14dad-127">Response</span></span>

<span data-ttu-id="14dad-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14dad-128">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14dad-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14dad-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="14dad-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14dad-130">Request</span></span>

<span data-ttu-id="14dad-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14dad-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="14dad-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="14dad-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="14dad-133">C#</span><span class="sxs-lookup"><span data-stu-id="14dad-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14dad-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14dad-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="14dad-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="14dad-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="14dad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="14dad-136">Response</span></span>

<span data-ttu-id="14dad-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14dad-137">The following is an example of the response.</span></span> 

><span data-ttu-id="14dad-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14dad-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
