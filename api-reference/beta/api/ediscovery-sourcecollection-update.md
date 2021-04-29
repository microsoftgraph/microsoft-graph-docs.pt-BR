---
title: Atualizar sourceCollection
description: Atualize as propriedades de um objeto sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 482d60dcec4e6f169bbf6962b20deebfbc52f5d5
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080240"
---
# <a name="update-sourcecollection"></a><span data-ttu-id="e5743-103">Atualizar sourceCollection</span><span class="sxs-lookup"><span data-stu-id="e5743-103">Update sourceCollection</span></span>

<span data-ttu-id="e5743-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e5743-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5743-105">Atualize as propriedades de um [objeto sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="e5743-105">Update the properties of a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5743-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5743-106">Permissions</span></span>

<span data-ttu-id="e5743-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5743-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5743-109">Permission type</span></span>|<span data-ttu-id="e5743-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5743-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5743-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5743-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5743-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5743-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e5743-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5743-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5743-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5743-114">Not supported.</span></span>|
|<span data-ttu-id="e5743-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5743-115">Application</span></span>|<span data-ttu-id="e5743-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5743-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5743-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5743-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="request-headers"></a><span data-ttu-id="e5743-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5743-118">Request headers</span></span>

|<span data-ttu-id="e5743-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e5743-119">Name</span></span>|<span data-ttu-id="e5743-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5743-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e5743-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5743-121">Authorization</span></span>|<span data-ttu-id="e5743-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5743-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e5743-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5743-124">Content-Type</span></span>|<span data-ttu-id="e5743-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5743-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5743-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5743-127">Request body</span></span>

<span data-ttu-id="e5743-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e5743-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e5743-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e5743-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e5743-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e5743-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="e5743-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5743-131">Property</span></span>|<span data-ttu-id="e5743-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5743-132">Type</span></span>|<span data-ttu-id="e5743-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5743-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5743-134">contentQuery</span><span class="sxs-lookup"><span data-stu-id="e5743-134">contentQuery</span></span>|<span data-ttu-id="e5743-135">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e5743-135">String</span></span>|<span data-ttu-id="e5743-136">A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language).</span><span class="sxs-lookup"><span data-stu-id="e5743-136">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="e5743-137">Para obter detalhes, consulte [Consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta De Conteúdo.](/microsoft-365/compliance/keyword-queries-and-search-conditions)</span><span class="sxs-lookup"><span data-stu-id="e5743-137">For details, see [Keyword queries and search conditions for Content Search and eDiscovery](/microsoft-365/compliance/keyword-queries-and-search-conditions).</span></span>  <span data-ttu-id="e5743-138">Você pode refinar pesquisas usando campos emparelhados com valores; por exemplo, `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016` .</span><span class="sxs-lookup"><span data-stu-id="e5743-138">You can refine searches by using fields paired with values; for example, `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016`.</span></span>|
|<span data-ttu-id="e5743-139">dataSourceScopes</span><span class="sxs-lookup"><span data-stu-id="e5743-139">dataSourceScopes</span></span>|<span data-ttu-id="e5743-140">microsoft.graph.ediscovery.dataSourceScopes</span><span class="sxs-lookup"><span data-stu-id="e5743-140">microsoft.graph.ediscovery.dataSourceScopes</span></span>|<span data-ttu-id="e5743-141">Quando especificado, a coleção se estenderá por um serviço para uma carga de trabalho inteira.</span><span class="sxs-lookup"><span data-stu-id="e5743-141">When specified, the collection will span across a service for an entire workload.</span></span> <span data-ttu-id="e5743-142">Os valores possíveis são: `none` , , , , `allTenantMailboxes` `allTenantSites` `allCaseCustodians` `allCaseNoncustodialDataSources` .</span><span class="sxs-lookup"><span data-stu-id="e5743-142">Possible values are: `none`,`allTenantMailboxes`,`allTenantSites`,`allCaseCustodians`,`allCaseNoncustodialDataSources`.</span></span> <span data-ttu-id="e5743-143">**Observação:** Um custodiante ou a especificação de dadosSourceScope é necessária ao criar uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="e5743-143">**Note:** Either one custodian or specifying dataSourceScope is required when creating a source collection.</span></span>|
|<span data-ttu-id="e5743-144">description</span><span class="sxs-lookup"><span data-stu-id="e5743-144">description</span></span>|<span data-ttu-id="e5743-145">String</span><span class="sxs-lookup"><span data-stu-id="e5743-145">String</span></span>|<span data-ttu-id="e5743-146">A descrição da **sourceCollection**.</span><span class="sxs-lookup"><span data-stu-id="e5743-146">The description of the **sourceCollection**.</span></span>|
|<span data-ttu-id="e5743-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e5743-147">displayName</span></span>|<span data-ttu-id="e5743-148">String</span><span class="sxs-lookup"><span data-stu-id="e5743-148">String</span></span>|<span data-ttu-id="e5743-149">O nome de exibição do **sourceCollection**.</span><span class="sxs-lookup"><span data-stu-id="e5743-149">The display name of the **sourceCollection**.</span></span>|

## <a name="response"></a><span data-ttu-id="e5743-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5743-150">Response</span></span>

<span data-ttu-id="e5743-151">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e5743-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e5743-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e5743-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5743-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5743-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e5743-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5743-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_sourcecollection"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119
Content-Type: application/json
Content-length: 247

{
    "displayName": "Quarterly Financials search",
}
```
# <a name="c"></a>[<span data-ttu-id="e5743-155">C#</span><span class="sxs-lookup"><span data-stu-id="e5743-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-sourcecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5743-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5743-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-sourcecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5743-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5743-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-sourcecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5743-158">Java</span><span class="sxs-lookup"><span data-stu-id="e5743-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-sourcecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5743-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5743-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
