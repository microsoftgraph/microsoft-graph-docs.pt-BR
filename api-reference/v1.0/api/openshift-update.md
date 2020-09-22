---
title: Atualizar openShift
description: Atualiza as propriedades de um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 71b6dc24bb4eb6426e5b15ca7c4147ae77ff1457
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032933"
---
# <a name="update-openshift"></a><span data-ttu-id="31c5e-103">Atualizar openShift</span><span class="sxs-lookup"><span data-stu-id="31c5e-103">Update openShift</span></span>

<span data-ttu-id="31c5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31c5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31c5e-105">Atualiza as propriedades de um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="31c5e-105">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31c5e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31c5e-106">Permissions</span></span>

<span data-ttu-id="31c5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31c5e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31c5e-109">Permission type</span></span>                        | <span data-ttu-id="31c5e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31c5e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="31c5e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31c5e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="31c5e-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="31c5e-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="31c5e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31c5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31c5e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31c5e-114">Not supported.</span></span> |
| <span data-ttu-id="31c5e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31c5e-115">Application</span></span>                            | <span data-ttu-id="31c5e-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c5e-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="31c5e-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="31c5e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="31c5e-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="31c5e-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="31c5e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31c5e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="31c5e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31c5e-120">Request headers</span></span>

| <span data-ttu-id="31c5e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="31c5e-121">Name</span></span>       | <span data-ttu-id="31c5e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="31c5e-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="31c5e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31c5e-123">Authorization</span></span> | <span data-ttu-id="31c5e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31c5e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31c5e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="31c5e-126">Content-type</span></span> | <span data-ttu-id="31c5e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31c5e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31c5e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31c5e-129">Request body</span></span>

<span data-ttu-id="31c5e-130">Forneça o objeto [openShift](../resources/openshift.md) modificado no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="31c5e-130">Provide the modified [openShift](../resources/openshift.md) object in the request body for this method.</span></span>

| <span data-ttu-id="31c5e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31c5e-131">Property</span></span>     | <span data-ttu-id="31c5e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="31c5e-132">Type</span></span>        | <span data-ttu-id="31c5e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="31c5e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="31c5e-134">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="31c5e-134">draftOpenShift</span></span>|<span data-ttu-id="31c5e-135">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="31c5e-135">openShiftItem</span></span>|<span data-ttu-id="31c5e-136">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="31c5e-136">An unpublished open shift.</span></span>|
|<span data-ttu-id="31c5e-137">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="31c5e-137">schedulingGroupId</span></span>|<span data-ttu-id="31c5e-138">String</span><span class="sxs-lookup"><span data-stu-id="31c5e-138">String</span></span>| <span data-ttu-id="31c5e-139">ID do grupo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="31c5e-139">Scheduling group ID.</span></span> |
|<span data-ttu-id="31c5e-140">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="31c5e-140">sharedOpenShift</span></span>|<span data-ttu-id="31c5e-141">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="31c5e-141">openShiftItem</span></span>|<span data-ttu-id="31c5e-142">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="31c5e-142">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="31c5e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="31c5e-143">Response</span></span>

<span data-ttu-id="31c5e-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [openShift](../resources/openshift.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31c5e-144">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31c5e-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="31c5e-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31c5e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31c5e-146">Request</span></span>

<span data-ttu-id="31c5e-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31c5e-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="31c5e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="31c5e-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
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
# <a name="c"></a>[<span data-ttu-id="31c5e-149">C#</span><span class="sxs-lookup"><span data-stu-id="31c5e-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31c5e-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31c5e-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31c5e-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31c5e-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31c5e-152">Java</span><span class="sxs-lookup"><span data-stu-id="31c5e-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="31c5e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="31c5e-153">Response</span></span>

<span data-ttu-id="31c5e-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31c5e-154">The following is an example of the response.</span></span>

> <span data-ttu-id="31c5e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31c5e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

