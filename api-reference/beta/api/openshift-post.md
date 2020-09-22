---
title: Criar openShift
description: Criar uma instância do objeto openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5f9b02e5463c5215e67aef206d5876400ef275a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019940"
---
# <a name="create-openshift"></a><span data-ttu-id="6855f-103">Criar openShift</span><span class="sxs-lookup"><span data-stu-id="6855f-103">Create openShift</span></span>

<span data-ttu-id="6855f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6855f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6855f-105">Criar uma instância de um objeto [openshift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="6855f-105">Create an instance of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6855f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6855f-106">Permissions</span></span>

<span data-ttu-id="6855f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6855f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6855f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6855f-109">Permission type</span></span>                        | <span data-ttu-id="6855f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6855f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6855f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6855f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6855f-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6855f-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6855f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6855f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6855f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6855f-114">Not supported.</span></span> |
| <span data-ttu-id="6855f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6855f-115">Application</span></span>                            | <span data-ttu-id="6855f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6855f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6855f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6855f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShifts
```

## <a name="request-headers"></a><span data-ttu-id="6855f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6855f-118">Request headers</span></span>

| <span data-ttu-id="6855f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6855f-119">Name</span></span>      |<span data-ttu-id="6855f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6855f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6855f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6855f-121">Authorization</span></span> | <span data-ttu-id="6855f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6855f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6855f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="6855f-124">Content-type</span></span> | <span data-ttu-id="6855f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6855f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6855f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6855f-127">Request body</span></span>

<span data-ttu-id="6855f-128">Forneça o novo objeto [openshift](../resources/openshift.md) no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="6855f-128">Provide the new [openshift](../resources/openshift.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6855f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6855f-129">Response</span></span>

<span data-ttu-id="6855f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [openShift](../resources/openshift.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6855f-130">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6855f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6855f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6855f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6855f-132">Request</span></span>

<span data-ttu-id="6855f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6855f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openshifts
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
   "id":"OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
   "schedulingGroupId":"TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
   "sharedOpenShift":{
      "notes":"InventoryManagement",
      "openSlotCount":2,
      "displayName":"Dayshift",
      "startDateTime":"2018-10-04T00: 58: 45.340Z",
      "endDateTime":"2018-10-04T09: 50: 45.332Z",
      "theme":"white",
      "activities":[
         {
            "isPaid":true,
            "startDateTime":"2018-10-04T00: 58: 45.340Z",
            "endDateTime":"2018-10-04T01: 58: 45.340Z",
            "code":"",
            "displayName":"Lunch"
         }
      ]
   },
   "draftOpenShift":null,
   "createdDateTime":"2019-03-14T04: 32: 51.451Z",
   "lastModifiedDateTime":"2019-03-14T05: 32: 51.451Z",
   "lastModifiedBy":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
         "displayName":"JohnDoe"
      }
   }
}
```

### <a name="response"></a><span data-ttu-id="6855f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6855f-134">Response</span></span>

<span data-ttu-id="6855f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6855f-135">The following is an example of the response.</span></span>

> <span data-ttu-id="6855f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6855f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "draftOpenShift": null,
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


