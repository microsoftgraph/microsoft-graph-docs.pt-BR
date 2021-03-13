---
title: Listar additionalSources
description: Obter uma lista de objetos dataSource adicionais associados a uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2cd723f3e527e477681224e0b59375099f5d36f7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50769607"
---
# <a name="list-additionalsources"></a><span data-ttu-id="1417e-103">Listar additionalSources</span><span class="sxs-lookup"><span data-stu-id="1417e-103">List additionalSources</span></span>

<span data-ttu-id="1417e-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="1417e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1417e-105">Obter uma lista de [objetos dataSource adicionais](../resources/ediscovery-datasource.md) associados a uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="1417e-105">Get a list of additional [dataSource](../resources/ediscovery-datasource.md) objects associated with a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="1417e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1417e-106">Permissions</span></span>

<span data-ttu-id="1417e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1417e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1417e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1417e-109">Permission type</span></span>|<span data-ttu-id="1417e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1417e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1417e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1417e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1417e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1417e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="1417e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1417e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1417e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1417e-114">Not supported.</span></span>|
|<span data-ttu-id="1417e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1417e-115">Application</span></span>|<span data-ttu-id="1417e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1417e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1417e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1417e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1417e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1417e-118">Optional query parameters</span></span>

<span data-ttu-id="1417e-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1417e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1417e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1417e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1417e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1417e-121">Request headers</span></span>

|<span data-ttu-id="1417e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1417e-122">Name</span></span>|<span data-ttu-id="1417e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1417e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1417e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1417e-124">Authorization</span></span>|<span data-ttu-id="1417e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1417e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1417e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1417e-127">Request body</span></span>

<span data-ttu-id="1417e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1417e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1417e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1417e-129">Response</span></span>

<span data-ttu-id="1417e-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1417e-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1417e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1417e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1417e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1417e-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1417e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1417e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```
# <a name="c"></a>[<span data-ttu-id="1417e-134">C#</span><span class="sxs-lookup"><span data-stu-id="1417e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-datasource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1417e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1417e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-datasource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1417e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1417e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-datasource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1417e-137">Java</span><span class="sxs-lookup"><span data-stu-id="1417e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-datasource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1417e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1417e-138">Response</span></span>

<span data-ttu-id="1417e-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1417e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
