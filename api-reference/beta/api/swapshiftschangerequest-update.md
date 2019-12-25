---
title: Atualizar swapShiftsChangeRequest
description: Atualiza as propriedades de um objeto swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0955428ce82f585bbdb085e0d6d2f2f6023f92f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870782"
---
# <a name="update-swapshiftschangerequest"></a><span data-ttu-id="63051-103">Atualizar swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="63051-103">Update swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63051-104">Atualiza as propriedades de um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="63051-104">Update the properties of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63051-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="63051-105">Permissions</span></span>

<span data-ttu-id="63051-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63051-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63051-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63051-108">Permission type</span></span>                        | <span data-ttu-id="63051-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63051-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="63051-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63051-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="63051-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63051-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="63051-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63051-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63051-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63051-113">Not supported.</span></span> |
|<span data-ttu-id="63051-114">Application</span><span class="sxs-lookup"><span data-stu-id="63051-114">Application</span></span> | <span data-ttu-id="63051-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="63051-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="63051-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="63051-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="63051-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63051-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="63051-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63051-118">Request headers</span></span>

| <span data-ttu-id="63051-119">Nome</span><span class="sxs-lookup"><span data-stu-id="63051-119">Name</span></span>       | <span data-ttu-id="63051-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="63051-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="63051-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="63051-121">Authorization</span></span> | <span data-ttu-id="63051-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63051-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63051-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="63051-124">Content-type</span></span> | <span data-ttu-id="63051-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63051-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63051-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63051-127">Request body</span></span>

<span data-ttu-id="63051-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="63051-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="63051-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="63051-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="63051-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="63051-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="63051-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63051-131">Property</span></span>     | <span data-ttu-id="63051-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="63051-132">Type</span></span>        | <span data-ttu-id="63051-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="63051-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63051-134">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="63051-134">recipientShiftId</span></span>|<span data-ttu-id="63051-135">String</span><span class="sxs-lookup"><span data-stu-id="63051-135">String</span></span>|<span data-ttu-id="63051-136">A ID do destinatário da solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="63051-136">The ID of the recipient of the swap request.</span></span> <span data-ttu-id="63051-137">Este é o usuário que é solicitado a trocar por.</span><span class="sxs-lookup"><span data-stu-id="63051-137">This is the user who is requested to swap with.</span></span>|

## <a name="response"></a><span data-ttu-id="63051-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="63051-138">Response</span></span>

<span data-ttu-id="63051-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63051-139">If successful, this method returns a `200 OK` response code and an updated [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63051-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="63051-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="63051-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63051-141">Request</span></span>

<span data-ttu-id="63051-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63051-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63051-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="63051-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="63051-144">C#</span><span class="sxs-lookup"><span data-stu-id="63051-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63051-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63051-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63051-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63051-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63051-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="63051-147">Response</span></span>

<span data-ttu-id="63051-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="63051-148">The following is an example of the response.</span></span>

> <span data-ttu-id="63051-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63051-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
