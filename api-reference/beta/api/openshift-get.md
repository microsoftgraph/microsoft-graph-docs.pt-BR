---
title: Obter openShift
description: Recupere as propriedades e os relacionamentos do objeto openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1ef127e1262b070c421b159aaea55b74156956c2
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951906"
---
# <a name="get-openshift"></a><span data-ttu-id="3cd2b-103">Obter openShift</span><span class="sxs-lookup"><span data-stu-id="3cd2b-103">Get openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cd2b-104">Recupere as propriedades e os relacionamentos de um objeto [openshift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="3cd2b-104">Retrieve the properties and relationships of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cd2b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cd2b-105">Permissions</span></span>

<span data-ttu-id="3cd2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cd2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3cd2b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cd2b-108">Permission type</span></span>                        | <span data-ttu-id="3cd2b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cd2b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3cd2b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cd2b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cd2b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd2b-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="3cd2b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cd2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cd2b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cd2b-113">Not supported.</span></span> |
| <span data-ttu-id="3cd2b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cd2b-114">Application</span></span>                            | <span data-ttu-id="3cd2b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cd2b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cd2b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd2b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cd2b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3cd2b-117">Optional query parameters</span></span>

<span data-ttu-id="3cd2b-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3cd2b-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3cd2b-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3cd2b-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="3cd2b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd2b-120">Request headers</span></span>

| <span data-ttu-id="3cd2b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3cd2b-121">Name</span></span>      |<span data-ttu-id="3cd2b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cd2b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3cd2b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cd2b-123">Authorization</span></span> | <span data-ttu-id="3cd2b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cd2b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cd2b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd2b-126">Request body</span></span>

<span data-ttu-id="3cd2b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cd2b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cd2b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd2b-128">Response</span></span>

<span data-ttu-id="3cd2b-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [openShift](../resources/openshift.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cd2b-129">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3cd2b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3cd2b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cd2b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd2b-131">Request</span></span>

<span data-ttu-id="3cd2b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cd2b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```

### <a name="response"></a><span data-ttu-id="3cd2b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd2b-133">Response</span></span>

<span data-ttu-id="3cd2b-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3cd2b-134">The following is an example of the response.</span></span>

> <span data-ttu-id="3cd2b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cd2b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
