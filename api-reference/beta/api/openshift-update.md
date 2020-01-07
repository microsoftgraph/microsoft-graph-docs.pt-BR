---
title: Atualizar openShift
description: Atualiza as propriedades de um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aeb686da646a7665cb262761ead92bb182ef12ee
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951892"
---
# <a name="update-openshift"></a><span data-ttu-id="2e390-103">Atualizar openShift</span><span class="sxs-lookup"><span data-stu-id="2e390-103">Update openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e390-104">Atualiza as propriedades de um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="2e390-104">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e390-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e390-105">Permissions</span></span>

<span data-ttu-id="2e390-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e390-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e390-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e390-108">Permission type</span></span>                        | <span data-ttu-id="2e390-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e390-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e390-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e390-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e390-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e390-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2e390-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e390-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e390-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e390-113">Not supported.</span></span> |
| <span data-ttu-id="2e390-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e390-114">Application</span></span>                            | <span data-ttu-id="2e390-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e390-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e390-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e390-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="2e390-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e390-117">Request headers</span></span>

| <span data-ttu-id="2e390-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2e390-118">Name</span></span>       | <span data-ttu-id="2e390-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e390-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2e390-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e390-120">Authorization</span></span> | <span data-ttu-id="2e390-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e390-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e390-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="2e390-123">Content-type</span></span> | <span data-ttu-id="2e390-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e390-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e390-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e390-126">Request body</span></span>

<span data-ttu-id="2e390-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="2e390-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2e390-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="2e390-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2e390-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2e390-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2e390-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e390-130">Property</span></span>     | <span data-ttu-id="2e390-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e390-131">Type</span></span>        | <span data-ttu-id="2e390-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e390-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2e390-133">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="2e390-133">draftOpenShift</span></span>|<span data-ttu-id="2e390-134">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="2e390-134">openShiftItem</span></span>|<span data-ttu-id="2e390-135">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="2e390-135">An unpublished open shift.</span></span>|
|<span data-ttu-id="2e390-136">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="2e390-136">schedulingGroupId</span></span>|<span data-ttu-id="2e390-137">String</span><span class="sxs-lookup"><span data-stu-id="2e390-137">String</span></span>| <span data-ttu-id="2e390-138">ID do grupo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="2e390-138">Scheduling group id.</span></span> |
|<span data-ttu-id="2e390-139">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="2e390-139">sharedOpenShift</span></span>|<span data-ttu-id="2e390-140">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="2e390-140">openShiftItem</span></span>|<span data-ttu-id="2e390-141">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="2e390-141">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="2e390-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e390-142">Response</span></span>

<span data-ttu-id="2e390-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [openShift](../resources/openshift.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e390-143">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e390-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2e390-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e390-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e390-145">Request</span></span>

<span data-ttu-id="2e390-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e390-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2e390-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e390-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PUT https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/{openShiftId}
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e390-148">C#</span><span class="sxs-lookup"><span data-stu-id="2e390-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e390-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e390-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e390-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e390-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e390-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e390-151">Response</span></span>

<span data-ttu-id="2e390-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e390-152">The following is an example of the response.</span></span>

> <span data-ttu-id="2e390-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e390-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
