---
title: Atualizar openShift
description: Atualiza as propriedades de um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 821ad6579d7e77959263aab91511e71e0352e364
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867783"
---
# <a name="update-openshift"></a><span data-ttu-id="0d7d2-103">Atualizar openShift</span><span class="sxs-lookup"><span data-stu-id="0d7d2-103">Update openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d7d2-104">Atualiza as propriedades de um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="0d7d2-104">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d7d2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d7d2-105">Permissions</span></span>

<span data-ttu-id="0d7d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d7d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d7d2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d7d2-108">Permission type</span></span>                        | <span data-ttu-id="0d7d2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d7d2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d7d2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d7d2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d7d2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d7d2-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="0d7d2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d7d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d7d2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-113">Not supported.</span></span> |
| <span data-ttu-id="0d7d2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d7d2-114">Application</span></span>                            | <span data-ttu-id="0d7d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d7d2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d7d2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/openShifts
```

## <a name="request-headers"></a><span data-ttu-id="0d7d2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d7d2-117">Request headers</span></span>

| <span data-ttu-id="0d7d2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0d7d2-118">Name</span></span>       | <span data-ttu-id="0d7d2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d7d2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0d7d2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d7d2-120">Authorization</span></span> | <span data-ttu-id="0d7d2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0d7d2-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="0d7d2-123">Content-type</span></span> | <span data-ttu-id="0d7d2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d7d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d7d2-126">Request body</span></span>

<span data-ttu-id="0d7d2-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0d7d2-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0d7d2-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d7d2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d7d2-130">Property</span></span>     | <span data-ttu-id="0d7d2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d7d2-131">Type</span></span>        | <span data-ttu-id="0d7d2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d7d2-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d7d2-133">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="0d7d2-133">draftOpenShift</span></span>|<span data-ttu-id="0d7d2-134">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="0d7d2-134">openShiftItem</span></span>|<span data-ttu-id="0d7d2-135">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-135">An unpublished open shift.</span></span>|
|<span data-ttu-id="0d7d2-136">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="0d7d2-136">schedulingGroupId</span></span>|<span data-ttu-id="0d7d2-137">String</span><span class="sxs-lookup"><span data-stu-id="0d7d2-137">String</span></span>| <span data-ttu-id="0d7d2-138">ID do grupo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-138">Scheduling group id.</span></span> |
|<span data-ttu-id="0d7d2-139">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="0d7d2-139">sharedOpenShift</span></span>|<span data-ttu-id="0d7d2-140">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="0d7d2-140">openShiftItem</span></span>|<span data-ttu-id="0d7d2-141">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-141">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="0d7d2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d7d2-142">Response</span></span>

<span data-ttu-id="0d7d2-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [openShift](../resources/openshift.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-143">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d7d2-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d7d2-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d7d2-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d7d2-145">Request</span></span>

<span data-ttu-id="0d7d2-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0d7d2-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d7d2-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts
Content-type: application/json

{
  "sharedOpenShift": {
    "openSlotCount": 99
  },
  "draftOpenShift": {
    "openSlotCount": 99
  },
  "schedulingGroupId": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0d7d2-148">C#</span><span class="sxs-lookup"><span data-stu-id="0d7d2-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d7d2-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d7d2-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0d7d2-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d7d2-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0d7d2-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d7d2-151">Response</span></span>

<span data-ttu-id="0d7d2-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-152">The following is an example of the response.</span></span>

> <span data-ttu-id="0d7d2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d7d2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "sharedOpenShift": {
    "openSlotCount": 99
  },
  "draftOpenShift": {
    "openSlotCount": 99
  },
  "schedulingGroupId": "schedulingGroupId-value"
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
