---
title: Listar openShifts
description: Listar objetos openshift em uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 76a5fd1976c117834924ba9edca1652b77ab406a
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155086"
---
# <a name="list-openshifts"></a><span data-ttu-id="19962-103">Listar openShifts</span><span class="sxs-lookup"><span data-stu-id="19962-103">List openShifts</span></span>

<span data-ttu-id="19962-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19962-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19962-105">Listar objetos [openShift](../resources/openshift.md) em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="19962-105">List [openShift](../resources/openshift.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="19962-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="19962-106">Permissions</span></span>

<span data-ttu-id="19962-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19962-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19962-109">Permission type</span></span>                        | <span data-ttu-id="19962-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19962-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19962-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19962-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="19962-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="19962-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="19962-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19962-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19962-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19962-114">Not supported.</span></span> |
| <span data-ttu-id="19962-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19962-115">Application</span></span>                            | <span data-ttu-id="19962-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="19962-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="19962-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="19962-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="19962-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="19962-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="19962-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19962-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19962-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="19962-120">Optional query parameters</span></span>

<span data-ttu-id="19962-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="19962-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="19962-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="19962-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="19962-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19962-123">Request headers</span></span>

| <span data-ttu-id="19962-124">Nome</span><span class="sxs-lookup"><span data-stu-id="19962-124">Name</span></span>      |<span data-ttu-id="19962-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="19962-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19962-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="19962-126">Authorization</span></span> | <span data-ttu-id="19962-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19962-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19962-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19962-129">Request body</span></span>

<span data-ttu-id="19962-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19962-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19962-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="19962-131">Response</span></span>

<span data-ttu-id="19962-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e todos os objetos [openShift](../resources/openshift.md) na equipe no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19962-132">If successful, this method returns a `200 OK` response code and all [openShift](../resources/openshift.md) objects in the team in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19962-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19962-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19962-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19962-134">Request</span></span>

<span data-ttu-id="19962-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19962-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts
```
---


### <a name="response"></a><span data-ttu-id="19962-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="19962-136">Response</span></span>

<span data-ttu-id="19962-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19962-137">The following is an example of the response.</span></span>

> <span data-ttu-id="19962-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19962-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
