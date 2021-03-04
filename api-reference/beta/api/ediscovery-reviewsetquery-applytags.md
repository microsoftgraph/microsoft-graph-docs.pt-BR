---
title: 'reviewSetQuery: applyTags'
description: Aplique marcas a documentos que corresponderem à consulta especificada.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2c3f41d1fbe9851babc582c1f21c9f9673d53541
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445771"
---
# <a name="reviewsetquery-applytags"></a><span data-ttu-id="c7442-103">reviewSetQuery: applyTags</span><span class="sxs-lookup"><span data-stu-id="c7442-103">reviewSetQuery: applyTags</span></span>

<span data-ttu-id="c7442-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c7442-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="c7442-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7442-105">Permissions</span></span>

<span data-ttu-id="c7442-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7442-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7442-108">Permission type</span></span>|<span data-ttu-id="c7442-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7442-109">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7442-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7442-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c7442-111">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7442-111">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c7442-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7442-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7442-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7442-113">Not supported.</span></span>|
|<span data-ttu-id="c7442-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7442-114">Application</span></span>|<span data-ttu-id="c7442-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7442-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7442-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7442-116">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewSetId}/queries/{reviewSetQueryId}/applyTags
```

## <a name="request-headers"></a><span data-ttu-id="c7442-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7442-117">Request headers</span></span>

|<span data-ttu-id="c7442-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c7442-118">Name</span></span>|<span data-ttu-id="c7442-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7442-119">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7442-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7442-120">Authorization</span></span>|<span data-ttu-id="c7442-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7442-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c7442-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7442-123">Content-Type</span></span>|<span data-ttu-id="c7442-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7442-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7442-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7442-126">Request body</span></span>

<span data-ttu-id="c7442-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c7442-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c7442-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c7442-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c7442-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c7442-129">Parameter</span></span>|<span data-ttu-id="c7442-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7442-130">Type</span></span>|<span data-ttu-id="c7442-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7442-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7442-132">tagsToAdd</span><span class="sxs-lookup"><span data-stu-id="c7442-132">tagsToAdd</span></span>|<span data-ttu-id="c7442-133">[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="c7442-133">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="c7442-134">IDs de marcas para adicionar aos documentos que corresponderem à consulta.</span><span class="sxs-lookup"><span data-stu-id="c7442-134">IDs of tags to add to the documents that match the query.</span></span>|
|<span data-ttu-id="c7442-135">tagsToRemove</span><span class="sxs-lookup"><span data-stu-id="c7442-135">tagsToRemove</span></span>|<span data-ttu-id="c7442-136">[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="c7442-136">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="c7442-137">IDs das marcas a remover dos documentos que corresponderem à consulta.</span><span class="sxs-lookup"><span data-stu-id="c7442-137">IDs of tags to remove from the documents that match the query.</span></span>|

## <a name="response"></a><span data-ttu-id="c7442-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7442-138">Response</span></span>

<span data-ttu-id="c7442-139">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="c7442-139">If successful, this action returns a `202 Accepted` response code.</span></span>

<span data-ttu-id="c7442-140">Se a operação de marcação for iniciada com êxito, essa ação retornará um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7442-140">If the tagging operation is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="c7442-141">A resposta também conterá um header, que contém o local da `Location` [tagOperation](../resources/ediscovery-tagOperation.md) que foi criada para manipular a marcação.</span><span class="sxs-lookup"><span data-stu-id="c7442-141">The response will also contain a `Location` header, which contains the location of the [tagOperation](../resources/ediscovery-tagOperation.md) that was created to handle the tagging.</span></span> <span data-ttu-id="c7442-142">Verifique o status da operação de marcação fazendo uma solicitação GET para o local, quando concluído com êxito, o [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) mudará para `succeeded` .</span><span class="sxs-lookup"><span data-stu-id="c7442-142">Check the status of the tagging operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="c7442-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c7442-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7442-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7442-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "reviewsetquery_applytags"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/reviewsets/6c95c2a6-31fa-45a8-93ef-dd4531974783/queries/b4798d14-748d-468e-a1ec-96a2b1d49677/applyTags
Content-Type: application/json
Content-length: 778

{
    "tagsToAdd": [
        {
            "id": "b4798d14-748d-468e-a1ec-96a2b1d49677"
        }
    ]
}
```

### <a name="response"></a><span data-ttu-id="c7442-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7442-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: no-cache,
client-request-id: 56c9dd8b-d8f7-59ae-6733-38191862c9c9,
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/operations('d77f7933e88842bab3221e280be9dc0b'),
request-id: c2397a81-e9c2-4851-b669-d87e0751e45a
```
