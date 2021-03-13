---
title: Marca de atualização
description: Atualize as propriedades de um objeto tag.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ee8d46d92b7f5e29a4612d3399028dacc36ad6fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776393"
---
# <a name="update-tag"></a><span data-ttu-id="9254f-103">Marca de atualização</span><span class="sxs-lookup"><span data-stu-id="9254f-103">Update tag</span></span>

<span data-ttu-id="9254f-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9254f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9254f-105">Atualize as propriedades de um [objeto tag.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="9254f-105">Update the properties of a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9254f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9254f-106">Permissions</span></span>

<span data-ttu-id="9254f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9254f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9254f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9254f-109">Permission type</span></span>|<span data-ttu-id="9254f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9254f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9254f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9254f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9254f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9254f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="9254f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9254f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9254f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9254f-114">Not supported.</span></span>|
|<span data-ttu-id="9254f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9254f-115">Application</span></span>|<span data-ttu-id="9254f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9254f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9254f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9254f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/tags/{tagId}
```

## <a name="request-headers"></a><span data-ttu-id="9254f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9254f-118">Request headers</span></span>

|<span data-ttu-id="9254f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9254f-119">Name</span></span>|<span data-ttu-id="9254f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9254f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9254f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9254f-121">Authorization</span></span>|<span data-ttu-id="9254f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9254f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9254f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9254f-124">Content-Type</span></span>|<span data-ttu-id="9254f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9254f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9254f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9254f-127">Request body</span></span>

<span data-ttu-id="9254f-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="9254f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9254f-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9254f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9254f-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9254f-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="9254f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9254f-131">Property</span></span>|<span data-ttu-id="9254f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9254f-132">Type</span></span>|<span data-ttu-id="9254f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9254f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9254f-134">description</span><span class="sxs-lookup"><span data-stu-id="9254f-134">description</span></span>|<span data-ttu-id="9254f-135">String</span><span class="sxs-lookup"><span data-stu-id="9254f-135">String</span></span>|<span data-ttu-id="9254f-136">A descrição da marca.</span><span class="sxs-lookup"><span data-stu-id="9254f-136">The description for the tag.</span></span>|
|<span data-ttu-id="9254f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9254f-137">displayName</span></span>|<span data-ttu-id="9254f-138">String</span><span class="sxs-lookup"><span data-stu-id="9254f-138">String</span></span>|<span data-ttu-id="9254f-139">Nome de exibição da marca.</span><span class="sxs-lookup"><span data-stu-id="9254f-139">Display name of the tag.</span></span>|

## <a name="response"></a><span data-ttu-id="9254f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9254f-140">Response</span></span>

<span data-ttu-id="9254f-141">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9254f-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9254f-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9254f-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9254f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9254f-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9254f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9254f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tag"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504
Content-Type: application/json
Content-length: 210

{
  "description":"This is an updated description."
}
```
# <a name="c"></a>[<span data-ttu-id="9254f-145">C#</span><span class="sxs-lookup"><span data-stu-id="9254f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9254f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9254f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9254f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9254f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9254f-148">Java</span><span class="sxs-lookup"><span data-stu-id="9254f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9254f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9254f-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
