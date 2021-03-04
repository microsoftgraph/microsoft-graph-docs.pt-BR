---
title: Caso de atualização
description: Atualize as propriedades de um objeto case.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 24b2a72efc8e0f36a6cf8f00161a3ca636987805
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445819"
---
# <a name="update-case"></a><span data-ttu-id="6a2bc-103">Caso de atualização</span><span class="sxs-lookup"><span data-stu-id="6a2bc-103">Update case</span></span>

<span data-ttu-id="6a2bc-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6a2bc-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a2bc-105">Atualize as propriedades de um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="6a2bc-105">Update the properties of a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a2bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a2bc-106">Permissions</span></span>

<span data-ttu-id="6a2bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a2bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a2bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a2bc-109">Permission type</span></span>|<span data-ttu-id="6a2bc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a2bc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a2bc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a2bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a2bc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a2bc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="6a2bc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a2bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a2bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-114">Not supported.</span></span>|
|<span data-ttu-id="6a2bc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a2bc-115">Application</span></span>|<span data-ttu-id="6a2bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a2bc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a2bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a2bc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a2bc-118">Request headers</span></span>

| <span data-ttu-id="6a2bc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6a2bc-119">Name</span></span>       | <span data-ttu-id="6a2bc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a2bc-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6a2bc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a2bc-121">Authorization</span></span> | <span data-ttu-id="6a2bc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a2bc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a2bc-124">Request body</span></span>

<span data-ttu-id="6a2bc-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6a2bc-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6a2bc-127">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6a2bc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a2bc-128">Property</span></span>     | <span data-ttu-id="6a2bc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a2bc-129">Type</span></span>        | <span data-ttu-id="6a2bc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a2bc-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a2bc-131">description</span><span class="sxs-lookup"><span data-stu-id="6a2bc-131">description</span></span>|<span data-ttu-id="6a2bc-132">String</span><span class="sxs-lookup"><span data-stu-id="6a2bc-132">String</span></span>|<span data-ttu-id="6a2bc-133">A descrição do caso.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-133">The case description.</span></span>|
|<span data-ttu-id="6a2bc-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6a2bc-134">displayName</span></span>|<span data-ttu-id="6a2bc-135">String</span><span class="sxs-lookup"><span data-stu-id="6a2bc-135">String</span></span>|<span data-ttu-id="6a2bc-136">O nome do caso.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-136">The case name.</span></span>|
|<span data-ttu-id="6a2bc-137">externalId</span><span class="sxs-lookup"><span data-stu-id="6a2bc-137">externalId</span></span>|<span data-ttu-id="6a2bc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a2bc-138">String</span></span>|<span data-ttu-id="6a2bc-139">O número de caso externo para referência do cliente.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-139">The external case number for customer reference.</span></span>|

## <a name="response"></a><span data-ttu-id="6a2bc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a2bc-140">Response</span></span>

<span data-ttu-id="6a2bc-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-141">If successful, this method returns a `200 OK` response code and an updated [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a2bc-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a2bc-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a2bc-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a2bc-143">Request</span></span>

<span data-ttu-id="6a2bc-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6a2bc-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a2bc-145">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_case"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
Content-type: application/json

{
  "displayName": "My Case 1 - Renamed",
  "description": "Updated description",
  "externalId": "Updated externalId"
}
```

# <a name="c"></a>[<span data-ttu-id="6a2bc-146">C#</span><span class="sxs-lookup"><span data-stu-id="6a2bc-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a2bc-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a2bc-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a2bc-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a2bc-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a2bc-149">Java</span><span class="sxs-lookup"><span data-stu-id="6a2bc-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6a2bc-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a2bc-150">Response</span></span>

<span data-ttu-id="6a2bc-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
