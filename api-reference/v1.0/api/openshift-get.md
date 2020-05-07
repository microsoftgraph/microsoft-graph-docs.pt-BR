---
title: Obter openShift
description: Recupere as propriedades e os relacionamentos do objeto openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c63c494f64930d96c7174d315bf271e4b07e7d7e
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155093"
---
# <a name="get-openshift"></a><span data-ttu-id="8586f-103">Obter openShift</span><span class="sxs-lookup"><span data-stu-id="8586f-103">Get openShift</span></span>

<span data-ttu-id="8586f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8586f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8586f-105">Recupere as propriedades e os relacionamentos de um objeto [openshift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="8586f-105">Retrieve the properties and relationships of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8586f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8586f-106">Permissions</span></span>

<span data-ttu-id="8586f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8586f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8586f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8586f-109">Permission type</span></span>                        | <span data-ttu-id="8586f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8586f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8586f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8586f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8586f-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8586f-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8586f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8586f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8586f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8586f-114">Not supported.</span></span> |
| <span data-ttu-id="8586f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8586f-115">Application</span></span>                            | <span data-ttu-id="8586f-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8586f-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="8586f-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="8586f-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8586f-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="8586f-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8586f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8586f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts/{openShiftId}
```
 
## <a name="request-headers"></a><span data-ttu-id="8586f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8586f-120">Request headers</span></span>

| <span data-ttu-id="8586f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8586f-121">Name</span></span>      |<span data-ttu-id="8586f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8586f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8586f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8586f-123">Authorization</span></span> | <span data-ttu-id="8586f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8586f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8586f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8586f-126">Request body</span></span>

<span data-ttu-id="8586f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8586f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8586f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8586f-128">Response</span></span>

<span data-ttu-id="8586f-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [openShift](../resources/openshift.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8586f-129">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8586f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8586f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8586f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8586f-131">Request</span></span>

<span data-ttu-id="8586f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8586f-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
---


### <a name="response"></a><span data-ttu-id="8586f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8586f-133">Response</span></span>

<span data-ttu-id="8586f-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8586f-134">The following is an example of the response.</span></span>

> <span data-ttu-id="8586f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8586f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":2,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T09:50:45.332Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T01:58:45.340Z",
  "code": "",
  "displayName": "Lunch"
  }
  ]
  },
  "draftOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":3,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.332Z",
  "endDateTime": "2018-10-04T08:58:45.340Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T07:58:45.332Z",
  "code": "Break",
  "displayName": "Lunch"
  }
  ]
  },
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "lastModifiedBy": {
  "application": null,
  "device": null,
  "conversation": null,
  "user": {
  "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
  "displayName": "John Doe"
  }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
