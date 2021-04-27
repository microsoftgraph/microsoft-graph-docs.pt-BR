---
title: Atualizar reviewSetQuery
description: Atualize as propriedades de um objeto reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d5ce888c2b4a32e175ddc69e2edc6f2df0fc0411
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044547"
---
# <a name="update-reviewsetquery"></a><span data-ttu-id="d920a-103">Atualizar reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="d920a-103">Update reviewSetQuery</span></span>

<span data-ttu-id="d920a-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d920a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d920a-105">Atualize as propriedades de uma revisão de Descoberta [AutomáticaSetQuery](../resources/ediscovery-reviewsetquery.md).</span><span class="sxs-lookup"><span data-stu-id="d920a-105">Update the properties of an eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d920a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d920a-106">Permissions</span></span>

<span data-ttu-id="d920a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d920a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d920a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d920a-109">Permission type</span></span>|<span data-ttu-id="d920a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d920a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d920a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d920a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d920a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d920a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d920a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d920a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d920a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d920a-114">Not supported.</span></span>|
|<span data-ttu-id="d920a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d920a-115">Application</span></span>|<span data-ttu-id="d920a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d920a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d920a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d920a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d920a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d920a-118">Request headers</span></span>

| <span data-ttu-id="d920a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d920a-119">Name</span></span>       | <span data-ttu-id="d920a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d920a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d920a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d920a-121">Authorization</span></span> | <span data-ttu-id="d920a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d920a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d920a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d920a-124">Request body</span></span>

<span data-ttu-id="d920a-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d920a-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d920a-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d920a-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d920a-127">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d920a-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d920a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d920a-128">Property</span></span>     | <span data-ttu-id="d920a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d920a-129">Type</span></span>        | <span data-ttu-id="d920a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d920a-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d920a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="d920a-131">displayName</span></span> | <span data-ttu-id="d920a-132">String</span><span class="sxs-lookup"><span data-stu-id="d920a-132">String</span></span> | <span data-ttu-id="d920a-133">Nome de exibição para eles revisarem a consulta de conjunto.</span><span class="sxs-lookup"><span data-stu-id="d920a-133">Display name for they review set query.</span></span> |
| <span data-ttu-id="d920a-134">consulta</span><span class="sxs-lookup"><span data-stu-id="d920a-134">query</span></span> | <span data-ttu-id="d920a-135">String</span><span class="sxs-lookup"><span data-stu-id="d920a-135">String</span></span> | <span data-ttu-id="d920a-136">A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language).</span><span class="sxs-lookup"><span data-stu-id="d920a-136">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="d920a-137">Para obter detalhes, consulte [Campos de metadados de documento](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="d920a-137">For details, see [Document metadata fields](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span> |

## <a name="response"></a><span data-ttu-id="d920a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d920a-138">Response</span></span>

<span data-ttu-id="d920a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d920a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d920a-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d920a-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d920a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d920a-142">Request</span></span>

<span data-ttu-id="d920a-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d920a-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d920a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d920a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_reviewsetquery"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
Content-type: application/json

{
  "displayName": "My Query 1 - Renamed"
}
```
# <a name="c"></a>[<span data-ttu-id="d920a-145">C#</span><span class="sxs-lookup"><span data-stu-id="d920a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d920a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d920a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d920a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d920a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d920a-148">Java</span><span class="sxs-lookup"><span data-stu-id="d920a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d920a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d920a-149">Response</span></span>

<span data-ttu-id="d920a-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d920a-150">The following is an example of the response.</span></span>

> <span data-ttu-id="d920a-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d920a-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewsetquery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
