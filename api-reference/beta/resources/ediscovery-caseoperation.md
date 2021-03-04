---
title: Tipo de recurso caseOperation
description: Uma entidade abstrata que representa um processo de Descoberta eDiscovery de longa duração.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b94aeba03a49f2c49cbf991f0046422a18b20b50
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446174"
---
# <a name="caseoperation-resource-type"></a><span data-ttu-id="2aebb-103">Tipo de recurso caseOperation</span><span class="sxs-lookup"><span data-stu-id="2aebb-103">caseOperation resource type</span></span>

<span data-ttu-id="2aebb-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2aebb-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2aebb-105">Uma entidade abstrata que representa um processo de Descoberta eDiscovery de longa duração.</span><span class="sxs-lookup"><span data-stu-id="2aebb-105">An abstract entity that represents a long-running eDiscovery process.</span></span> <span data-ttu-id="2aebb-106">Ele contém um conjunto comum de propriedades que são compartilhadas entre entidades herdadas.</span><span class="sxs-lookup"><span data-stu-id="2aebb-106">It contains a common set of properties that are shared among inheriting entities.</span></span>  <span data-ttu-id="2aebb-107">Entidades derivadas de **caseOperation** incluem:</span><span class="sxs-lookup"><span data-stu-id="2aebb-107">Entities that derive from **caseOperation** include:</span></span>

- [<span data-ttu-id="2aebb-108">caseExportOperation</span><span class="sxs-lookup"><span data-stu-id="2aebb-108">caseExportOperation</span></span>](../resources/ediscovery-caseexportoperation.md)
- [<span data-ttu-id="2aebb-109">tagOperation</span><span class="sxs-lookup"><span data-stu-id="2aebb-109">tagOperation</span></span>](../resources/ediscovery-tagoperation.md)
- [<span data-ttu-id="2aebb-110">estimateStatisticsOperation</span><span class="sxs-lookup"><span data-stu-id="2aebb-110">estimateStatisticsOperation</span></span>](../resources/ediscovery-estimatestatisticsoperation.md)

<span data-ttu-id="2aebb-111">Herda da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="2aebb-111">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2aebb-112">Methods</span><span class="sxs-lookup"><span data-stu-id="2aebb-112">Methods</span></span>

<span data-ttu-id="2aebb-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2aebb-113">None.</span></span>

## <a name="properties"></a><span data-ttu-id="2aebb-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2aebb-114">Properties</span></span>

|<span data-ttu-id="2aebb-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2aebb-115">Property</span></span>|<span data-ttu-id="2aebb-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="2aebb-116">Type</span></span>|<span data-ttu-id="2aebb-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2aebb-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aebb-118">ação</span><span class="sxs-lookup"><span data-stu-id="2aebb-118">action</span></span>|[<span data-ttu-id="2aebb-119">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="2aebb-119">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="2aebb-120">O tipo de ação que a operação representa.</span><span class="sxs-lookup"><span data-stu-id="2aebb-120">The type of action the operation represents.</span></span> <span data-ttu-id="2aebb-121">Os valores possíveis são: `addToReviewSet` , `applyTags` , `contentExport` , `convertToPdf``estimateStatistics`</span><span class="sxs-lookup"><span data-stu-id="2aebb-121">Possible values are: `addToReviewSet`,`applyTags`,`contentExport`,`convertToPdf`,`estimateStatistics`</span></span>|
|<span data-ttu-id="2aebb-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2aebb-122">completedDateTime</span></span>|<span data-ttu-id="2aebb-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2aebb-123">DateTimeOffset</span></span>| <span data-ttu-id="2aebb-124">A data e a hora em que a operação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="2aebb-124">The date and time the operation was completed.</span></span> |
|<span data-ttu-id="2aebb-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="2aebb-125">createdBy</span></span>|[<span data-ttu-id="2aebb-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="2aebb-126">identitySet</span></span>](../resources/identityset.md)| <span data-ttu-id="2aebb-127">O usuário que criou a operação.</span><span class="sxs-lookup"><span data-stu-id="2aebb-127">The user that created the operation.</span></span> |
|<span data-ttu-id="2aebb-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2aebb-128">createdDateTime</span></span>|<span data-ttu-id="2aebb-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2aebb-129">DateTimeOffset</span></span>| <span data-ttu-id="2aebb-130">A data e a hora em que a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="2aebb-130">The date and time the operation was created.</span></span> |
|<span data-ttu-id="2aebb-131">id</span><span class="sxs-lookup"><span data-stu-id="2aebb-131">id</span></span>|<span data-ttu-id="2aebb-132">String</span><span class="sxs-lookup"><span data-stu-id="2aebb-132">String</span></span>| <span data-ttu-id="2aebb-133">A ID da operação.</span><span class="sxs-lookup"><span data-stu-id="2aebb-133">The ID for the operation.</span></span> <span data-ttu-id="2aebb-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2aebb-134">Read-only.</span></span> |
|<span data-ttu-id="2aebb-135">percentProgress</span><span class="sxs-lookup"><span data-stu-id="2aebb-135">percentProgress</span></span>|<span data-ttu-id="2aebb-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2aebb-136">Int32</span></span>| <span data-ttu-id="2aebb-137">O progresso da operação.</span><span class="sxs-lookup"><span data-stu-id="2aebb-137">The progress of the operation.</span></span> |
|<span data-ttu-id="2aebb-138">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2aebb-138">resultInfo</span></span>|[<span data-ttu-id="2aebb-139">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2aebb-139">resultInfo</span></span>](../resources/resultinfo.md)| <span data-ttu-id="2aebb-140">Contém informações de resultados específicas de falha e sucesso.</span><span class="sxs-lookup"><span data-stu-id="2aebb-140">Contains success and failure-specific result information.</span></span> |
|<span data-ttu-id="2aebb-141">status</span><span class="sxs-lookup"><span data-stu-id="2aebb-141">status</span></span>|[<span data-ttu-id="2aebb-142">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="2aebb-142">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)| <span data-ttu-id="2aebb-143">O status da operação de caso.</span><span class="sxs-lookup"><span data-stu-id="2aebb-143">The status of the case operation.</span></span> <span data-ttu-id="2aebb-144">Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2aebb-144">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

### <a name="caseaction-values"></a><span data-ttu-id="2aebb-145">valores caseAction</span><span class="sxs-lookup"><span data-stu-id="2aebb-145">caseAction values</span></span>

|<span data-ttu-id="2aebb-146">Member</span><span class="sxs-lookup"><span data-stu-id="2aebb-146">Member</span></span>|<span data-ttu-id="2aebb-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="2aebb-147">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="2aebb-148">addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="2aebb-148">addToReviewSet</span></span> | <span data-ttu-id="2aebb-149">A operação representa a adição de dados a um conjunto de revisão de uma coleção eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="2aebb-149">The operation represents adding data to a review set from an eDiscovery collection.</span></span> |
| <span data-ttu-id="2aebb-150">applyTags</span><span class="sxs-lookup"><span data-stu-id="2aebb-150">applyTags</span></span> | <span data-ttu-id="2aebb-151">A operação representa documentos de marcação em massa em um conjunto de revisão para a consulta do conjunto de revisão especificado.</span><span class="sxs-lookup"><span data-stu-id="2aebb-151">The operation represents bulk tagging documents in a review set for the specified review set query.</span></span> |
| <span data-ttu-id="2aebb-152">contentExport</span><span class="sxs-lookup"><span data-stu-id="2aebb-152">contentExport</span></span> | <span data-ttu-id="2aebb-153">A operação representa uma exportação de conteúdo de um conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="2aebb-153">The operation represents a content export from a review set.</span></span> |
| <span data-ttu-id="2aebb-154">convertToPdf</span><span class="sxs-lookup"><span data-stu-id="2aebb-154">convertToPdf</span></span> | <span data-ttu-id="2aebb-155">A operação representa a conversão de documentos em PDFs com redação.</span><span class="sxs-lookup"><span data-stu-id="2aebb-155">The operation represents converting documents to PDFs with redactions.</span></span> |
| <span data-ttu-id="2aebb-156">estimateStatistics</span><span class="sxs-lookup"><span data-stu-id="2aebb-156">estimateStatistics</span></span>  | <span data-ttu-id="2aebb-157">A operação representa a pesquisa em serviços do Microsoft 365, como Exchange, SharePoint e OneDrive para empresas.</span><span class="sxs-lookup"><span data-stu-id="2aebb-157">The operation represents searching against Microsoft 365 services such as Exchange, SharePoint, and OneDrive for business.</span></span> |

### <a name="caseoperationstatus-values"></a><span data-ttu-id="2aebb-158">valores caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="2aebb-158">caseOperationStatus values</span></span>

|<span data-ttu-id="2aebb-159">Member</span><span class="sxs-lookup"><span data-stu-id="2aebb-159">Member</span></span>|<span data-ttu-id="2aebb-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="2aebb-160">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="2aebb-161">notStarted</span><span class="sxs-lookup"><span data-stu-id="2aebb-161">notStarted</span></span> | <span data-ttu-id="2aebb-162">A operação ainda não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="2aebb-162">The operation has not yet started.</span></span> |
| <span data-ttu-id="2aebb-163">submissionFailed</span><span class="sxs-lookup"><span data-stu-id="2aebb-163">submissionFailed</span></span> | <span data-ttu-id="2aebb-164">Falha no envio da operação.</span><span class="sxs-lookup"><span data-stu-id="2aebb-164">Submission of the operation failed.</span></span> |
| <span data-ttu-id="2aebb-165">running</span><span class="sxs-lookup"><span data-stu-id="2aebb-165">running</span></span> | <span data-ttu-id="2aebb-166">A operação está em execução no momento.</span><span class="sxs-lookup"><span data-stu-id="2aebb-166">The operation is currently running.</span></span> |
| <span data-ttu-id="2aebb-167">bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="2aebb-167">succeeded</span></span> | <span data-ttu-id="2aebb-168">A operação foi concluída com êxito sem erros.</span><span class="sxs-lookup"><span data-stu-id="2aebb-168">The operation was successfully completed without any errors.</span></span> |
| <span data-ttu-id="2aebb-169">partiallySucceededed</span><span class="sxs-lookup"><span data-stu-id="2aebb-169">partiallySucceeded</span></span> | <span data-ttu-id="2aebb-170">A operação foi concluída, mas houve erros - Consulte [resultInfo para](../resources/resultinfo.md) obter detalhes de erro.</span><span class="sxs-lookup"><span data-stu-id="2aebb-170">The operation completed, but there were errors - See [resultInfo](../resources/resultinfo.md) for error details.</span></span> |
| <span data-ttu-id="2aebb-171">failed</span><span class="sxs-lookup"><span data-stu-id="2aebb-171">failed</span></span> | <span data-ttu-id="2aebb-172">Falha na operação - Consulte informações de resultados para obter detalhes de erro.</span><span class="sxs-lookup"><span data-stu-id="2aebb-172">The operation failed - See result info for error details.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2aebb-173">Relações</span><span class="sxs-lookup"><span data-stu-id="2aebb-173">Relationships</span></span>

<span data-ttu-id="2aebb-174">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2aebb-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2aebb-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2aebb-175">JSON representation</span></span>

<span data-ttu-id="2aebb-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2aebb-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
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
