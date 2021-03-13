---
title: Atualizar legalHold
description: Atualize as propriedades de um objeto legalHold.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 21789c048ee18fd604e44110bea7e995c891b17f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772945"
---
# <a name="update-legalhold"></a><span data-ttu-id="37497-103">Atualizar legalHold</span><span class="sxs-lookup"><span data-stu-id="37497-103">Update legalHold</span></span>

<span data-ttu-id="37497-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="37497-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37497-105">Atualize as propriedades de um [objeto legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="37497-105">Update the properties of a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37497-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="37497-106">Permissions</span></span>

<span data-ttu-id="37497-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37497-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37497-109">Permission type</span></span>|<span data-ttu-id="37497-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37497-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37497-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37497-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37497-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37497-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="37497-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37497-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37497-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37497-114">Not supported.</span></span>|
|<span data-ttu-id="37497-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37497-115">Application</span></span>|<span data-ttu-id="37497-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37497-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37497-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37497-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

## <a name="request-headers"></a><span data-ttu-id="37497-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37497-118">Request headers</span></span>

|<span data-ttu-id="37497-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37497-119">Name</span></span>|<span data-ttu-id="37497-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37497-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37497-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37497-121">Authorization</span></span>|<span data-ttu-id="37497-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37497-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="37497-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37497-124">Content-Type</span></span>|<span data-ttu-id="37497-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37497-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37497-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37497-127">Request body</span></span>

<span data-ttu-id="37497-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="37497-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="37497-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="37497-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="37497-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="37497-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="37497-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37497-131">Property</span></span>|<span data-ttu-id="37497-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="37497-132">Type</span></span>|<span data-ttu-id="37497-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="37497-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37497-134">contentQuery</span><span class="sxs-lookup"><span data-stu-id="37497-134">contentQuery</span></span>|<span data-ttu-id="37497-135">String</span><span class="sxs-lookup"><span data-stu-id="37497-135">String</span></span>|<span data-ttu-id="37497-136">Consulta KQL que especifica o conteúdo a ser mantido nos locais especificados.</span><span class="sxs-lookup"><span data-stu-id="37497-136">KQL query that specifies content to be held in the specified locations.</span></span> <span data-ttu-id="37497-137">Para obter mais informações sobre KQL na Descoberta Digital, consulte Consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo [e Descoberta Digital.](/microsoft-365/compliance/keyword-queries-and-search-conditions)</span><span class="sxs-lookup"><span data-stu-id="37497-137">For more information about KQL in eDiscovery, see [Keyword queries and search conditions for Content Search and eDiscovery](/microsoft-365/compliance/keyword-queries-and-search-conditions).</span></span> <span data-ttu-id="37497-138">Para manter todo o conteúdo nos locais especificados, deixe **contentQuery em** branco.</span><span class="sxs-lookup"><span data-stu-id="37497-138">To hold all content in the specified locations, leave **contentQuery** blank.</span></span> |
|<span data-ttu-id="37497-139">descrição</span><span class="sxs-lookup"><span data-stu-id="37497-139">description</span></span>|<span data-ttu-id="37497-140">String</span><span class="sxs-lookup"><span data-stu-id="37497-140">String</span></span>| <span data-ttu-id="37497-141">A descrição de espera legal.</span><span class="sxs-lookup"><span data-stu-id="37497-141">The legal hold description.</span></span> |
|<span data-ttu-id="37497-142">displayName</span><span class="sxs-lookup"><span data-stu-id="37497-142">displayName</span></span>|<span data-ttu-id="37497-143">String</span><span class="sxs-lookup"><span data-stu-id="37497-143">String</span></span>| <span data-ttu-id="37497-144">O nome de exibição da ressução legal.</span><span class="sxs-lookup"><span data-stu-id="37497-144">The display name of the legal hold.</span></span> |
|<span data-ttu-id="37497-145">isEnabled</span><span class="sxs-lookup"><span data-stu-id="37497-145">isEnabled</span></span>|<span data-ttu-id="37497-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="37497-146">Boolean</span></span>|<span data-ttu-id="37497-147">Indica se a espera está habilitada e mantendo o conteúdo ativamente.</span><span class="sxs-lookup"><span data-stu-id="37497-147">Indicates whether the hold is enabled and actively holding content.</span></span> |

## <a name="response"></a><span data-ttu-id="37497-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="37497-148">Response</span></span>

<span data-ttu-id="37497-149">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="37497-149">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="37497-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37497-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37497-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37497-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37497-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="37497-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_legalhold"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
Content-Type: application/json
Content-length: 295

{
  "description": "This is a description for a legalHold"
}
```
# <a name="c"></a>[<span data-ttu-id="37497-153">C#</span><span class="sxs-lookup"><span data-stu-id="37497-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-legalhold-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37497-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37497-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-legalhold-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37497-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37497-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-legalhold-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37497-156">Java</span><span class="sxs-lookup"><span data-stu-id="37497-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-legalhold-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37497-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="37497-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 204 No Content
```
