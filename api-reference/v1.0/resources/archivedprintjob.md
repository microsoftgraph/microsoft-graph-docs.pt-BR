---
title: Tipo de recurso archivedPrintJob
description: Um registro de um trabalho de impressão "estado final" (concluído, abortado ou com falha) usado para fins de relatório. Este não é um trabalho de impressão ativo.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2132b5a7cdf5024fb13845c57844220594ba6e1f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516922"
---
# <a name="archivedprintjob-resource-type"></a><span data-ttu-id="cf5da-104">Tipo de recurso archivedPrintJob</span><span class="sxs-lookup"><span data-stu-id="cf5da-104">archivedPrintJob resource type</span></span>

<span data-ttu-id="cf5da-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf5da-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf5da-106">Um registro de um trabalho de impressão "estado final" (concluído, abortado ou com falha) usado para fins de relatório.</span><span class="sxs-lookup"><span data-stu-id="cf5da-106">A record of a "final state" (completed, aborted or failed) print job that is used for reporting purposes.</span></span> <span data-ttu-id="cf5da-107">Este não é um trabalho de impressão ativo.</span><span class="sxs-lookup"><span data-stu-id="cf5da-107">This is not an active print job.</span></span>

## <a name="properties"></a><span data-ttu-id="cf5da-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf5da-108">Properties</span></span>
| <span data-ttu-id="cf5da-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf5da-109">Property</span></span>     | <span data-ttu-id="cf5da-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf5da-110">Type</span></span>        | <span data-ttu-id="cf5da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf5da-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf5da-112">id</span><span class="sxs-lookup"><span data-stu-id="cf5da-112">id</span></span>|<span data-ttu-id="cf5da-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf5da-113">String</span></span>|<span data-ttu-id="cf5da-114">GUID do trabalho de impressão arquivado.</span><span class="sxs-lookup"><span data-stu-id="cf5da-114">The archived print job's GUID.</span></span> <span data-ttu-id="cf5da-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf5da-115">Read-only.</span></span>|
|<span data-ttu-id="cf5da-116">printerId</span><span class="sxs-lookup"><span data-stu-id="cf5da-116">printerId</span></span>|<span data-ttu-id="cf5da-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf5da-117">String</span></span>|<span data-ttu-id="cf5da-118">A ID da impressora na fila do trabalho.</span><span class="sxs-lookup"><span data-stu-id="cf5da-118">The printer ID that the job was queued for.</span></span> <span data-ttu-id="cf5da-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf5da-119">Read-only.</span></span>|
|<span data-ttu-id="cf5da-120">processingState</span><span class="sxs-lookup"><span data-stu-id="cf5da-120">processingState</span></span>|<span data-ttu-id="cf5da-121">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="cf5da-121">printJobProcessingState</span></span>|<span data-ttu-id="cf5da-122">O estado final de processamento do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="cf5da-122">The print job's final processing state.</span></span> <span data-ttu-id="cf5da-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf5da-123">Read-only.</span></span>|
|<span data-ttu-id="cf5da-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5da-124">createdDateTime</span></span>|<span data-ttu-id="cf5da-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5da-125">DateTimeOffset</span></span>|<span data-ttu-id="cf5da-126">DateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="cf5da-126">The dateTimeOffset when the job was created.</span></span> <span data-ttu-id="cf5da-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf5da-127">Read-only.</span></span>|
|<span data-ttu-id="cf5da-128">acquiredDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5da-128">acquiredDateTime</span></span>|<span data-ttu-id="cf5da-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5da-129">DateTimeOffset</span></span>|<span data-ttu-id="cf5da-130">O dateTimeOffset quando o trabalho foi adquirido pela impressora, se for o caso.</span><span class="sxs-lookup"><span data-stu-id="cf5da-130">The dateTimeOffset when the job was acquired by the printer, if any.</span></span> <span data-ttu-id="cf5da-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf5da-131">Read-only.</span></span>|
|<span data-ttu-id="cf5da-132">completionDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5da-132">completionDateTime</span></span>|<span data-ttu-id="cf5da-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5da-133">DateTimeOffset</span></span>|<span data-ttu-id="cf5da-134">DateTimeOffset quando o trabalho foi concluído, cancelado ou abortado.</span><span class="sxs-lookup"><span data-stu-id="cf5da-134">The dateTimeOffset when the job was completed, canceled or aborted.</span></span> <span data-ttu-id="cf5da-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf5da-135">Read-only.</span></span>|
|<span data-ttu-id="cf5da-136">acquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="cf5da-136">acquiredByPrinter</span></span>|<span data-ttu-id="cf5da-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf5da-137">Boolean</span></span>|<span data-ttu-id="cf5da-138">True se o trabalho foi adquirido por uma impressora; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="cf5da-138">True if the job was acquired by a printer; false otherwise.</span></span> <span data-ttu-id="cf5da-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf5da-139">Read-only.</span></span>|
|<span data-ttu-id="cf5da-140">copiesPrinted</span><span class="sxs-lookup"><span data-stu-id="cf5da-140">copiesPrinted</span></span>|<span data-ttu-id="cf5da-141">Int32</span><span class="sxs-lookup"><span data-stu-id="cf5da-141">Int32</span></span>|<span data-ttu-id="cf5da-142">O número de cópias que foram impressas.</span><span class="sxs-lookup"><span data-stu-id="cf5da-142">The number of copies that were printed.</span></span> <span data-ttu-id="cf5da-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf5da-143">Read-only.</span></span>|
|<span data-ttu-id="cf5da-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="cf5da-144">createdBy</span></span>|[<span data-ttu-id="cf5da-145">userIdentity</span><span class="sxs-lookup"><span data-stu-id="cf5da-145">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="cf5da-146">O usuário que criou o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="cf5da-146">The user who created the print job.</span></span> <span data-ttu-id="cf5da-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf5da-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf5da-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf5da-148">JSON representation</span></span>

<span data-ttu-id="cf5da-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf5da-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->
```json
    {   
  "@odata.type": "#microsoft.graph.archivedPrintJob",   
  "id": "String (identifier)",  
  "printerId": "String",    
  "processingState": "String",  
  "createdDateTime": "String (timestamp)",  
  "acquiredDateTime": "String (timestamp)", 
  "completionDateTime": "String (timestamp)",   
  "acquiredByPrinter": "Boolean",   
  "copiesPrinted": "Integer",   
  "createdBy": {    
    "@odata.type": "microsoft.graph.userIdentity"   
  } 
}
```