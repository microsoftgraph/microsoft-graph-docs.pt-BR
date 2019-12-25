---
title: Criar turno
description: Criar um novo turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ed3e1e5d908d3683afeebe19a37b640cae567593
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867978"
---
# <a name="create-shift"></a><span data-ttu-id="a71d0-103">Criar turno</span><span class="sxs-lookup"><span data-stu-id="a71d0-103">Create shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a71d0-104">Criar uma nova instância de [turno](../resources/shift.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="a71d0-104">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a71d0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a71d0-105">Permissions</span></span>

<span data-ttu-id="a71d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a71d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a71d0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a71d0-108">Permission type</span></span>      | <span data-ttu-id="a71d0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a71d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a71d0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a71d0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a71d0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a71d0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a71d0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a71d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a71d0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a71d0-113">Not supported.</span></span>    |
|<span data-ttu-id="a71d0-114">Application</span><span class="sxs-lookup"><span data-stu-id="a71d0-114">Application</span></span> | <span data-ttu-id="a71d0-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="a71d0-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="a71d0-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="a71d0-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="a71d0-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a71d0-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a71d0-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="a71d0-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a71d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a71d0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="a71d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a71d0-120">Request headers</span></span>

| <span data-ttu-id="a71d0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a71d0-121">Header</span></span>       | <span data-ttu-id="a71d0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a71d0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a71d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a71d0-123">Authorization</span></span>  | <span data-ttu-id="a71d0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a71d0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a71d0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a71d0-126">Content-Type</span></span>  | <span data-ttu-id="a71d0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a71d0-p104">application/json. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a71d0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a71d0-129">Response</span></span>

<span data-ttu-id="a71d0-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a71d0-130">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a71d0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a71d0-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a71d0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a71d0-132">Request</span></span>

<span data-ttu-id="a71d0-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a71d0-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a71d0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a71d0-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a71d0-135">C#</span><span class="sxs-lookup"><span data-stu-id="a71d0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a71d0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a71d0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a71d0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a71d0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a71d0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a71d0-138">Response</span></span>

<span data-ttu-id="a71d0-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a71d0-139">The following is an example of the response.</span></span> 

><span data-ttu-id="a71d0-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a71d0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
