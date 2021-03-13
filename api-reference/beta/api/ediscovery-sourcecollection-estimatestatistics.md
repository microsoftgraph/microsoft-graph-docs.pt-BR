---
title: 'sourceCollection: estimateStatistics'
description: Executa uma estimativa da coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2ae6b7363bdb1be34e38dd7f5502962fc920808d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772706"
---
# <a name="sourcecollection-estimatestatistics"></a><span data-ttu-id="14331-103">sourceCollection: estimateStatistics</span><span class="sxs-lookup"><span data-stu-id="14331-103">sourceCollection: estimateStatistics</span></span>

<span data-ttu-id="14331-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="14331-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14331-105">Execute uma estimativa do número de emails e documentos na coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="14331-105">Run an estimate of the number of emails and documents in the source collection.</span></span> <span data-ttu-id="14331-106">Para saber mais sobre coleções de origem (também conhecidas como pesquisas na Descoberta eDiscovery), consulte Coletar dados para uma ocorrência em [Descoberta Avançada em Descoberta Externa](https://docs.microsoft.com/microsoft-365/compliance/collecting-data-for-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="14331-106">To learn more about source collections (also known as searches in eDiscovery), see [Collect data for a case in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/collecting-data-for-ediscovery).</span></span>

## <a name="permissions"></a><span data-ttu-id="14331-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="14331-107">Permissions</span></span>

<span data-ttu-id="14331-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14331-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14331-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14331-110">Permission type</span></span>|<span data-ttu-id="14331-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14331-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14331-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14331-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14331-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14331-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="14331-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14331-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14331-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14331-115">Not supported.</span></span>|
|<span data-ttu-id="14331-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14331-116">Application</span></span>|<span data-ttu-id="14331-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14331-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14331-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14331-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```

## <a name="request-headers"></a><span data-ttu-id="14331-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14331-119">Request headers</span></span>

|<span data-ttu-id="14331-120">Nome</span><span class="sxs-lookup"><span data-stu-id="14331-120">Name</span></span>|<span data-ttu-id="14331-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="14331-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="14331-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14331-122">Authorization</span></span>|<span data-ttu-id="14331-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14331-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14331-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14331-125">Request body</span></span>

<span data-ttu-id="14331-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14331-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14331-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="14331-127">Response</span></span>

<span data-ttu-id="14331-128">Se a estimativa for iniciada com êxito, essa ação retornará um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="14331-128">If the estimate is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="14331-129">A resposta também conterá um header, que contém o local da `Location` [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) que foi criada para manipular a estimativa.</span><span class="sxs-lookup"><span data-stu-id="14331-129">The response will also contain a `Location` header, which contains the location of the [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) that was created to handle the estimate.</span></span> <span data-ttu-id="14331-130">Verifique o status da operação de estimativa fazendo uma solicitação GET para o local, quando concluído com êxito, o [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) será alterado para `succeeded` .</span><span class="sxs-lookup"><span data-stu-id="14331-130">Check the status of the estimate operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="14331-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14331-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14331-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14331-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="14331-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="14331-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sourcecollection_estimatestatistics"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```
# <a name="c"></a>[<span data-ttu-id="14331-134">C#</span><span class="sxs-lookup"><span data-stu-id="14331-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sourcecollection-estimatestatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14331-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14331-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sourcecollection-estimatestatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14331-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14331-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sourcecollection-estimatestatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14331-137">Java</span><span class="sxs-lookup"><span data-stu-id="14331-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sourcecollection-estimatestatistics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14331-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="14331-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: private
client-request-id: af32de50-99d9-e3a8-371b-a4f366cc78e7
content-length: 0
content-type: text/plain
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/82edd40e182a464fa02c24a36fa94873
request-id: e890176f-640f-4222-9cd8-be26e71c5e5d
```
