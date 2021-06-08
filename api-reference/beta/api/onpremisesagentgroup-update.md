---
title: Atualizar onPremisesAgentGroup
description: Atualize as propriedades de um **objeto onPremisesAgentGroup.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: b78c82989f8fc06daed22dd0a80cb1d07be8e77e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785946"
---
# <a name="update-onpremisesagentgroup"></a><span data-ttu-id="14a24-103">Atualizar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="14a24-103">Update onPremisesAgentGroup</span></span>

<span data-ttu-id="14a24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14a24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14a24-105">Atualize as propriedades de um [objeto onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="14a24-105">Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14a24-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="14a24-106">Permissions</span></span>

<span data-ttu-id="14a24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14a24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14a24-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14a24-109">Permission type</span></span>                        | <span data-ttu-id="14a24-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14a24-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="14a24-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14a24-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14a24-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a24-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="14a24-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14a24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14a24-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14a24-114">Not supported.</span></span> |
| <span data-ttu-id="14a24-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14a24-115">Application</span></span>                            | <span data-ttu-id="14a24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14a24-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14a24-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14a24-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="request-headers"></a><span data-ttu-id="14a24-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14a24-118">Request headers</span></span>

| <span data-ttu-id="14a24-119">Nome</span><span class="sxs-lookup"><span data-stu-id="14a24-119">Name</span></span>       | <span data-ttu-id="14a24-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="14a24-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="14a24-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="14a24-121">Authorization</span></span> | <span data-ttu-id="14a24-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="14a24-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="14a24-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14a24-123">Request body</span></span>

<span data-ttu-id="14a24-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="14a24-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="14a24-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="14a24-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="14a24-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="14a24-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="14a24-127">Veja a seguir a lista de propriedades que você pode atualizar.</span><span class="sxs-lookup"><span data-stu-id="14a24-127">The following is the list of properties that you can update.</span></span>

| <span data-ttu-id="14a24-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14a24-128">Property</span></span>     | <span data-ttu-id="14a24-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="14a24-129">Type</span></span>        | <span data-ttu-id="14a24-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="14a24-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14a24-131">displayName</span><span class="sxs-lookup"><span data-stu-id="14a24-131">displayName</span></span>|<span data-ttu-id="14a24-132">String</span><span class="sxs-lookup"><span data-stu-id="14a24-132">String</span></span>| <span data-ttu-id="14a24-133">Representa o nome do grupo de agentes locais.</span><span class="sxs-lookup"><span data-stu-id="14a24-133">Represents the on-premises agents group name.</span></span>|

## <a name="response"></a><span data-ttu-id="14a24-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="14a24-134">Response</span></span>

<span data-ttu-id="14a24-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="14a24-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="14a24-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14a24-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14a24-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14a24-137">Request</span></span>

<span data-ttu-id="14a24-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14a24-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14a24-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="14a24-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="14a24-140">C#</span><span class="sxs-lookup"><span data-stu-id="14a24-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14a24-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14a24-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14a24-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14a24-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14a24-143">Java</span><span class="sxs-lookup"><span data-stu-id="14a24-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14a24-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="14a24-144">Response</span></span>

<span data-ttu-id="14a24-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14a24-145">The following is an example of the response.</span></span>

> <span data-ttu-id="14a24-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="14a24-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
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



