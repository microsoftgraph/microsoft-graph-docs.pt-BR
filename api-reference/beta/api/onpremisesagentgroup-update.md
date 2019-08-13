---
title: Atualizar onPremisesAgentGroup
description: Atualiza as propriedades de um objeto **onPremisesAgentGroup** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 89c138669422d2530c0166ddae9915d757c79edc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346684"
---
# <a name="update-onpremisesagentgroup"></a><span data-ttu-id="f3e22-103">Atualizar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="f3e22-103">Update onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3e22-104">Atualiza as propriedades de um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="f3e22-104">Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3e22-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3e22-105">Permissions</span></span>

<span data-ttu-id="f3e22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3e22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3e22-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3e22-108">Permission type</span></span>                        | <span data-ttu-id="f3e22-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3e22-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3e22-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3e22-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3e22-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f3e22-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="f3e22-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3e22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3e22-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3e22-113">Not supported.</span></span> |
| <span data-ttu-id="f3e22-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3e22-114">Application</span></span>                            | <span data-ttu-id="f3e22-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3e22-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3e22-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3e22-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="request-headers"></a><span data-ttu-id="f3e22-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3e22-117">Request headers</span></span>

| <span data-ttu-id="f3e22-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f3e22-118">Name</span></span>       | <span data-ttu-id="f3e22-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3e22-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f3e22-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3e22-120">Authorization</span></span> | <span data-ttu-id="f3e22-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f3e22-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3e22-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3e22-122">Request body</span></span>

<span data-ttu-id="f3e22-123">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f3e22-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f3e22-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f3e22-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f3e22-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f3e22-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="f3e22-126">Veja a seguir a lista de propriedades que você pode atualizar.</span><span class="sxs-lookup"><span data-stu-id="f3e22-126">The following is the list of properties that you can update.</span></span>

| <span data-ttu-id="f3e22-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3e22-127">Property</span></span>     | <span data-ttu-id="f3e22-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3e22-128">Type</span></span>        | <span data-ttu-id="f3e22-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3e22-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f3e22-130">displayName</span><span class="sxs-lookup"><span data-stu-id="f3e22-130">displayName</span></span>|<span data-ttu-id="f3e22-131">String</span><span class="sxs-lookup"><span data-stu-id="f3e22-131">String</span></span>| <span data-ttu-id="f3e22-132">Representa o nome do grupo de agentes local.</span><span class="sxs-lookup"><span data-stu-id="f3e22-132">Represents the on-premises agents group name.</span></span>|

## <a name="response"></a><span data-ttu-id="f3e22-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3e22-133">Response</span></span>

<span data-ttu-id="f3e22-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f3e22-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f3e22-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f3e22-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3e22-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3e22-136">Request</span></span>

<span data-ttu-id="f3e22-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3e22-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f3e22-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3e22-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisesagentgroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
Content-type: application/json

{
    "displayName": "Group New Name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f3e22-139">C#</span><span class="sxs-lookup"><span data-stu-id="f3e22-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3e22-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3e22-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f3e22-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f3e22-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f3e22-142">Java</span><span class="sxs-lookup"><span data-stu-id="f3e22-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f3e22-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3e22-143">Response</span></span>

<span data-ttu-id="f3e22-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3e22-144">The following is an example of the response.</span></span>

> <span data-ttu-id="f3e22-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3e22-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update onpremisesagentgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
