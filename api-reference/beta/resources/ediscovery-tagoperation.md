---
title: Tipo de recurso tagOperation
description: Representa a operação que lida com a aplicação de marcas a documentos em um conjunto de revisão com base em uma consulta de conjunto de revisão.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2af9b255e643a46f5f065b3caf62fda0ae9967a4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445943"
---
# <a name="tagoperation-resource-type"></a><span data-ttu-id="a1e3b-103">Tipo de recurso tagOperation</span><span class="sxs-lookup"><span data-stu-id="a1e3b-103">tagOperation resource type</span></span>

<span data-ttu-id="a1e3b-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a1e3b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1e3b-105">Representa a operação que lida com a aplicação de marcas a documentos em um conjunto de revisão com base em uma consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-105">Represents the operation that handles applying tags to documents in a review set based on a review set query.</span></span>

<span data-ttu-id="a1e3b-106">Herda de [caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="a1e3b-106">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a1e3b-107">Methods</span><span class="sxs-lookup"><span data-stu-id="a1e3b-107">Methods</span></span>

<span data-ttu-id="a1e3b-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="a1e3b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1e3b-109">Properties</span></span>

|<span data-ttu-id="a1e3b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1e3b-110">Property</span></span>|<span data-ttu-id="a1e3b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1e3b-111">Type</span></span>|<span data-ttu-id="a1e3b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1e3b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1e3b-113">ação</span><span class="sxs-lookup"><span data-stu-id="a1e3b-113">action</span></span>|[<span data-ttu-id="a1e3b-114">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="a1e3b-114">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="a1e3b-115">A ação de caso dessa entidade sempre será `applyTags` .</span><span class="sxs-lookup"><span data-stu-id="a1e3b-115">The case action for this entity will always be `applyTags`.</span></span> <span data-ttu-id="a1e3b-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-116">Read-only.</span></span> <span data-ttu-id="a1e3b-117">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="a1e3b-117">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="a1e3b-118">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e3b-118">completedDateTime</span></span>|<span data-ttu-id="a1e3b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e3b-119">DateTimeOffset</span></span>|<span data-ttu-id="a1e3b-120">A data e a hora em que a operação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-120">The date and time the operation was completed.</span></span> <span data-ttu-id="a1e3b-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-121">Read-only.</span></span> <span data-ttu-id="a1e3b-122">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="a1e3b-122">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="a1e3b-123">createdBy</span><span class="sxs-lookup"><span data-stu-id="a1e3b-123">createdBy</span></span>|[<span data-ttu-id="a1e3b-124">identitySet</span><span class="sxs-lookup"><span data-stu-id="a1e3b-124">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a1e3b-125">O usuário que criou a operação.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-125">The user who created the operation.</span></span> <span data-ttu-id="a1e3b-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-126">Read-only.</span></span> <span data-ttu-id="a1e3b-127">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="a1e3b-127">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="a1e3b-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e3b-128">createdDateTime</span></span>|<span data-ttu-id="a1e3b-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e3b-129">DateTimeOffset</span></span>|<span data-ttu-id="a1e3b-130">A data e a hora em que a operação foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-130">The date and time the operation was started.</span></span> <span data-ttu-id="a1e3b-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-131">Read-only.</span></span> <span data-ttu-id="a1e3b-132">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="a1e3b-132">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="a1e3b-133">id</span><span class="sxs-lookup"><span data-stu-id="a1e3b-133">id</span></span>|<span data-ttu-id="a1e3b-134">String</span><span class="sxs-lookup"><span data-stu-id="a1e3b-134">String</span></span>| <span data-ttu-id="a1e3b-135">A ID da operação.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-135">The ID for the operation.</span></span> <span data-ttu-id="a1e3b-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-136">Read-only.</span></span> <span data-ttu-id="a1e3b-137">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="a1e3b-137">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="a1e3b-138">percentProgress</span><span class="sxs-lookup"><span data-stu-id="a1e3b-138">percentProgress</span></span>|<span data-ttu-id="a1e3b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a1e3b-139">Int32</span></span>|<span data-ttu-id="a1e3b-140">O progresso da operação.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-140">The progress of the operation.</span></span> <span data-ttu-id="a1e3b-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-141">Read-only.</span></span> <span data-ttu-id="a1e3b-142">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="a1e3b-142">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="a1e3b-143">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a1e3b-143">resultInfo</span></span>|[<span data-ttu-id="a1e3b-144">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a1e3b-144">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="a1e3b-145">Contém informações de resultados específicas de falha e sucesso.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-145">Contains success and failure-specific result information.</span></span> <span data-ttu-id="a1e3b-146">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="a1e3b-146">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="a1e3b-147">status</span><span class="sxs-lookup"><span data-stu-id="a1e3b-147">status</span></span>|[<span data-ttu-id="a1e3b-148">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="a1e3b-148">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="a1e3b-149">O status da operação de caso.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-149">The status of the case operation.</span></span> <span data-ttu-id="a1e3b-150">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="a1e3b-150">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="a1e3b-151">Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-151">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1e3b-152">Relações</span><span class="sxs-lookup"><span data-stu-id="a1e3b-152">Relationships</span></span>

<span data-ttu-id="a1e3b-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1e3b-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1e3b-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1e3b-154">JSON representation</span></span>

<span data-ttu-id="a1e3b-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-155">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tagOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tagOperation",
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
