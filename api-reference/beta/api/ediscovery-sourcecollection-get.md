---
title: Obter sourceCollection
description: Leia as propriedades e as relações de um objeto sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b10f29de6bbf61151f55aae2a37ac10ddf3ece86
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445751"
---
# <a name="get-sourcecollection"></a><span data-ttu-id="ad4c5-103">Obter sourceCollection</span><span class="sxs-lookup"><span data-stu-id="ad4c5-103">Get sourceCollection</span></span>

<span data-ttu-id="ad4c5-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ad4c5-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad4c5-105">Leia as propriedades e as relações de um [objeto sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="ad4c5-105">Read the properties and relationships of a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad4c5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad4c5-106">Permissions</span></span>

<span data-ttu-id="ad4c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad4c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad4c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad4c5-109">Permission type</span></span>|<span data-ttu-id="ad4c5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad4c5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad4c5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad4c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad4c5-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4c5-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="ad4c5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad4c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad4c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad4c5-114">Not supported.</span></span>|
|<span data-ttu-id="ad4c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad4c5-115">Application</span></span>|<span data-ttu-id="ad4c5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad4c5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad4c5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad4c5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad4c5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ad4c5-118">Optional query parameters</span></span>

<span data-ttu-id="ad4c5-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ad4c5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ad4c5-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ad4c5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="ad4c5-121">Use `$expand` para expandir operações de conjunto de revisão, fontes de custodia e a última operação de estatísticas de estimativa.</span><span class="sxs-lookup"><span data-stu-id="ad4c5-121">Use `$expand` to expand review set operations, custodian sources, and the last estimate statistics operation.</span></span>

```http
https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```

## <a name="request-headers"></a><span data-ttu-id="ad4c5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad4c5-122">Request headers</span></span>

|<span data-ttu-id="ad4c5-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ad4c5-123">Name</span></span>|<span data-ttu-id="ad4c5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad4c5-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ad4c5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad4c5-125">Authorization</span></span>|<span data-ttu-id="ad4c5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad4c5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad4c5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad4c5-128">Request body</span></span>

<span data-ttu-id="ad4c5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad4c5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad4c5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad4c5-130">Response</span></span>

<span data-ttu-id="ad4c5-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad4c5-131">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad4c5-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ad4c5-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ad4c5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad4c5-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```

### <a name="response"></a><span data-ttu-id="ad4c5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad4c5-134">Response</span></span>

<span data-ttu-id="ad4c5-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ad4c5-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/sourceCollections/$entity",
    "description": null,
    "lastModifiedDateTime": "2021-01-12T18:09:03.7378679Z",
    "contentQuery": "subject:'Quarterly Financials'",
    "tenantSources": "none",
    "id": "1a9b4145d8f84e39bc45a7f68c5c5119",
    "displayName": "Quarterly Financials search",
    "createdDateTime": "2021-01-12T18:09:03.417009Z",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.onmicrosoft.com"
        }
    },
    "addToReviewSetOperation": {
        "createdDateTime": "2021-01-13T05:38:49.9186654Z",
        "completedDateTime": "2021-01-13T07:54:45.0007868Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "addToReviewSet",
        "id": "aef586b34d89405d802497658a14194f",
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": null,
                "userPrincipalName": "admin@contoso.com"
            }
        }
    },
    "lastEstimateStatisticsOperation": {
        "createdDateTime": "2021-01-12T21:53:50.7272654Z",
        "completedDateTime": "2021-01-12T21:54:49.5595543Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "estimateStatistics",
        "id": "f3db0382af0842eaa98c7dd59e7dace6",
        "indexedItemCount": 39598,
        "indexedItemsSize": 3760920737,
        "unindexedItemCount": 0,
        "unindexedItemsSize": 0,
        "mailboxCount": 1,
        "siteCount": 1,
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": "EDisco Admin",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    }
}
```
