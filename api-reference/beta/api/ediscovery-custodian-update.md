---
title: Atualizar custodiatário
description: Atualize as propriedades de um objeto custodiante.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 051c7db53f9d949018583fcb2f6a1e44ce2eddb9
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786009"
---
# <a name="update-custodian"></a><span data-ttu-id="a82bd-103">Atualizar custodiatário</span><span class="sxs-lookup"><span data-stu-id="a82bd-103">Update custodian</span></span>

<span data-ttu-id="a82bd-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a82bd-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a82bd-105">Atualize as propriedades de [um objeto custodiante.](../resources/ediscovery-custodian.md)</span><span class="sxs-lookup"><span data-stu-id="a82bd-105">Update the properties of a [custodian](../resources/ediscovery-custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a82bd-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a82bd-106">Permissions</span></span>

<span data-ttu-id="a82bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a82bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a82bd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a82bd-109">Permission type</span></span>|<span data-ttu-id="a82bd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a82bd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a82bd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a82bd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a82bd-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a82bd-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a82bd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a82bd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a82bd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a82bd-114">Not supported.</span></span>|
|<span data-ttu-id="a82bd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a82bd-115">Application</span></span>|<span data-ttu-id="a82bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a82bd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a82bd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a82bd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}
```

## <a name="request-headers"></a><span data-ttu-id="a82bd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a82bd-118">Request headers</span></span>

|<span data-ttu-id="a82bd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a82bd-119">Name</span></span>|<span data-ttu-id="a82bd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a82bd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a82bd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a82bd-121">Authorization</span></span>|<span data-ttu-id="a82bd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a82bd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a82bd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a82bd-124">Content-Type</span></span>|<span data-ttu-id="a82bd-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a82bd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a82bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a82bd-127">Request body</span></span>

<span data-ttu-id="a82bd-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a82bd-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a82bd-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a82bd-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a82bd-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a82bd-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="a82bd-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a82bd-131">Property</span></span>|<span data-ttu-id="a82bd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a82bd-132">Type</span></span>|<span data-ttu-id="a82bd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a82bd-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a82bd-134">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="a82bd-134">applyHoldToSources</span></span>|<span data-ttu-id="a82bd-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="a82bd-135">Boolean</span></span>|<span data-ttu-id="a82bd-136">Identifica se as fontes de um custodiador foram colocadas em espera durante a criação.</span><span class="sxs-lookup"><span data-stu-id="a82bd-136">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|

## <a name="response"></a><span data-ttu-id="a82bd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a82bd-137">Response</span></span>

<span data-ttu-id="a82bd-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a82bd-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a82bd-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a82bd-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a82bd-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a82bd-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a82bd-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a82bd-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_custodian"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
Content-Type: application/json
Content-length: 254

{
  "applyHoldToSources": "false",
}
```
# <a name="c"></a>[<span data-ttu-id="a82bd-142">C#</span><span class="sxs-lookup"><span data-stu-id="a82bd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-custodian-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a82bd-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a82bd-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-custodian-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a82bd-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a82bd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-custodian-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a82bd-145">Java</span><span class="sxs-lookup"><span data-stu-id="a82bd-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-custodian-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a82bd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a82bd-146">Response</span></span>

<!-- {
  "blockType": "response"
}
-->

``` http
HTTP/1.1 204 No Content
```
