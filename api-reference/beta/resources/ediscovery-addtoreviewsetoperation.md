---
title: Tipo de recurso addToReviewSetOperation
description: Adiciona os resultados de uma sourceCollection a um reviewSet
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d7323fbd6d2d068888d556328fc3ea4e399ab2fe
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446181"
---
# <a name="addtoreviewsetoperation-resource-type"></a><span data-ttu-id="3c5ea-103">Tipo de recurso addToReviewSetOperation</span><span class="sxs-lookup"><span data-stu-id="3c5ea-103">addToReviewSetOperation resource type</span></span>

<span data-ttu-id="3c5ea-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3c5ea-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c5ea-105">Representa uma operação para adicionar [uma sourceCollection](../resources/ediscovery-sourcecollection.md) a um [reviewSet](../resources/ediscovery-reviewset.md).</span><span class="sxs-lookup"><span data-stu-id="3c5ea-105">Represents an operation to add a [sourceCollection](../resources/ediscovery-sourcecollection.md) to a [reviewSet](../resources/ediscovery-reviewset.md).</span></span>

<span data-ttu-id="3c5ea-106">Herda de [caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3c5ea-106">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3c5ea-107">Methods</span><span class="sxs-lookup"><span data-stu-id="3c5ea-107">Methods</span></span>

<span data-ttu-id="3c5ea-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="3c5ea-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c5ea-109">Properties</span></span>

|<span data-ttu-id="3c5ea-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c5ea-110">Property</span></span>|<span data-ttu-id="3c5ea-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c5ea-111">Type</span></span>|<span data-ttu-id="3c5ea-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c5ea-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c5ea-113">ação</span><span class="sxs-lookup"><span data-stu-id="3c5ea-113">action</span></span>|[<span data-ttu-id="3c5ea-114">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="3c5ea-114">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="3c5ea-115">A ação de caso dessa entidade sempre será `addToReviewSet` .</span><span class="sxs-lookup"><span data-stu-id="3c5ea-115">The case action for this entity will always be `addToReviewSet`.</span></span> <span data-ttu-id="3c5ea-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-116">Read-only.</span></span> <span data-ttu-id="3c5ea-117">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3c5ea-117">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="3c5ea-118">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c5ea-118">completedDateTime</span></span>|<span data-ttu-id="3c5ea-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c5ea-119">DateTimeOffset</span></span>|<span data-ttu-id="3c5ea-120">A data e a hora em que a operação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-120">The date and time the operation was completed.</span></span> <span data-ttu-id="3c5ea-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-121">Read-only.</span></span> <span data-ttu-id="3c5ea-122">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="3c5ea-122">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="3c5ea-123">createdBy</span><span class="sxs-lookup"><span data-stu-id="3c5ea-123">createdBy</span></span>|[<span data-ttu-id="3c5ea-124">identitySet</span><span class="sxs-lookup"><span data-stu-id="3c5ea-124">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="3c5ea-125">O usuário que criou a operação.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-125">The user who created the operation.</span></span> <span data-ttu-id="3c5ea-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-126">Read-only.</span></span> <span data-ttu-id="3c5ea-127">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="3c5ea-127">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="3c5ea-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c5ea-128">createdDateTime</span></span>|<span data-ttu-id="3c5ea-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c5ea-129">DateTimeOffset</span></span>|<span data-ttu-id="3c5ea-130">A data e a hora em que a operação foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-130">The date and time the operation was started.</span></span> <span data-ttu-id="3c5ea-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-131">Read-only.</span></span> <span data-ttu-id="3c5ea-132">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="3c5ea-132">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="3c5ea-133">id</span><span class="sxs-lookup"><span data-stu-id="3c5ea-133">id</span></span>|<span data-ttu-id="3c5ea-134">String</span><span class="sxs-lookup"><span data-stu-id="3c5ea-134">String</span></span>| <span data-ttu-id="3c5ea-135">A ID da operação.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-135">The ID for the operation.</span></span> <span data-ttu-id="3c5ea-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-136">Read-only.</span></span> <span data-ttu-id="3c5ea-137">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3c5ea-137">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="3c5ea-138">percentProgress</span><span class="sxs-lookup"><span data-stu-id="3c5ea-138">percentProgress</span></span>|<span data-ttu-id="3c5ea-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3c5ea-139">Int32</span></span>|<span data-ttu-id="3c5ea-140">O progresso da operação.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-140">The progress of the operation.</span></span> <span data-ttu-id="3c5ea-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-141">Read-only.</span></span> <span data-ttu-id="3c5ea-142">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3c5ea-142">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="3c5ea-143">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3c5ea-143">resultInfo</span></span>|[<span data-ttu-id="3c5ea-144">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3c5ea-144">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="3c5ea-145">Contém informações de resultados específicas de falha e sucesso.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-145">Contains success and failure-specific result information.</span></span> <span data-ttu-id="3c5ea-146">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3c5ea-146">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="3c5ea-147">status</span><span class="sxs-lookup"><span data-stu-id="3c5ea-147">status</span></span>|[<span data-ttu-id="3c5ea-148">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="3c5ea-148">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="3c5ea-149">O status da operação de caso.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-149">The status of the case operation.</span></span> <span data-ttu-id="3c5ea-150">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3c5ea-150">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="3c5ea-151">Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-151">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

### <a name="datacollectionscope-values"></a><span data-ttu-id="3c5ea-152">valores dataCollectionScope</span><span class="sxs-lookup"><span data-stu-id="3c5ea-152">dataCollectionScope values</span></span>

|<span data-ttu-id="3c5ea-153">Member</span><span class="sxs-lookup"><span data-stu-id="3c5ea-153">Member</span></span>|<span data-ttu-id="3c5ea-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c5ea-154">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="3c5ea-155">allVersions</span><span class="sxs-lookup"><span data-stu-id="3c5ea-155">allVersions</span></span>|<span data-ttu-id="3c5ea-156">Inclua todas as versões de arquivos de sites.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-156">Include all versions of files from sites.</span></span>|
|<span data-ttu-id="3c5ea-157">linkedFiles</span><span class="sxs-lookup"><span data-stu-id="3c5ea-157">linkedFiles</span></span>|<span data-ttu-id="3c5ea-158">Inclua **anexo de nuvem** com emails na coleção.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-158">Include **cloud attachment** with emails in the collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c5ea-159">Relações</span><span class="sxs-lookup"><span data-stu-id="3c5ea-159">Relationships</span></span>

|<span data-ttu-id="3c5ea-160">Relação</span><span class="sxs-lookup"><span data-stu-id="3c5ea-160">Relationship</span></span>|<span data-ttu-id="3c5ea-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c5ea-161">Type</span></span>|<span data-ttu-id="3c5ea-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c5ea-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c5ea-163">reviewSet</span><span class="sxs-lookup"><span data-stu-id="3c5ea-163">reviewSet</span></span>|[<span data-ttu-id="3c5ea-164">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="3c5ea-164">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md)| <span data-ttu-id="3c5ea-165">O conjunto de revisão ao qual os itens correspondentes à consulta da coleção de origem são adicionados.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-165">The review set to which items matching the source collection query are added to.</span></span> |
|<span data-ttu-id="3c5ea-166">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="3c5ea-166">sourceCollection</span></span>|[<span data-ttu-id="3c5ea-167">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="3c5ea-167">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourceCollection.md)| <span data-ttu-id="3c5ea-168">A sourceCollection de onde os itens estão sendo adicionados.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-168">The sourceCollection that items are being added from.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3c5ea-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c5ea-169">JSON representation</span></span>

<span data-ttu-id="3c5ea-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c5ea-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.addToReviewSetOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.addToReviewSetOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```
