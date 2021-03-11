---
title: 'reviewSet: addToReviewSet'
description: Inicie o processo de adição de uma coleção de serviços do Microsoft 365 a um conjunto de revisão.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 4eb0a7c2de533332c57f3e26d3b6fba25a68259d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720372"
---
# <a name="reviewset-addtoreviewset"></a><span data-ttu-id="e60cb-103">reviewSet: addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="e60cb-103">reviewSet: addToReviewSet</span></span>

<span data-ttu-id="e60cb-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e60cb-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e60cb-105">Inicie o processo de adição de uma coleção de serviços do Microsoft 365 a um conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="e60cb-105">Start the process of adding a collection from Microsoft 365 services to a review set.</span></span> <span data-ttu-id="e60cb-106">Depois que a operação for criada, você poderá obter o status da operação recuperando o parâmetro `Location` dos headers de resposta.</span><span class="sxs-lookup"><span data-stu-id="e60cb-106">After the operation is created, you can get the status of the operation by retrieving the `Location` parameter from the response headers.</span></span> <span data-ttu-id="e60cb-107">O local fornece uma URL que retornará [caseExportOperation](../resources/ediscovery-caseexportoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e60cb-107">The location provides a URL that will return a [caseExportOperation](../resources/ediscovery-caseexportoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e60cb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e60cb-108">Permissions</span></span>

<span data-ttu-id="e60cb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e60cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e60cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e60cb-111">Permission type</span></span>|<span data-ttu-id="e60cb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e60cb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e60cb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e60cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e60cb-114">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e60cb-114">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e60cb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e60cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e60cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e60cb-116">Not supported.</span></span>|
|<span data-ttu-id="e60cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e60cb-117">Application</span></span>|<span data-ttu-id="e60cb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e60cb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e60cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e60cb-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewsetId}/addToReviewSet
```

## <a name="request-headers"></a><span data-ttu-id="e60cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e60cb-120">Request headers</span></span>

|<span data-ttu-id="e60cb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e60cb-121">Name</span></span>|<span data-ttu-id="e60cb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e60cb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e60cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e60cb-123">Authorization</span></span>|<span data-ttu-id="e60cb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e60cb-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e60cb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e60cb-126">Content-Type</span></span>|<span data-ttu-id="e60cb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e60cb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e60cb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e60cb-129">Request body</span></span>

<span data-ttu-id="e60cb-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e60cb-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e60cb-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e60cb-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e60cb-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e60cb-132">Parameter</span></span>|<span data-ttu-id="e60cb-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e60cb-133">Type</span></span>|<span data-ttu-id="e60cb-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e60cb-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e60cb-135">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="e60cb-135">sourceCollection</span></span>|[<span data-ttu-id="e60cb-136">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="e60cb-136">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="e60cb-137">A ID da **sourceCollection**.</span><span class="sxs-lookup"><span data-stu-id="e60cb-137">The ID of the **sourceCollection**.</span></span>|
|<span data-ttu-id="e60cb-138">additionalData</span><span class="sxs-lookup"><span data-stu-id="e60cb-138">additionalData</span></span>|[<span data-ttu-id="e60cb-139">microsoft.graph.ediscovery.dataCollectionScope</span><span class="sxs-lookup"><span data-stu-id="e60cb-139">microsoft.graph.ediscovery.dataCollectionScope</span></span>](../resources/ediscovery-addtoreviewsetoperation.md#datacollectionscope-values)|<span data-ttu-id="e60cb-140">O **dataCollectionScope** que será incluído na coleção.</span><span class="sxs-lookup"><span data-stu-id="e60cb-140">The **dataCollectionScope** that will be included with the collection.</span></span>|

## <a name="response"></a><span data-ttu-id="e60cb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e60cb-141">Response</span></span>

<span data-ttu-id="e60cb-142">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="e60cb-142">If successful, this action returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e60cb-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e60cb-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e60cb-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e60cb-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "reviewset_addtoreviewset"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/080e8cad-f21f-4452-8826-0ddf7e949fdd/reviewSets/6fe25d32-8167-4625-b75c-c4181ccbd9d5/addToReviewSet
Content-Type: application/json
Content-length: 531

{
    "sourceCollection": {
        "id": "1a9b4145d8f84e39bc45a7f68c5c5119"
    },
    "additionalData": "linkedFiles"
}
```

### <a name="response"></a><span data-ttu-id="e60cb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e60cb-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```
