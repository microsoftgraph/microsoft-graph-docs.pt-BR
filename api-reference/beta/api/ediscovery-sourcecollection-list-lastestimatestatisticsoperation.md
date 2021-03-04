---
title: Listar estimateStatisticsOperation
description: Obter o último objeto estimateStatisticsOperation associado a uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c7a8c02e5401ee7a1f6f513004357db1998a4cf3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445745"
---
# <a name="list-estimatestatisticsoperation"></a><span data-ttu-id="a700c-103">Listar estimateStatisticsOperation</span><span class="sxs-lookup"><span data-stu-id="a700c-103">List estimateStatisticsOperation</span></span>

<span data-ttu-id="a700c-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a700c-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a700c-105">Obter o último [objeto estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) associado a uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="a700c-105">Get the last [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) object associated with a source collection.</span></span> 

><span data-ttu-id="a700c-106">**Observação:** Este método lista apenas a última operação; ele não retorna um histórico de todas as operações.</span><span class="sxs-lookup"><span data-stu-id="a700c-106">**Note:** This method only lists the last operation; it does not return a history of all operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="a700c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a700c-107">Permissions</span></span>

<span data-ttu-id="a700c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a700c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a700c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a700c-110">Permission type</span></span>|<span data-ttu-id="a700c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a700c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a700c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a700c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a700c-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a700c-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a700c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a700c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a700c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a700c-115">Not supported.</span></span>|
|<span data-ttu-id="a700c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a700c-116">Application</span></span>|<span data-ttu-id="a700c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a700c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a700c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a700c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/lastEstimateStatisticsOperation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a700c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a700c-119">Optional query parameters</span></span>

<span data-ttu-id="a700c-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a700c-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a700c-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a700c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a700c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a700c-122">Request headers</span></span>

|<span data-ttu-id="a700c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a700c-123">Name</span></span>|<span data-ttu-id="a700c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a700c-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a700c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a700c-125">Authorization</span></span>|<span data-ttu-id="a700c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a700c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a700c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a700c-128">Request body</span></span>

<span data-ttu-id="a700c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a700c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a700c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a700c-130">Response</span></span>

<span data-ttu-id="a700c-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a700c-131">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a700c-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a700c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a700c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a700c-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_estimatestatisticsoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/95bdbf84f02f4bdaafbbb2fe945a4962/lastEstimateStatisticsOperation
```

### <a name="response"></a><span data-ttu-id="a700c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a700c-134">Response</span></span>

<span data-ttu-id="a700c-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a700c-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.estimateStatisticsOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "createdDateTime": "2021-01-12T20:12:01.4443402Z",
        "completedDateTime": "2021-01-12T20:12:35.4818899Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "estimateStatistics",
        "id": "95bdbf84f02f4bdaafbbb2fe945a4962",
        "indexedItemCount": 3,
        "indexedItemsSize": 68848,
        "unindexedItemCount": 0,
        "unindexedItemsSize": 0,
        "mailboxCount": 2,
        "siteCount": 0
    }
  ]
}
```
