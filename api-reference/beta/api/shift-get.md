---
title: Obter turno
description: Obter um turno por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e02c7df12eb0ba69400490f6e62d1608ca0c13b4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869802"
---
# <a name="get-shift"></a><span data-ttu-id="d2c8f-103">Obter turno</span><span class="sxs-lookup"><span data-stu-id="d2c8f-103">Get shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2c8f-104">Recupere as propriedades e os relacionamentos de um objeto [Shift](../resources/shift.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-104">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2c8f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2c8f-105">Permissions</span></span>

<span data-ttu-id="d2c8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2c8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2c8f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2c8f-108">Permission type</span></span>      | <span data-ttu-id="d2c8f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2c8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2c8f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2c8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2c8f-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2c8f-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2c8f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2c8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2c8f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-113">Not supported.</span></span>    |
|<span data-ttu-id="d2c8f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2c8f-114">Application</span></span> | <span data-ttu-id="d2c8f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-115">Not supported.</span></span> |

> <span data-ttu-id="d2c8f-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d2c8f-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d2c8f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2c8f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="d2c8f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c8f-119">Request headers</span></span>

| <span data-ttu-id="d2c8f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2c8f-120">Header</span></span>       | <span data-ttu-id="d2c8f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d2c8f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2c8f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2c8f-122">Authorization</span></span>  | <span data-ttu-id="d2c8f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2c8f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2c8f-125">Content-Type</span></span>  | <span data-ttu-id="d2c8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2c8f-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2c8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c8f-127">Request body</span></span>
<span data-ttu-id="d2c8f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2c8f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2c8f-129">Response</span></span>

<span data-ttu-id="d2c8f-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-130">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2c8f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2c8f-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d2c8f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c8f-132">Request</span></span>

<span data-ttu-id="d2c8f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2c8f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2c8f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2c8f-135">C#</span><span class="sxs-lookup"><span data-stu-id="d2c8f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2c8f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2c8f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2c8f-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d2c8f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2c8f-138">Java</span><span class="sxs-lookup"><span data-stu-id="d2c8f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d2c8f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2c8f-139">Response</span></span>

<span data-ttu-id="d2c8f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-140">The following is an example of the response.</span></span> 

><span data-ttu-id="d2c8f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2c8f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Get a shift by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
