---
title: Obter reviewSet
description: Recupere as propriedades e as relações de um objeto reviewSet.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 220a52d7ceb7a3b5fce766a9ec98dbe9c7bf308b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044694"
---
# <a name="get-reviewset"></a><span data-ttu-id="820dd-103">Obter reviewSet</span><span class="sxs-lookup"><span data-stu-id="820dd-103">Get reviewSet</span></span>

<span data-ttu-id="820dd-104">Namespace: microsoft.graph.ediscovery.ediscovery</span><span class="sxs-lookup"><span data-stu-id="820dd-104">Namespace: microsoft.graph.ediscovery.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="820dd-105">Recupere as propriedades e as relações de um [objeto reviewSet.](../resources/ediscovery-reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="820dd-105">Retrieve the properties and relationships of a [reviewSet](../resources/ediscovery-reviewset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="820dd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="820dd-106">Permissions</span></span>

<span data-ttu-id="820dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="820dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="820dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="820dd-109">Permission type</span></span>|<span data-ttu-id="820dd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="820dd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="820dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="820dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="820dd-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="820dd-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="820dd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="820dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="820dd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="820dd-114">Not supported.</span></span>|
|<span data-ttu-id="820dd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="820dd-115">Application</span></span>|<span data-ttu-id="820dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="820dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="820dd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="820dd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="820dd-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="820dd-118">Optional query parameters</span></span>

<span data-ttu-id="820dd-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="820dd-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="820dd-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="820dd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="820dd-121">Por padrão, todos os campos do conjunto de revisão são retornados; no entanto, você pode especificar determinados campos a retornar usando o parâmetro `$select` de consulta OData.</span><span class="sxs-lookup"><span data-stu-id="820dd-121">By default, all review set fields are returned; however, you can specify certain fields to return using the OData `$select` query parameter.</span></span>  <span data-ttu-id="820dd-122">Por exemplo, para retornar somente **o displayName** e a ID, adicione o seguinte à sua consulta: `$select=displayName,Id` .</span><span class="sxs-lookup"><span data-stu-id="820dd-122">For example, to only return the **displayName** and ID, add the following to your query: `$select=displayName,Id`.</span></span>

<span data-ttu-id="820dd-123">Como uma solicitação pode retornar muitos casos, você pode filtre-as usando **displayName**.</span><span class="sxs-lookup"><span data-stu-id="820dd-123">Because a request can return many cases, you can filter them by using **displayName**.</span></span>  <span data-ttu-id="820dd-124">Para filtrar **por displayName,** adicione o seguinte à consulta: , onde o nome do conjunto de revisão `$filter=displayName eq 'rs1'` é rs1.</span><span class="sxs-lookup"><span data-stu-id="820dd-124">To filter by **displayName**, add the following to your query: `$filter=displayName eq 'rs1'`, where the review set name is rs1.</span></span>

<span data-ttu-id="820dd-125">Para obter mais informações sobre como filtrar e especificar campos, consulte [Using Filter Expressions in OData URIs ](/dynamics-nav/using-filter-expressions-in-odata-uris).</span><span class="sxs-lookup"><span data-stu-id="820dd-125">For more information about filtering and specifying fields, see [Using Filter Expressions in OData URIs ](/dynamics-nav/using-filter-expressions-in-odata-uris).</span></span>

## <a name="request-headers"></a><span data-ttu-id="820dd-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="820dd-126">Request headers</span></span>

| <span data-ttu-id="820dd-127">Nome</span><span class="sxs-lookup"><span data-stu-id="820dd-127">Name</span></span>      |<span data-ttu-id="820dd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="820dd-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="820dd-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="820dd-129">Authorization</span></span> | <span data-ttu-id="820dd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="820dd-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="820dd-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="820dd-132">Request body</span></span>

<span data-ttu-id="820dd-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="820dd-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="820dd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="820dd-134">Response</span></span>

<span data-ttu-id="820dd-135">Se tiver êxito, este método retornará um código de resposta e o objeto `200 OK` [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="820dd-135">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="820dd-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="820dd-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="820dd-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="820dd-137">Request</span></span>

<span data-ttu-id="820dd-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="820dd-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="820dd-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="820dd-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets/0157910c-57ce-4e48-bd4b-90f3c88ca32e
```
# <a name="c"></a>[<span data-ttu-id="820dd-140">C#</span><span class="sxs-lookup"><span data-stu-id="820dd-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="820dd-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="820dd-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="820dd-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="820dd-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="820dd-143">Java</span><span class="sxs-lookup"><span data-stu-id="820dd-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="820dd-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="820dd-144">Response</span></span>

<span data-ttu-id="820dd-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="820dd-145">The following is an example of the response.</span></span>

> <span data-ttu-id="820dd-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="820dd-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
