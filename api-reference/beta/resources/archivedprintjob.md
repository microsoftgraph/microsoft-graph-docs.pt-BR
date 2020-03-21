---
title: tipo de recurso archivedPrintJob
description: Um registro de um trabalho de impressão "estado final" (concluído, anulado ou com falha) que é usado para fins de relatório. Este não é um trabalho de impressão ativo.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 170f3b735b4f14173058efbaaa1c81b80490f020
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895474"
---
# <a name="archivedprintjob-resource-type"></a><span data-ttu-id="11fac-104">tipo de recurso archivedPrintJob</span><span class="sxs-lookup"><span data-stu-id="11fac-104">archivedPrintJob resource type</span></span>

<span data-ttu-id="11fac-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11fac-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11fac-106">Um registro de um trabalho de impressão "estado final" (concluído, anulado ou com falha) que é usado para fins de relatório.</span><span class="sxs-lookup"><span data-stu-id="11fac-106">A record of a "final state" (completed, aborted or failed) print job that is used for reporting purposes.</span></span> <span data-ttu-id="11fac-107">Este não é um trabalho de impressão ativo.</span><span class="sxs-lookup"><span data-stu-id="11fac-107">This is not an active print job.</span></span>

## <a name="properties"></a><span data-ttu-id="11fac-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11fac-108">Properties</span></span>
| <span data-ttu-id="11fac-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11fac-109">Property</span></span>     | <span data-ttu-id="11fac-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="11fac-110">Type</span></span>        | <span data-ttu-id="11fac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11fac-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11fac-112">id</span><span class="sxs-lookup"><span data-stu-id="11fac-112">id</span></span>|<span data-ttu-id="11fac-113">String</span><span class="sxs-lookup"><span data-stu-id="11fac-113">String</span></span>|<span data-ttu-id="11fac-114">O GUID do trabalho de impressão arquivado.</span><span class="sxs-lookup"><span data-stu-id="11fac-114">The archived print job's GUID.</span></span> <span data-ttu-id="11fac-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-115">Read-only.</span></span>|
|<span data-ttu-id="11fac-116">printerid</span><span class="sxs-lookup"><span data-stu-id="11fac-116">printerId</span></span>|<span data-ttu-id="11fac-117">String</span><span class="sxs-lookup"><span data-stu-id="11fac-117">String</span></span>|<span data-ttu-id="11fac-118">A ID da impressora para a qual o trabalho foi enfileirado.</span><span class="sxs-lookup"><span data-stu-id="11fac-118">The printer ID that the job was queued for.</span></span> <span data-ttu-id="11fac-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-119">Read-only.</span></span>|
|<span data-ttu-id="11fac-120">ProcessingState</span><span class="sxs-lookup"><span data-stu-id="11fac-120">processingState</span></span>|<span data-ttu-id="11fac-121">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="11fac-121">printJobProcessingState</span></span>|<span data-ttu-id="11fac-122">O estado de processamento final do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="11fac-122">The print job's final processing state.</span></span> <span data-ttu-id="11fac-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-123">Read-only.</span></span>|
|<span data-ttu-id="11fac-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11fac-124">createdDateTime</span></span>|<span data-ttu-id="11fac-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11fac-125">DateTimeOffset</span></span>|<span data-ttu-id="11fac-126">O dateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="11fac-126">The dateTimeOffset when the job was created.</span></span> <span data-ttu-id="11fac-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-127">Read-only.</span></span>|
|<span data-ttu-id="11fac-128">acquiredDateTime</span><span class="sxs-lookup"><span data-stu-id="11fac-128">acquiredDateTime</span></span>|<span data-ttu-id="11fac-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11fac-129">DateTimeOffset</span></span>|<span data-ttu-id="11fac-130">O dateTimeOffset quando o trabalho foi adquirido pela impressora, se houver.</span><span class="sxs-lookup"><span data-stu-id="11fac-130">The dateTimeOffset when the job was acquired by the printer, if any.</span></span> <span data-ttu-id="11fac-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-131">Read-only.</span></span>|
|<span data-ttu-id="11fac-132">completionDateTime</span><span class="sxs-lookup"><span data-stu-id="11fac-132">completionDateTime</span></span>|<span data-ttu-id="11fac-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11fac-133">DateTimeOffset</span></span>|<span data-ttu-id="11fac-134">O dateTimeOffset quando o trabalho foi concluído, cancelado ou anulado.</span><span class="sxs-lookup"><span data-stu-id="11fac-134">The dateTimeOffset when the job was completed, canceled or aborted.</span></span> <span data-ttu-id="11fac-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-135">Read-only.</span></span>|
|<span data-ttu-id="11fac-136">acquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="11fac-136">acquiredByPrinter</span></span>|<span data-ttu-id="11fac-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="11fac-137">Boolean</span></span>|<span data-ttu-id="11fac-138">True se o trabalho foi adquirido por uma impressora; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="11fac-138">True if the job was acquired by a printer; false otherwise.</span></span> <span data-ttu-id="11fac-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-139">Read-only.</span></span>|
|<span data-ttu-id="11fac-140">copiesPrinted</span><span class="sxs-lookup"><span data-stu-id="11fac-140">copiesPrinted</span></span>|<span data-ttu-id="11fac-141">Int32</span><span class="sxs-lookup"><span data-stu-id="11fac-141">Int32</span></span>|<span data-ttu-id="11fac-142">O número de cópias que foram impressas.</span><span class="sxs-lookup"><span data-stu-id="11fac-142">The number of copies that were printed.</span></span> <span data-ttu-id="11fac-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-143">Read-only.</span></span>|
|<span data-ttu-id="11fac-144">pageCount</span><span class="sxs-lookup"><span data-stu-id="11fac-144">pageCount</span></span>|<span data-ttu-id="11fac-145">Int32</span><span class="sxs-lookup"><span data-stu-id="11fac-145">Int32</span></span>|<span data-ttu-id="11fac-146">O número total de páginas que foram impressas.</span><span class="sxs-lookup"><span data-stu-id="11fac-146">The total number of pages that were printed.</span></span> <span data-ttu-id="11fac-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-147">Read-only.</span></span>|
|<span data-ttu-id="11fac-148">blackAndWhitePageCount</span><span class="sxs-lookup"><span data-stu-id="11fac-148">blackAndWhitePageCount</span></span>|<span data-ttu-id="11fac-149">Int32</span><span class="sxs-lookup"><span data-stu-id="11fac-149">Int32</span></span>|<span data-ttu-id="11fac-150">O número de páginas em preto e branco que foram impressas.</span><span class="sxs-lookup"><span data-stu-id="11fac-150">The number of black and white pages that were printed.</span></span> <span data-ttu-id="11fac-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-151">Read-only.</span></span>|
|<span data-ttu-id="11fac-152">colorPageCount</span><span class="sxs-lookup"><span data-stu-id="11fac-152">colorPageCount</span></span>|<span data-ttu-id="11fac-153">Int32</span><span class="sxs-lookup"><span data-stu-id="11fac-153">Int32</span></span>|<span data-ttu-id="11fac-154">O número de páginas de cores que foram impressas.</span><span class="sxs-lookup"><span data-stu-id="11fac-154">The number of color pages that were printed.</span></span> <span data-ttu-id="11fac-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-155">Read-only.</span></span>|
|<span data-ttu-id="11fac-156">simplexPageCount</span><span class="sxs-lookup"><span data-stu-id="11fac-156">simplexPageCount</span></span>|<span data-ttu-id="11fac-157">Int32</span><span class="sxs-lookup"><span data-stu-id="11fac-157">Int32</span></span>|<span data-ttu-id="11fac-158">O número de páginas simplex (de lado único) que foram impressas.</span><span class="sxs-lookup"><span data-stu-id="11fac-158">The number of simplex (single-sided) pages that were printed.</span></span> <span data-ttu-id="11fac-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-159">Read-only.</span></span>|
|<span data-ttu-id="11fac-160">duplexPageCount</span><span class="sxs-lookup"><span data-stu-id="11fac-160">duplexPageCount</span></span>|<span data-ttu-id="11fac-161">Int32</span><span class="sxs-lookup"><span data-stu-id="11fac-161">Int32</span></span>|<span data-ttu-id="11fac-162">O número de páginas duplex (frente e verso) que foram impressas.</span><span class="sxs-lookup"><span data-stu-id="11fac-162">The number of duplex (double-sided) pages that were printed.</span></span> <span data-ttu-id="11fac-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-163">Read-only.</span></span>|
|<span data-ttu-id="11fac-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="11fac-164">createdBy</span></span>|[<span data-ttu-id="11fac-165">userIdentity</span><span class="sxs-lookup"><span data-stu-id="11fac-165">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="11fac-166">O usuário que criou o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="11fac-166">The user who created the print job.</span></span> <span data-ttu-id="11fac-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11fac-167">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11fac-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11fac-168">JSON representation</span></span>

<span data-ttu-id="11fac-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11fac-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->

```json
{
    "id": "String (identifier)",
    "printer": {"@odata.type": "microsoft.graph.directoryObject"},
    "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
    "processingState": {"@odata.type": "microsoft.graph.printJobProcessingState"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "archivedPrintJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->