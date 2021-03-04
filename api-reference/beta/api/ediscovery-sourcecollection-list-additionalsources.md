---
title: Listar additionalSources
description: Obter uma lista de objetos dataSource adicionais associados a uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5f9c08fe286be1dd983fa81a4b9ee9b61563b503
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445749"
---
# <a name="list-additionalsources"></a><span data-ttu-id="451c3-103">Listar additionalSources</span><span class="sxs-lookup"><span data-stu-id="451c3-103">List additionalSources</span></span>

<span data-ttu-id="451c3-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="451c3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="451c3-105">Obter uma lista de [objetos dataSource adicionais](../resources/ediscovery-datasource.md) associados a uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="451c3-105">Get a list of additional [dataSource](../resources/ediscovery-datasource.md) objects associated with a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="451c3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="451c3-106">Permissions</span></span>

<span data-ttu-id="451c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="451c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="451c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="451c3-109">Permission type</span></span>|<span data-ttu-id="451c3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="451c3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="451c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="451c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="451c3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="451c3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="451c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="451c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="451c3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="451c3-114">Not supported.</span></span>|
|<span data-ttu-id="451c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="451c3-115">Application</span></span>|<span data-ttu-id="451c3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="451c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="451c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="451c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="451c3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="451c3-118">Optional query parameters</span></span>

<span data-ttu-id="451c3-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="451c3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="451c3-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="451c3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="451c3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="451c3-121">Request headers</span></span>

|<span data-ttu-id="451c3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="451c3-122">Name</span></span>|<span data-ttu-id="451c3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="451c3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="451c3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="451c3-124">Authorization</span></span>|<span data-ttu-id="451c3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="451c3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="451c3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="451c3-127">Request body</span></span>

<span data-ttu-id="451c3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="451c3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="451c3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="451c3-129">Response</span></span>

<span data-ttu-id="451c3-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="451c3-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="451c3-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="451c3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="451c3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="451c3-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

### <a name="response"></a><span data-ttu-id="451c3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="451c3-133">Response</span></span>

<span data-ttu-id="451c3-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="451c3-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
