---
title: Atualizar swapShiftsChangeRequest
description: Atualiza as propriedades de um objeto swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 141b011ab1dbca436c39e9e48f8312fea77ec6f0
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895539"
---
# <a name="update-swapshiftschangerequest"></a><span data-ttu-id="3ac53-103">Atualizar swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="3ac53-103">Update swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ac53-104">Atualiza as propriedades de um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="3ac53-104">Update the properties of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ac53-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ac53-105">Permissions</span></span>

<span data-ttu-id="3ac53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ac53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ac53-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ac53-108">Permission type</span></span>                        | <span data-ttu-id="3ac53-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ac53-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ac53-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ac53-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ac53-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ac53-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="3ac53-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ac53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ac53-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ac53-113">Not supported.</span></span> |
| <span data-ttu-id="3ac53-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ac53-114">Application</span></span>                            | <span data-ttu-id="3ac53-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ac53-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ac53-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ac53-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="3ac53-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ac53-117">Request headers</span></span>

| <span data-ttu-id="3ac53-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3ac53-118">Name</span></span>       | <span data-ttu-id="3ac53-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ac53-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3ac53-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ac53-120">Authorization</span></span> | <span data-ttu-id="3ac53-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ac53-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ac53-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="3ac53-123">Content-type</span></span> | <span data-ttu-id="3ac53-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ac53-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ac53-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ac53-126">Request body</span></span>

<span data-ttu-id="3ac53-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="3ac53-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3ac53-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="3ac53-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3ac53-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3ac53-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3ac53-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ac53-130">Property</span></span>     | <span data-ttu-id="3ac53-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ac53-131">Type</span></span>        | <span data-ttu-id="3ac53-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ac53-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ac53-133">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="3ac53-133">recipientShiftId</span></span>|<span data-ttu-id="3ac53-134">String</span><span class="sxs-lookup"><span data-stu-id="3ac53-134">String</span></span>|<span data-ttu-id="3ac53-135">A ID do destinatário da solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="3ac53-135">The ID of the recipient of the swap request.</span></span> <span data-ttu-id="3ac53-136">Este é o usuário que é solicitado a trocar por.</span><span class="sxs-lookup"><span data-stu-id="3ac53-136">This is the user who is requested to swap with.</span></span>|

## <a name="response"></a><span data-ttu-id="3ac53-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ac53-137">Response</span></span>

<span data-ttu-id="3ac53-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ac53-138">If successful, this method returns a `200 OK` response code and an updated [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ac53-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3ac53-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ac53-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ac53-140">Request</span></span>

<span data-ttu-id="3ac53-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ac53-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_swapshiftschangerequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
Content-type: application/json

{
  "recipientShiftId": "recipientShiftId-value"
}
```

### <a name="response"></a><span data-ttu-id="3ac53-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ac53-142">Response</span></span>

<span data-ttu-id="3ac53-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ac53-143">The following is an example of the response.</span></span>

> <span data-ttu-id="3ac53-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ac53-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientShiftId": "recipientShiftId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update swapshiftschangerequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
