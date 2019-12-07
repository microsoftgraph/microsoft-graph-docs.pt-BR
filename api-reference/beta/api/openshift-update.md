---
title: Atualizar openShift
description: Atualiza as propriedades de um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5863b3a52eb195fed205788480cf1e5eda1237eb
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895553"
---
# <a name="update-openshift"></a><span data-ttu-id="7085c-103">Atualizar openShift</span><span class="sxs-lookup"><span data-stu-id="7085c-103">Update openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7085c-104">Atualiza as propriedades de um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="7085c-104">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7085c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7085c-105">Permissions</span></span>

<span data-ttu-id="7085c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7085c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7085c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7085c-108">Permission type</span></span>                        | <span data-ttu-id="7085c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7085c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7085c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7085c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7085c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7085c-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="7085c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7085c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7085c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7085c-113">Not supported.</span></span> |
| <span data-ttu-id="7085c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7085c-114">Application</span></span>                            | <span data-ttu-id="7085c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7085c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7085c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7085c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/openShifts
```

## <a name="request-headers"></a><span data-ttu-id="7085c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7085c-117">Request headers</span></span>

| <span data-ttu-id="7085c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7085c-118">Name</span></span>       | <span data-ttu-id="7085c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7085c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7085c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7085c-120">Authorization</span></span> | <span data-ttu-id="7085c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7085c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7085c-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="7085c-123">Content-type</span></span> | <span data-ttu-id="7085c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7085c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7085c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7085c-126">Request body</span></span>

<span data-ttu-id="7085c-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7085c-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7085c-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7085c-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7085c-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7085c-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7085c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7085c-130">Property</span></span>     | <span data-ttu-id="7085c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7085c-131">Type</span></span>        | <span data-ttu-id="7085c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7085c-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7085c-133">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="7085c-133">draftOpenShift</span></span>|<span data-ttu-id="7085c-134">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="7085c-134">openShiftItem</span></span>|<span data-ttu-id="7085c-135">Um turno aberto não publicado.</span><span class="sxs-lookup"><span data-stu-id="7085c-135">An unpublished open shift.</span></span>|
|<span data-ttu-id="7085c-136">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="7085c-136">schedulingGroupId</span></span>|<span data-ttu-id="7085c-137">String</span><span class="sxs-lookup"><span data-stu-id="7085c-137">String</span></span>| <span data-ttu-id="7085c-138">ID do grupo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="7085c-138">Scheduling group id.</span></span> |
|<span data-ttu-id="7085c-139">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="7085c-139">sharedOpenShift</span></span>|<span data-ttu-id="7085c-140">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="7085c-140">openShiftItem</span></span>|<span data-ttu-id="7085c-141">Um turno aberto publicado.</span><span class="sxs-lookup"><span data-stu-id="7085c-141">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="7085c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7085c-142">Response</span></span>

<span data-ttu-id="7085c-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [openShift](../resources/openshift.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7085c-143">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7085c-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7085c-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7085c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7085c-145">Request</span></span>

<span data-ttu-id="7085c-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7085c-146">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7085c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="7085c-147">Response</span></span>

<span data-ttu-id="7085c-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7085c-148">The following is an example of the response.</span></span>

> <span data-ttu-id="7085c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7085c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
