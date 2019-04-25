---
title: Obter turno
description: Obter um turno por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 60d2aa9c09305ee016d16d15514e14d91cf7a5cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537494"
---
# <a name="get-shift"></a><span data-ttu-id="90ca4-103">Obter turno</span><span class="sxs-lookup"><span data-stu-id="90ca4-103">Get shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90ca4-104">Recupere as propriedades e os relacionamentos de um objeto [Shift](../resources/shift.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="90ca4-104">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="90ca4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="90ca4-105">Permissions</span></span>

<span data-ttu-id="90ca4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90ca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ca4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90ca4-108">Permission type</span></span>      | <span data-ttu-id="90ca4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90ca4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90ca4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90ca4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90ca4-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ca4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="90ca4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90ca4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90ca4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90ca4-113">Not supported.</span></span>    |
|<span data-ttu-id="90ca4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90ca4-114">Application</span></span> | <span data-ttu-id="90ca4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90ca4-115">Not supported.</span></span> |

> <span data-ttu-id="90ca4-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="90ca4-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="90ca4-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="90ca4-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="90ca4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90ca4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="90ca4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca4-119">Request headers</span></span>

| <span data-ttu-id="90ca4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90ca4-120">Header</span></span>       | <span data-ttu-id="90ca4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90ca4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90ca4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90ca4-122">Authorization</span></span>  | <span data-ttu-id="90ca4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90ca4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90ca4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90ca4-125">Content-Type</span></span>  | <span data-ttu-id="90ca4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90ca4-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90ca4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca4-127">Request body</span></span>
<span data-ttu-id="90ca4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90ca4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90ca4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ca4-129">Response</span></span>

<span data-ttu-id="90ca4-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90ca4-130">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ca4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90ca4-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="90ca4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca4-132">Request</span></span>

<span data-ttu-id="90ca4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90ca4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```

#### <a name="response"></a><span data-ttu-id="90ca4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ca4-134">Response</span></span>

<span data-ttu-id="90ca4-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90ca4-135">The following is an example of the response.</span></span> 

><span data-ttu-id="90ca4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90ca4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/shift-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
