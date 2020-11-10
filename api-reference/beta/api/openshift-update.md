---
title: Atualizar openShift
description: Atualiza as propriedades de um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c17e56fb6fe0f6eb963d30beb35dc867955cea3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976880"
---
# <a name="update-openshift"></a><span data-ttu-id="d0507-103">Atualizar openShift</span><span class="sxs-lookup"><span data-stu-id="d0507-103">Update openShift</span></span>

<span data-ttu-id="d0507-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0507-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0507-105">Atualiza as propriedades de um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="d0507-105">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0507-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0507-106">Permissions</span></span>

<span data-ttu-id="d0507-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0507-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0507-109">Permission type</span></span>                        | <span data-ttu-id="d0507-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0507-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d0507-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0507-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0507-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0507-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d0507-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0507-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0507-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0507-114">Not supported.</span></span> |
| <span data-ttu-id="d0507-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0507-115">Application</span></span>                            | <span data-ttu-id="d0507-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0507-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0507-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0507-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="d0507-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0507-118">Request headers</span></span>

| <span data-ttu-id="d0507-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d0507-119">Name</span></span>       | <span data-ttu-id="d0507-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0507-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d0507-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0507-121">Authorization</span></span> | <span data-ttu-id="d0507-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0507-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0507-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="d0507-124">Content-type</span></span> | <span data-ttu-id="d0507-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0507-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0507-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0507-127">Request body</span></span>

<span data-ttu-id="d0507-128">Forneça o objeto [openshift](../resources/openshift.md) modificado no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="d0507-128">Provide the modified [openshift](../resources/openshift.md) object in the request body for this method.</span></span>

| <span data-ttu-id="d0507-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0507-129">Property</span></span>     | <span data-ttu-id="d0507-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0507-130">Type</span></span>        | <span data-ttu-id="d0507-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0507-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0507-132">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="d0507-132">draftOpenShift</span></span>|<span data-ttu-id="d0507-133">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="d0507-133">openShiftItem</span></span>|<span data-ttu-id="d0507-134">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="d0507-134">An unpublished open shift.</span></span>|
|<span data-ttu-id="d0507-135">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="d0507-135">schedulingGroupId</span></span>|<span data-ttu-id="d0507-136">String</span><span class="sxs-lookup"><span data-stu-id="d0507-136">String</span></span>| <span data-ttu-id="d0507-137">ID do grupo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="d0507-137">Scheduling group id.</span></span> |
|<span data-ttu-id="d0507-138">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="d0507-138">sharedOpenShift</span></span>|<span data-ttu-id="d0507-139">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="d0507-139">openShiftItem</span></span>|<span data-ttu-id="d0507-140">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="d0507-140">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="d0507-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0507-141">Response</span></span>

<span data-ttu-id="d0507-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [openShift](../resources/openshift.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0507-142">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0507-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0507-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0507-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0507-144">Request</span></span>

<span data-ttu-id="d0507-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0507-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0507-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0507-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PUT https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
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
# <a name="c"></a>[<span data-ttu-id="d0507-147">C#</span><span class="sxs-lookup"><span data-stu-id="d0507-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0507-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0507-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0507-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0507-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0507-150">Java</span><span class="sxs-lookup"><span data-stu-id="d0507-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0507-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0507-151">Response</span></span>

<span data-ttu-id="d0507-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0507-152">The following is an example of the response.</span></span>

> <span data-ttu-id="d0507-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0507-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


