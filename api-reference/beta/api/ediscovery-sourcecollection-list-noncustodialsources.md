---
title: Listar noncustodialSources
description: Obter os recursos nãocustodialDataSource da propriedade de navegação noncustodialSources.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 65f59c6694131ce5af98511af75e5424fb06a7ce
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240788"
---
# <a name="list-noncustodialsources"></a><span data-ttu-id="2f7a5-103">Listar noncustodialSources</span><span class="sxs-lookup"><span data-stu-id="2f7a5-103">List noncustodialSources</span></span>

<span data-ttu-id="2f7a5-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2f7a5-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f7a5-105">Obter uma lista [de noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) associado a [uma sourceCollection](../resources/ediscovery-sourcecollection.md).</span><span class="sxs-lookup"><span data-stu-id="2f7a5-105">Get a list of [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) associated with a [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="2f7a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f7a5-106">Permissions</span></span>

<span data-ttu-id="2f7a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f7a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f7a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f7a5-109">Permission type</span></span>|<span data-ttu-id="2f7a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f7a5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f7a5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f7a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f7a5-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f7a5-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="2f7a5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f7a5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f7a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f7a5-114">Not supported.</span></span>|
|<span data-ttu-id="2f7a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f7a5-115">Application</span></span>|<span data-ttu-id="2f7a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f7a5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f7a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f7a5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f7a5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f7a5-118">Optional query parameters</span></span>

<span data-ttu-id="2f7a5-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2f7a5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2f7a5-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2f7a5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f7a5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f7a5-121">Request headers</span></span>

|<span data-ttu-id="2f7a5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2f7a5-122">Name</span></span>|<span data-ttu-id="2f7a5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f7a5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2f7a5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f7a5-124">Authorization</span></span>|<span data-ttu-id="2f7a5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f7a5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f7a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f7a5-127">Request body</span></span>

<span data-ttu-id="2f7a5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f7a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f7a5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f7a5-129">Response</span></span>

<span data-ttu-id="2f7a5-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f7a5-130">If successful, this method returns a `200 OK` response code and a collection of [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f7a5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2f7a5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f7a5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f7a5-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2f7a5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f7a5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_noncustodialdatasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources
```
# <a name="c"></a>[<span data-ttu-id="2f7a5-134">C#</span><span class="sxs-lookup"><span data-stu-id="2f7a5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-noncustodialdatasource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f7a5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f7a5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-noncustodialdatasource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f7a5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f7a5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-noncustodialdatasource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f7a5-137">Java</span><span class="sxs-lookup"><span data-stu-id="2f7a5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-noncustodialdatasource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f7a5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f7a5-138">Response</span></span>

> <span data-ttu-id="2f7a5-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2f7a5-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.noncustodialDataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.ediscovery.noncustodialDataSource)",
    "value": [
        {
            "status": "0",
            "lastModifiedDateTime": "2021-04-07T16:45:49.625141Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "39383530323537383742433232433246",
            "displayName": "French fry closet",
            "createdDateTime": "2021-04-07T16:45:49.5761676Z",
            "applyHoldToSource": false
        }
    ]
}
```
