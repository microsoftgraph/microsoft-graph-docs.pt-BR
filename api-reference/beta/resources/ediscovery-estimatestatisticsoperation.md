---
title: Tipo de recurso estimateStatisticsOperation
description: Representa a operação que lida com a estimativa da contagem e do tamanho de uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e816ba01d4bb648a8e78b5b96369236f63fb163e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445928"
---
# <a name="estimatestatisticsoperation-resource-type"></a><span data-ttu-id="2336d-103">Tipo de recurso estimateStatisticsOperation</span><span class="sxs-lookup"><span data-stu-id="2336d-103">estimateStatisticsOperation resource type</span></span>

<span data-ttu-id="2336d-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2336d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2336d-105">Representa a operação que lida com a estimativa da contagem e do tamanho de [uma sourceCollection](../resources/ediscovery-sourcecollection.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-105">Represents the operation that handles estimating the count and size of a [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span> <span data-ttu-id="2336d-106">Para obter detalhes, [consulte Coletar dados para uma ocorrência em Descoberta Avançada de eDiscovery](/microsoft-365/compliance/collecting-data-for-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="2336d-106">For details, see [Collect data for a case in Advanced eDiscovery](/microsoft-365/compliance/collecting-data-for-ediscovery).</span></span>

<span data-ttu-id="2336d-107">Herda de [caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-107">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2336d-108">Methods</span><span class="sxs-lookup"><span data-stu-id="2336d-108">Methods</span></span>

<span data-ttu-id="2336d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2336d-109">None.</span></span>

## <a name="properties"></a><span data-ttu-id="2336d-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2336d-110">Properties</span></span>

|<span data-ttu-id="2336d-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2336d-111">Property</span></span>|<span data-ttu-id="2336d-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="2336d-112">Type</span></span>|<span data-ttu-id="2336d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2336d-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2336d-114">ação</span><span class="sxs-lookup"><span data-stu-id="2336d-114">action</span></span>|<span data-ttu-id="2336d-115">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="2336d-115">microsoft.graph.ediscovery.caseAction</span></span>| <span data-ttu-id="2336d-116">O tipo de operação.</span><span class="sxs-lookup"><span data-stu-id="2336d-116">The type of operation.</span></span> <span data-ttu-id="2336d-117">A ação de caso dessa entidade sempre será `estimateStatistics` .</span><span class="sxs-lookup"><span data-stu-id="2336d-117">The case action for this entity will always be `estimateStatistics`.</span></span> <span data-ttu-id="2336d-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2336d-118">Read-only.</span></span> <span data-ttu-id="2336d-119">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-119">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="2336d-120">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2336d-120">completedDateTime</span></span>|<span data-ttu-id="2336d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2336d-121">DateTimeOffset</span></span>|<span data-ttu-id="2336d-122">A data e a hora em que a operação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="2336d-122">The date and time the operation was completed.</span></span> <span data-ttu-id="2336d-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2336d-123">Read-only.</span></span> <span data-ttu-id="2336d-124">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-124">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="2336d-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="2336d-125">createdBy</span></span>|[<span data-ttu-id="2336d-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="2336d-126">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="2336d-127">O usuário que criou a operação.</span><span class="sxs-lookup"><span data-stu-id="2336d-127">The user who created the operation.</span></span> <span data-ttu-id="2336d-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2336d-128">Read-only.</span></span> <span data-ttu-id="2336d-129">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-129">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="2336d-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2336d-130">createdDateTime</span></span>|<span data-ttu-id="2336d-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2336d-131">DateTimeOffset</span></span>|<span data-ttu-id="2336d-132">A data e a hora em que a operação foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="2336d-132">The date and time the operation was started.</span></span> <span data-ttu-id="2336d-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2336d-133">Read-only.</span></span> <span data-ttu-id="2336d-134">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-134">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="2336d-135">id</span><span class="sxs-lookup"><span data-stu-id="2336d-135">id</span></span>|<span data-ttu-id="2336d-136">String</span><span class="sxs-lookup"><span data-stu-id="2336d-136">String</span></span>| <span data-ttu-id="2336d-137">A ID da operação.</span><span class="sxs-lookup"><span data-stu-id="2336d-137">The ID for the operation.</span></span> <span data-ttu-id="2336d-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2336d-138">Read-only.</span></span> <span data-ttu-id="2336d-139">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-139">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="2336d-140">indexedItemCount</span><span class="sxs-lookup"><span data-stu-id="2336d-140">indexedItemCount</span></span>|<span data-ttu-id="2336d-141">Int64</span><span class="sxs-lookup"><span data-stu-id="2336d-141">Int64</span></span>|<span data-ttu-id="2336d-142">A contagem estimada de itens para **o sourceCollection** que corresponderam à consulta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2336d-142">The estimated count of items for the **sourceCollection** that matched the content query.</span></span>|
|<span data-ttu-id="2336d-143">indexedItemsSize</span><span class="sxs-lookup"><span data-stu-id="2336d-143">indexedItemsSize</span></span>|<span data-ttu-id="2336d-144">Int64</span><span class="sxs-lookup"><span data-stu-id="2336d-144">Int64</span></span>|<span data-ttu-id="2336d-145">O tamanho estimado de itens para **o sourceCollection** que corresponderam à consulta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2336d-145">The estimated size of items for the **sourceCollection** that matched the content query.</span></span>|
|<span data-ttu-id="2336d-146">mailboxCount</span><span class="sxs-lookup"><span data-stu-id="2336d-146">mailboxCount</span></span>|<span data-ttu-id="2336d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2336d-147">Int32</span></span>|<span data-ttu-id="2336d-148">O número de caixas de correio que tiveram visitas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2336d-148">The number of mailboxes that had search hits.</span></span>|
|<span data-ttu-id="2336d-149">percentProgress</span><span class="sxs-lookup"><span data-stu-id="2336d-149">percentProgress</span></span>|<span data-ttu-id="2336d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2336d-150">Int32</span></span>|<span data-ttu-id="2336d-151">O progresso da operação.</span><span class="sxs-lookup"><span data-stu-id="2336d-151">The progress of the operation.</span></span> <span data-ttu-id="2336d-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2336d-152">Read-only.</span></span> <span data-ttu-id="2336d-153">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-153">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="2336d-154">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2336d-154">resultInfo</span></span>|[<span data-ttu-id="2336d-155">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2336d-155">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="2336d-156">Contém informações de resultados específicas de falha e sucesso.</span><span class="sxs-lookup"><span data-stu-id="2336d-156">Contains success and failure-specific result information.</span></span> <span data-ttu-id="2336d-157">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-157">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="2336d-158">siteCount</span><span class="sxs-lookup"><span data-stu-id="2336d-158">siteCount</span></span>|<span data-ttu-id="2336d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2336d-159">Int32</span></span>|<span data-ttu-id="2336d-160">O número de caixas de correio que tiveram visitas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2336d-160">The number of mailboxes that had search hits.</span></span>|
|<span data-ttu-id="2336d-161">status</span><span class="sxs-lookup"><span data-stu-id="2336d-161">status</span></span>|[<span data-ttu-id="2336d-162">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="2336d-162">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="2336d-163">O status da operação de caso.</span><span class="sxs-lookup"><span data-stu-id="2336d-163">The status of the case operation.</span></span> <span data-ttu-id="2336d-164">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2336d-164">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="2336d-165">Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2336d-165">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|
|<span data-ttu-id="2336d-166">unindexedItemCount</span><span class="sxs-lookup"><span data-stu-id="2336d-166">unindexedItemCount</span></span>|<span data-ttu-id="2336d-167">Int64</span><span class="sxs-lookup"><span data-stu-id="2336d-167">Int64</span></span>|<span data-ttu-id="2336d-168">A contagem estimada de itens não índicedos para a coleção.</span><span class="sxs-lookup"><span data-stu-id="2336d-168">The estimated count of unindexed items for the collection.</span></span>|
|<span data-ttu-id="2336d-169">unindexedItemsSize</span><span class="sxs-lookup"><span data-stu-id="2336d-169">unindexedItemsSize</span></span>|<span data-ttu-id="2336d-170">Int64</span><span class="sxs-lookup"><span data-stu-id="2336d-170">Int64</span></span>|<span data-ttu-id="2336d-171">O tamanho estimado de itens não índicedos para a coleção.</span><span class="sxs-lookup"><span data-stu-id="2336d-171">The estimated size of unindexed items for the collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2336d-172">Relações</span><span class="sxs-lookup"><span data-stu-id="2336d-172">Relationships</span></span>

|<span data-ttu-id="2336d-173">Relação</span><span class="sxs-lookup"><span data-stu-id="2336d-173">Relationship</span></span>|<span data-ttu-id="2336d-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="2336d-174">Type</span></span>|<span data-ttu-id="2336d-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="2336d-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2336d-176">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="2336d-176">sourceCollection</span></span>|[<span data-ttu-id="2336d-177">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="2336d-177">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="2336d-178">Coleção eDiscovery, comumente conhecida como pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2336d-178">eDiscovery collection, commonly known as a search.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2336d-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2336d-179">JSON representation</span></span>

<span data-ttu-id="2336d-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2336d-180">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.estimateStatisticsOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/$entity",
    "@odata.type": "#microsoft.graph.ediscovery.estimateStatisticsOperation",
    "createdDateTime": "2021-01-12T18:47:23.3974907Z",
    "completedDateTime": "2021-01-12T18:47:51.1461805Z",
    "percentProgress": 100,
    "status": "succeeded",
    "action": "estimateStatistics",
    "id": "82edd40e182a464fa02c24a36fa94873",
    "indexedItemCount": 2,
    "indexedItemsSize": 39276,
    "unindexedItemCount": 0,
    "unindexedItemsSize": 0,
    "mailboxCount": 1,
    "siteCount": 0,
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
