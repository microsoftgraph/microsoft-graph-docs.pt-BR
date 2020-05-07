---
title: Atualizar openShift
description: Atualiza as propriedades de um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f816593cdf370d3fb2df647d0f91ed09c53117fc
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155072"
---
# <a name="update-openshift"></a><span data-ttu-id="3af08-103">Atualizar openShift</span><span class="sxs-lookup"><span data-stu-id="3af08-103">Update openShift</span></span>

<span data-ttu-id="3af08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3af08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3af08-105">Atualiza as propriedades de um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="3af08-105">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3af08-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3af08-106">Permissions</span></span>

<span data-ttu-id="3af08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3af08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3af08-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3af08-109">Permission type</span></span>                        | <span data-ttu-id="3af08-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3af08-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3af08-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3af08-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3af08-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3af08-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="3af08-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3af08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3af08-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3af08-114">Not supported.</span></span> |
| <span data-ttu-id="3af08-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3af08-115">Application</span></span>                            | <span data-ttu-id="3af08-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3af08-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="3af08-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="3af08-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3af08-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="3af08-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3af08-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3af08-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="3af08-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3af08-120">Request headers</span></span>

| <span data-ttu-id="3af08-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3af08-121">Name</span></span>       | <span data-ttu-id="3af08-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3af08-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3af08-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3af08-123">Authorization</span></span> | <span data-ttu-id="3af08-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3af08-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3af08-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="3af08-126">Content-type</span></span> | <span data-ttu-id="3af08-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3af08-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3af08-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3af08-129">Request body</span></span>

<span data-ttu-id="3af08-130">Forneça o objeto [openShift](../resources/openshift.md) modificado no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="3af08-130">Provide the modified [openShift](../resources/openshift.md) object in the request body for this method.</span></span>

| <span data-ttu-id="3af08-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3af08-131">Property</span></span>     | <span data-ttu-id="3af08-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3af08-132">Type</span></span>        | <span data-ttu-id="3af08-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3af08-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3af08-134">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="3af08-134">draftOpenShift</span></span>|<span data-ttu-id="3af08-135">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="3af08-135">openShiftItem</span></span>|<span data-ttu-id="3af08-136">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="3af08-136">An unpublished open shift.</span></span>|
|<span data-ttu-id="3af08-137">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="3af08-137">schedulingGroupId</span></span>|<span data-ttu-id="3af08-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3af08-138">String</span></span>| <span data-ttu-id="3af08-139">ID do grupo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="3af08-139">Scheduling group ID.</span></span> |
|<span data-ttu-id="3af08-140">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="3af08-140">sharedOpenShift</span></span>|<span data-ttu-id="3af08-141">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="3af08-141">openShiftItem</span></span>|<span data-ttu-id="3af08-142">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="3af08-142">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="3af08-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3af08-143">Response</span></span>

<span data-ttu-id="3af08-144">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [openShift](../resources/openshift.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3af08-144">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3af08-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3af08-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3af08-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3af08-146">Request</span></span>

<span data-ttu-id="3af08-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3af08-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PUT https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
Content-type: application/json

{
"schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
"sharedOpenShift": {
"notes": "Inventory Management",
"openSlotCount":5,
"displayName": "Field shift",
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
"draftOpenShift": null
}
```

---


### <a name="response"></a><span data-ttu-id="3af08-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3af08-148">Response</span></span>

<span data-ttu-id="3af08-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3af08-149">The following is an example of the response.</span></span>

> <span data-ttu-id="3af08-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3af08-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "openSlotCount":5,
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
  "description": "Update openshift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
