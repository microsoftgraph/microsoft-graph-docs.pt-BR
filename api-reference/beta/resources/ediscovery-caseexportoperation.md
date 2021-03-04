---
title: Tipo de recurso caseExportOperation
description: Representa o processo de uma exportação de DescobertaSuporta.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c14f4211706879a6897b5f795202a30058d138bf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446179"
---
# <a name="caseexportoperation-resource-type"></a><span data-ttu-id="6fa20-103">Tipo de recurso caseExportOperation</span><span class="sxs-lookup"><span data-stu-id="6fa20-103">caseExportOperation resource type</span></span>

<span data-ttu-id="6fa20-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6fa20-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fa20-105">Representa o processo de uma exportação de DescobertaSuporta.</span><span class="sxs-lookup"><span data-stu-id="6fa20-105">Represents the process of an eDiscovery export.</span></span> <span data-ttu-id="6fa20-106">O **caseExportOperation** só pode ser recuperado do header na resposta `Location` a uma exportação de conjuntos de [revisão.](../api/ediscovery-reviewset-export.md)</span><span class="sxs-lookup"><span data-stu-id="6fa20-106">The **caseExportOperation** can only be retrieved from the `Location` header in the response to a [reviewset export](../api/ediscovery-reviewset-export.md).</span></span>

<span data-ttu-id="6fa20-107">Herda de [caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6fa20-107">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6fa20-108">Methods</span><span class="sxs-lookup"><span data-stu-id="6fa20-108">Methods</span></span>

|<span data-ttu-id="6fa20-109">Método</span><span class="sxs-lookup"><span data-stu-id="6fa20-109">Method</span></span>|<span data-ttu-id="6fa20-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6fa20-110">Return type</span></span>|<span data-ttu-id="6fa20-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa20-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fa20-112">getDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="6fa20-112">getDownloadUrl</span></span>](../api/ediscovery-caseexportoperation-getdownloadurl.md)|<span data-ttu-id="6fa20-113">String</span><span class="sxs-lookup"><span data-stu-id="6fa20-113">String</span></span>| <span data-ttu-id="6fa20-114">Retorna a URL da exportação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-114">Returns the URL for the export.</span></span>|

## <a name="properties"></a><span data-ttu-id="6fa20-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fa20-115">Properties</span></span>

|<span data-ttu-id="6fa20-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fa20-116">Property</span></span>|<span data-ttu-id="6fa20-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fa20-117">Type</span></span>|<span data-ttu-id="6fa20-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa20-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fa20-119">ação</span><span class="sxs-lookup"><span data-stu-id="6fa20-119">action</span></span>|[<span data-ttu-id="6fa20-120">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="6fa20-120">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="6fa20-121">A ação de caso dessa entidade sempre será `contentExport` .</span><span class="sxs-lookup"><span data-stu-id="6fa20-121">The case action for this entity will always be `contentExport`.</span></span> <span data-ttu-id="6fa20-122">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6fa20-122">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="6fa20-123">azureBlobContainer</span><span class="sxs-lookup"><span data-stu-id="6fa20-123">azureBlobContainer</span></span>|<span data-ttu-id="6fa20-124">String</span><span class="sxs-lookup"><span data-stu-id="6fa20-124">String</span></span>| <span data-ttu-id="6fa20-125">O nome do local de armazenamento do Azure onde a exportação será armazenada.</span><span class="sxs-lookup"><span data-stu-id="6fa20-125">The name of the Azure storage location where the export will be stored.</span></span> <span data-ttu-id="6fa20-126">Isso só se aplica às exportações armazenadas em seu próprio local de armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="6fa20-126">This only applies to exports stored in your own Azure storage location.</span></span> |
|<span data-ttu-id="6fa20-127">azureBlobToken</span><span class="sxs-lookup"><span data-stu-id="6fa20-127">azureBlobToken</span></span>|<span data-ttu-id="6fa20-128">String</span><span class="sxs-lookup"><span data-stu-id="6fa20-128">String</span></span>| <span data-ttu-id="6fa20-129">O token SAS para o local de armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="6fa20-129">The SAS token for the Azure storage location.</span></span>  <span data-ttu-id="6fa20-130">Isso só se aplica às exportações armazenadas em seu próprio local de armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="6fa20-130">This only applies to exports stored in your own Azure storage location.</span></span> |
|<span data-ttu-id="6fa20-131">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fa20-131">completedDateTime</span></span>|<span data-ttu-id="6fa20-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fa20-132">DateTimeOffset</span></span>| <span data-ttu-id="6fa20-133">A data e a hora em que a exportação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="6fa20-133">The date and time the export was completed.</span></span>  <span data-ttu-id="6fa20-134">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="6fa20-134">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="6fa20-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="6fa20-135">createdBy</span></span>|[<span data-ttu-id="6fa20-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="6fa20-136">identitySet</span></span>](../resources/identityset.md)| <span data-ttu-id="6fa20-137">O usuário que iniciou a operação de exportação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-137">The user who initiated the export operation.</span></span> <span data-ttu-id="6fa20-138">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="6fa20-138">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="6fa20-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fa20-139">createdDateTime</span></span>|<span data-ttu-id="6fa20-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fa20-140">DateTimeOffset</span></span>| <span data-ttu-id="6fa20-141">A data e a hora em que a exportação foi criada.</span><span class="sxs-lookup"><span data-stu-id="6fa20-141">The date and time the export was created.</span></span> <span data-ttu-id="6fa20-142">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="6fa20-142">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="6fa20-143">descrição</span><span class="sxs-lookup"><span data-stu-id="6fa20-143">description</span></span>|<span data-ttu-id="6fa20-144">String</span><span class="sxs-lookup"><span data-stu-id="6fa20-144">String</span></span>| <span data-ttu-id="6fa20-145">A descrição fornecida para a exportação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-145">The description provided for the export.</span></span> |
|<span data-ttu-id="6fa20-146">exportOptions</span><span class="sxs-lookup"><span data-stu-id="6fa20-146">exportOptions</span></span>|<span data-ttu-id="6fa20-147">microsoft.graph.ediscovery.exportOptions</span><span class="sxs-lookup"><span data-stu-id="6fa20-147">microsoft.graph.ediscovery.exportOptions</span></span>| <span data-ttu-id="6fa20-148">As opções fornecidas para a exportação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-148">The options provided for the export.</span></span> <span data-ttu-id="6fa20-149">Consulte [reviewSet: export](../api/ediscovery-reviewset-export.md) for more details.</span><span class="sxs-lookup"><span data-stu-id="6fa20-149">See [reviewSet: export](../api/ediscovery-reviewset-export.md) for more details.</span></span> <span data-ttu-id="6fa20-150">Os valores possíveis são: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span><span class="sxs-lookup"><span data-stu-id="6fa20-150">Possible values are: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span></span>|
|<span data-ttu-id="6fa20-151">exportStructure</span><span class="sxs-lookup"><span data-stu-id="6fa20-151">exportStructure</span></span>|<span data-ttu-id="6fa20-152">microsoft.graph.ediscovery.exportFileStructure</span><span class="sxs-lookup"><span data-stu-id="6fa20-152">microsoft.graph.ediscovery.exportFileStructure</span></span>|<span data-ttu-id="6fa20-153">As opções fornecidas que especificam a estrutura da exportação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-153">The options provided that specify the structure of the export.</span></span> <span data-ttu-id="6fa20-154">Consulte [reviewSet: export](../api/ediscovery-reviewset-export.md) for more details.</span><span class="sxs-lookup"><span data-stu-id="6fa20-154">See [reviewSet: export](../api/ediscovery-reviewset-export.md) for more details.</span></span> <span data-ttu-id="6fa20-155">Os valores possíveis são: `none`, `directory`, `pst`.</span><span class="sxs-lookup"><span data-stu-id="6fa20-155">Possible values are: `none`, `directory`, `pst`.</span></span>|
|<span data-ttu-id="6fa20-156">id</span><span class="sxs-lookup"><span data-stu-id="6fa20-156">id</span></span>|<span data-ttu-id="6fa20-157">String</span><span class="sxs-lookup"><span data-stu-id="6fa20-157">String</span></span>| <span data-ttu-id="6fa20-158">A ID da operação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-158">The ID for the operation.</span></span> <span data-ttu-id="6fa20-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fa20-159">Read-only.</span></span> <span data-ttu-id="6fa20-160">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6fa20-160">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="6fa20-161">outputName</span><span class="sxs-lookup"><span data-stu-id="6fa20-161">outputName</span></span>|<span data-ttu-id="6fa20-162">String</span><span class="sxs-lookup"><span data-stu-id="6fa20-162">String</span></span>| <span data-ttu-id="6fa20-163">O nome fornecido para a exportação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-163">The name provided for the export.</span></span>|
|<span data-ttu-id="6fa20-164">percentProgress</span><span class="sxs-lookup"><span data-stu-id="6fa20-164">percentProgress</span></span>|<span data-ttu-id="6fa20-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6fa20-165">Int32</span></span>| <span data-ttu-id="6fa20-166">O progresso da operação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-166">The progress of the operation.</span></span> <span data-ttu-id="6fa20-167">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="6fa20-167">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="6fa20-168">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6fa20-168">resultInfo</span></span>|[<span data-ttu-id="6fa20-169">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6fa20-169">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="6fa20-170">Contém informações de resultados específicas de falha e sucesso.</span><span class="sxs-lookup"><span data-stu-id="6fa20-170">Contains success and failure-specific result information.</span></span> <span data-ttu-id="6fa20-171">Herdado de [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="6fa20-171">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="6fa20-172">status</span><span class="sxs-lookup"><span data-stu-id="6fa20-172">status</span></span>|[<span data-ttu-id="6fa20-173">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="6fa20-173">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="6fa20-174">O status da operação de caso.</span><span class="sxs-lookup"><span data-stu-id="6fa20-174">The status of the case operation.</span></span> <span data-ttu-id="6fa20-175">Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6fa20-175">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="6fa20-176">Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6fa20-176">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

### <a name="exportoptions-values"></a><span data-ttu-id="6fa20-177">valores exportOptions</span><span class="sxs-lookup"><span data-stu-id="6fa20-177">exportOptions values</span></span>

|<span data-ttu-id="6fa20-178">Member</span><span class="sxs-lookup"><span data-stu-id="6fa20-178">Member</span></span>| <span data-ttu-id="6fa20-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa20-179">Description</span></span> |
|:---|:---|
|<span data-ttu-id="6fa20-180">originalFiles</span><span class="sxs-lookup"><span data-stu-id="6fa20-180">originalFiles</span></span>| <span data-ttu-id="6fa20-181">Incluir cópias dos arquivos originais - exclua essa opção ao gerar relatórios somente</span><span class="sxs-lookup"><span data-stu-id="6fa20-181">Include copies of the original files - exclude this option when generating reports only</span></span> |
|<span data-ttu-id="6fa20-182">texto</span><span class="sxs-lookup"><span data-stu-id="6fa20-182">text</span></span>| <span data-ttu-id="6fa20-183">Inclua arquivos de texto extraídos brutos para cada documento.</span><span class="sxs-lookup"><span data-stu-id="6fa20-183">Include raw extracted text files for each document.</span></span> |
|<span data-ttu-id="6fa20-184">pdfReplacement</span><span class="sxs-lookup"><span data-stu-id="6fa20-184">pdfReplacement</span></span>| <span data-ttu-id="6fa20-185">Se os arquivos PDF redacted são gerados durante a revisão, esses arquivos estarão disponíveis para exportação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-185">If redacted PDF files are generated during review, these files are available for export.</span></span> <span data-ttu-id="6fa20-186">Você pode optar por exportar os PDFs redacted em vez dos arquivos nativos originais incluindo essa opção.</span><span class="sxs-lookup"><span data-stu-id="6fa20-186">You can choose to export the redacted PDFs instead of the original native files by including this option.</span></span> |
|<span data-ttu-id="6fa20-187">fileInfo</span><span class="sxs-lookup"><span data-stu-id="6fa20-187">fileInfo</span></span>| <span data-ttu-id="6fa20-188">Inclua o arquivo de verão e de carga - isso sempre deve ser incluído.</span><span class="sxs-lookup"><span data-stu-id="6fa20-188">Include the summery and load file - this should always be included.</span></span> |
|<span data-ttu-id="6fa20-189">tags</span><span class="sxs-lookup"><span data-stu-id="6fa20-189">tags</span></span>| <span data-ttu-id="6fa20-190">Inclua marcas de documento que foram aplicadas durante a revisão no arquivo de carga.</span><span class="sxs-lookup"><span data-stu-id="6fa20-190">Include document tags that were applied during review in the load file.</span></span> |

### <a name="exportfilestructure-values"></a><span data-ttu-id="6fa20-191">valores exportFileStructure</span><span class="sxs-lookup"><span data-stu-id="6fa20-191">exportFileStructure values</span></span>

|<span data-ttu-id="6fa20-192">Member</span><span class="sxs-lookup"><span data-stu-id="6fa20-192">Member</span></span>| <span data-ttu-id="6fa20-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa20-193">Description</span></span> |
|:---|:---|
|<span data-ttu-id="6fa20-194">directory</span><span class="sxs-lookup"><span data-stu-id="6fa20-194">directory</span></span>| <span data-ttu-id="6fa20-195">Mapeia para a estrutura de diretório condensada comumente usada por ferramentas de Descoberta e.</span><span class="sxs-lookup"><span data-stu-id="6fa20-195">Maps to the condensed directory structure commonly used by eDiscovery tools.</span></span> <span data-ttu-id="6fa20-196">Todos os arquivos são exportados para um arquivo raiz chamado NativeFiles.</span><span class="sxs-lookup"><span data-stu-id="6fa20-196">All files are exported to a root file called NativeFiles.</span></span> |
|<span data-ttu-id="6fa20-197">pst</span><span class="sxs-lookup"><span data-stu-id="6fa20-197">pst</span></span>| <span data-ttu-id="6fa20-198">Os emails são armazenados em PSTs enquanto documentos de sites são armazenados em pastas que representam a estrutura de pastas nativas original.</span><span class="sxs-lookup"><span data-stu-id="6fa20-198">Emails are stored in PSTs while documents from sites are stored in folders that represent the original native folder structure.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6fa20-199">Relações</span><span class="sxs-lookup"><span data-stu-id="6fa20-199">Relationships</span></span>

|<span data-ttu-id="6fa20-200">Relação</span><span class="sxs-lookup"><span data-stu-id="6fa20-200">Relationship</span></span>|<span data-ttu-id="6fa20-201">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fa20-201">Type</span></span>|<span data-ttu-id="6fa20-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa20-202">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fa20-203">reviewSet</span><span class="sxs-lookup"><span data-stu-id="6fa20-203">reviewSet</span></span>|[<span data-ttu-id="6fa20-204">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="6fa20-204">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md)| <span data-ttu-id="6fa20-205">O conjunto de revisão de onde o conteúdo está sendo exportado.</span><span class="sxs-lookup"><span data-stu-id="6fa20-205">The review set the content is being exported from.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6fa20-206">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fa20-206">JSON representation</span></span>

<span data-ttu-id="6fa20-207">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fa20-207">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseExportOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseExportOperation",
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
  },
  "outputName": "String",
  "description": "String",
  "outputFolderId": "String",
  "azureBlobContainer": "String",
  "azureBlobToken": "String",
  "exportOptions": "String",
  "exportStructure": "String"
}
```
