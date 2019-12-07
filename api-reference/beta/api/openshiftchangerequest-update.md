---
title: Atualizar openShiftChangeRequest
description: Atualiza as propriedades de um objeto openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e58461437206809e1c71803c03781b704323fc81
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895541"
---
# <a name="update-openshiftchangerequest"></a><span data-ttu-id="ce666-103">Atualizar openshiftchangerequest</span><span class="sxs-lookup"><span data-stu-id="ce666-103">Update openshiftchangerequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce666-104">Atualiza as propriedades de um objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ce666-104">Update the properties of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce666-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce666-105">Permissions</span></span>

<span data-ttu-id="ce666-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce666-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce666-108">Permission type</span></span>                        | <span data-ttu-id="ce666-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce666-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce666-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce666-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce666-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce666-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ce666-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce666-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce666-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce666-113">Not supported.</span></span> |
| <span data-ttu-id="ce666-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce666-114">Application</span></span>                            | <span data-ttu-id="ce666-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce666-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce666-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce666-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="ce666-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce666-117">Request headers</span></span>

| <span data-ttu-id="ce666-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ce666-118">Name</span></span>       | <span data-ttu-id="ce666-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce666-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ce666-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce666-120">Authorization</span></span> | <span data-ttu-id="ce666-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce666-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce666-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="ce666-123">Content-type</span></span> | <span data-ttu-id="ce666-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce666-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce666-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce666-126">Request body</span></span>

<span data-ttu-id="ce666-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ce666-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ce666-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ce666-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ce666-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ce666-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ce666-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce666-130">Property</span></span>     | <span data-ttu-id="ce666-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce666-131">Type</span></span>        | <span data-ttu-id="ce666-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce666-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce666-133">openShiftId</span><span class="sxs-lookup"><span data-stu-id="ce666-133">openShiftId</span></span>|<span data-ttu-id="ce666-134">String</span><span class="sxs-lookup"><span data-stu-id="ce666-134">String</span></span>|<span data-ttu-id="ce666-135">ID para o turno aberto.</span><span class="sxs-lookup"><span data-stu-id="ce666-135">ID for the open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="ce666-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce666-136">Response</span></span>

<span data-ttu-id="ce666-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce666-137">If successful, this method returns a `200 OK` response code and an updated [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce666-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce666-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce666-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce666-139">Request</span></span>

<span data-ttu-id="ce666-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce666-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_openshiftchangerequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests
Content-type: application/json

{
  "openShiftId": "openShiftId-value"
}
```

### <a name="response"></a><span data-ttu-id="ce666-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce666-141">Response</span></span>

<span data-ttu-id="ce666-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce666-142">The following is an example of the response.</span></span>

> <span data-ttu-id="ce666-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce666-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "openShiftId": "openShiftId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update openshiftchangerequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
