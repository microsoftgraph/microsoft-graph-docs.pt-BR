---
title: Listar additionalSources
description: Obter uma lista de objetos dataSource adicionais associados a uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0e0d48253e93095176c5a45d78d6c155a9b02bd1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952145"
---
# <a name="list-additionalsources"></a><span data-ttu-id="b5e8b-103">Listar additionalSources</span><span class="sxs-lookup"><span data-stu-id="b5e8b-103">List additionalSources</span></span>

<span data-ttu-id="b5e8b-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b5e8b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5e8b-105">Obter uma lista de [objetos dataSource adicionais](../resources/ediscovery-datasource.md) associados a uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="b5e8b-105">Get a list of additional [dataSource](../resources/ediscovery-datasource.md) objects associated with a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e8b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5e8b-106">Permissions</span></span>

<span data-ttu-id="b5e8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5e8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5e8b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5e8b-109">Permission type</span></span>|<span data-ttu-id="b5e8b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5e8b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5e8b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5e8b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b5e8b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e8b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b5e8b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5e8b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5e8b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5e8b-114">Not supported.</span></span>|
|<span data-ttu-id="b5e8b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5e8b-115">Application</span></span>|<span data-ttu-id="b5e8b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5e8b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5e8b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e8b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5e8b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5e8b-118">Optional query parameters</span></span>

<span data-ttu-id="b5e8b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b5e8b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b5e8b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b5e8b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5e8b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5e8b-121">Request headers</span></span>

|<span data-ttu-id="b5e8b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b5e8b-122">Name</span></span>|<span data-ttu-id="b5e8b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5e8b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b5e8b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5e8b-124">Authorization</span></span>|<span data-ttu-id="b5e8b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5e8b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5e8b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5e8b-127">Request body</span></span>

<span data-ttu-id="b5e8b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5e8b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5e8b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5e8b-129">Response</span></span>

<span data-ttu-id="b5e8b-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5e8b-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5e8b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b5e8b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b5e8b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5e8b-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b5e8b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e8b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_datasource_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```
# <a name="c"></a>[<span data-ttu-id="b5e8b-134">C#</span><span class="sxs-lookup"><span data-stu-id="b5e8b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-datasource-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5e8b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5e8b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-datasource-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5e8b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5e8b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-datasource-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5e8b-137">Java</span><span class="sxs-lookup"><span data-stu-id="b5e8b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-datasource-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b5e8b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5e8b-138">Response</span></span>

<span data-ttu-id="b5e8b-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b5e8b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.dataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.dataSource",
      "id": "0fb67fc5-7fc5-0fb6-c57f-b60fc57fb60f",
      "displayName": "String",
      "createdDateTime": "String (timestamp)",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ]
}
```
