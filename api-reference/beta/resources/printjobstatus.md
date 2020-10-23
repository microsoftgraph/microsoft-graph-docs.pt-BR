---
title: tipo de recurso printJobStatus
description: Representa o status atual de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bb3221eb12946d58664211731a31993e540aaf00
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728932"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="f1946-103">tipo de recurso printJobStatus</span><span class="sxs-lookup"><span data-stu-id="f1946-103">printJobStatus resource type</span></span>

<span data-ttu-id="f1946-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1946-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1946-105">Representa o status atual de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1946-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="f1946-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1946-106">Properties</span></span>
| <span data-ttu-id="f1946-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1946-107">Property</span></span>     | <span data-ttu-id="f1946-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1946-108">Type</span></span>        | <span data-ttu-id="f1946-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1946-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f1946-110">state</span><span class="sxs-lookup"><span data-stu-id="f1946-110">state</span></span>|<span data-ttu-id="f1946-111">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="f1946-111">printJobProcessingState</span></span>|<span data-ttu-id="f1946-112">O estado atual de processamento do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1946-112">The print job's current processing state.</span></span> <span data-ttu-id="f1946-113">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f1946-113">Valid values are described in the following table.</span></span> <span data-ttu-id="f1946-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1946-114">Read-only.</span></span>|
|<span data-ttu-id="f1946-115">detalhes</span><span class="sxs-lookup"><span data-stu-id="f1946-115">details</span></span>|<span data-ttu-id="f1946-116">coleção printJobProcessingDetail</span><span class="sxs-lookup"><span data-stu-id="f1946-116">printJobProcessingDetail collection</span></span>|<span data-ttu-id="f1946-117">Detalhes adicionais para o estado do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1946-117">Additional details for print job state.</span></span> <span data-ttu-id="f1946-118">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f1946-118">Valid values are described in the following table.</span></span> <span data-ttu-id="f1946-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1946-119">Read-only.</span></span>|
|<span data-ttu-id="f1946-120">description</span><span class="sxs-lookup"><span data-stu-id="f1946-120">description</span></span>|<span data-ttu-id="f1946-121">String</span><span class="sxs-lookup"><span data-stu-id="f1946-121">String</span></span>|<span data-ttu-id="f1946-122">Uma descrição legível do estado de processamento atual do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1946-122">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="f1946-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1946-123">Read-only.</span></span>|
|<span data-ttu-id="f1946-124">isAcquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="f1946-124">isAcquiredByPrinter</span></span>|<span data-ttu-id="f1946-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1946-125">Boolean</span></span>|<span data-ttu-id="f1946-126">True se o trabalho foi confirmado por uma impressora; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="f1946-126">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="f1946-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1946-127">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="f1946-128">valores de printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="f1946-128">printJobProcessingState values</span></span>

|<span data-ttu-id="f1946-129">Membro</span><span class="sxs-lookup"><span data-stu-id="f1946-129">Member</span></span>|<span data-ttu-id="f1946-130">Valor</span><span class="sxs-lookup"><span data-stu-id="f1946-130">Value</span></span>|<span data-ttu-id="f1946-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1946-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1946-132">desconhecido</span><span class="sxs-lookup"><span data-stu-id="f1946-132">unknown</span></span>|<span data-ttu-id="f1946-133">,0</span><span class="sxs-lookup"><span data-stu-id="f1946-133">0</span></span>|<span data-ttu-id="f1946-134">O estado de processamento relatado pela impressora não é reconhecido.</span><span class="sxs-lookup"><span data-stu-id="f1946-134">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="f1946-135">função</span><span class="sxs-lookup"><span data-stu-id="f1946-135">pending</span></span>|<span data-ttu-id="f1946-136">1</span><span class="sxs-lookup"><span data-stu-id="f1946-136">1</span></span>|<span data-ttu-id="f1946-137">O trabalho de impressão está aguardando o processamento da impressora.</span><span class="sxs-lookup"><span data-stu-id="f1946-137">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="f1946-138">processe</span><span class="sxs-lookup"><span data-stu-id="f1946-138">processing</span></span>|<span data-ttu-id="f1946-139">duas</span><span class="sxs-lookup"><span data-stu-id="f1946-139">2</span></span>|<span data-ttu-id="f1946-140">O trabalho de impressão está sendo processado pela impressora no momento.</span><span class="sxs-lookup"><span data-stu-id="f1946-140">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="f1946-141">pausado</span><span class="sxs-lookup"><span data-stu-id="f1946-141">paused</span></span>|<span data-ttu-id="f1946-142">3D</span><span class="sxs-lookup"><span data-stu-id="f1946-142">3</span></span>|<span data-ttu-id="f1946-143">O trabalho de impressão foi pausado.</span><span class="sxs-lookup"><span data-stu-id="f1946-143">The print job has been paused.</span></span>|
|<span data-ttu-id="f1946-144">parar</span><span class="sxs-lookup"><span data-stu-id="f1946-144">stopped</span></span>|<span data-ttu-id="f1946-145">4 </span><span class="sxs-lookup"><span data-stu-id="f1946-145">4</span></span>|<span data-ttu-id="f1946-146">O trabalho de impressão foi interrompido porque um problema com a impressora precisa ser resolvido para que o trabalho possa continuar.</span><span class="sxs-lookup"><span data-stu-id="f1946-146">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="f1946-147">Mais informações podem ser encontradas no recurso de estado da impressora.</span><span class="sxs-lookup"><span data-stu-id="f1946-147">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="f1946-148">Completed</span><span class="sxs-lookup"><span data-stu-id="f1946-148">completed</span></span>|<span data-ttu-id="f1946-149">5 </span><span class="sxs-lookup"><span data-stu-id="f1946-149">5</span></span>|<span data-ttu-id="f1946-150">O trabalho de impressão foi concluído com êxito e nenhum processamento adicional ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="f1946-150">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="f1946-151">foi</span><span class="sxs-lookup"><span data-stu-id="f1946-151">canceled</span></span>|<span data-ttu-id="f1946-152">6 </span><span class="sxs-lookup"><span data-stu-id="f1946-152">6</span></span>|<span data-ttu-id="f1946-153">O trabalho de impressão foi cancelado por um usuário e nenhum processamento adicional ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="f1946-153">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="f1946-154">anulada</span><span class="sxs-lookup"><span data-stu-id="f1946-154">aborted</span></span>|<span data-ttu-id="f1946-155">7 </span><span class="sxs-lookup"><span data-stu-id="f1946-155">7</span></span>|<span data-ttu-id="f1946-156">O trabalho de impressão foi anulado por um usuário ou pela impressora e nenhum processamento adicional ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="f1946-156">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

### <a name="printjobprocessingdetail-values"></a><span data-ttu-id="f1946-157">valores de printJobProcessingDetail</span><span class="sxs-lookup"><span data-stu-id="f1946-157">printJobProcessingDetail values</span></span>

|<span data-ttu-id="f1946-158">Membro</span><span class="sxs-lookup"><span data-stu-id="f1946-158">Member</span></span>|<span data-ttu-id="f1946-159">Valor</span><span class="sxs-lookup"><span data-stu-id="f1946-159">Value</span></span>|<span data-ttu-id="f1946-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1946-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1946-161">uploadPending</span><span class="sxs-lookup"><span data-stu-id="f1946-161">uploadPending</span></span>|<span data-ttu-id="f1946-162">,0</span><span class="sxs-lookup"><span data-stu-id="f1946-162">0</span></span>|<span data-ttu-id="f1946-163">A carga do documento não foi carregada.</span><span class="sxs-lookup"><span data-stu-id="f1946-163">Document payload has not been uploaded.</span></span>|
|<span data-ttu-id="f1946-164">transformar</span><span class="sxs-lookup"><span data-stu-id="f1946-164">transforming</span></span>|<span data-ttu-id="f1946-165">1</span><span class="sxs-lookup"><span data-stu-id="f1946-165">1</span></span>|<span data-ttu-id="f1946-166">A carga do documento está sendo transformada.</span><span class="sxs-lookup"><span data-stu-id="f1946-166">Document payload is being transformed.</span></span>|
|<span data-ttu-id="f1946-167">completedSuccessfully</span><span class="sxs-lookup"><span data-stu-id="f1946-167">completedSuccessfully</span></span>|<span data-ttu-id="f1946-168">duas</span><span class="sxs-lookup"><span data-stu-id="f1946-168">2</span></span>|<span data-ttu-id="f1946-169">O trabalho foi concluído com êxito.</span><span class="sxs-lookup"><span data-stu-id="f1946-169">Job has been completed successfully.</span></span>|
|<span data-ttu-id="f1946-170">completedWithWarnings</span><span class="sxs-lookup"><span data-stu-id="f1946-170">completedWithWarnings</span></span>|<span data-ttu-id="f1946-171">3D</span><span class="sxs-lookup"><span data-stu-id="f1946-171">3</span></span>|<span data-ttu-id="f1946-172">O trabalho foi concluído com avisos.</span><span class="sxs-lookup"><span data-stu-id="f1946-172">Job has been completed with warnings.</span></span>|
|<span data-ttu-id="f1946-173">completedWithErrors</span><span class="sxs-lookup"><span data-stu-id="f1946-173">completedWithErrors</span></span>|<span data-ttu-id="f1946-174">4 </span><span class="sxs-lookup"><span data-stu-id="f1946-174">4</span></span>|<span data-ttu-id="f1946-175">O trabalho foi concluído com erros.</span><span class="sxs-lookup"><span data-stu-id="f1946-175">Job has been completed with errors.</span></span>|
|<span data-ttu-id="f1946-176">releaseWait</span><span class="sxs-lookup"><span data-stu-id="f1946-176">releaseWait</span></span>|<span data-ttu-id="f1946-177">5 </span><span class="sxs-lookup"><span data-stu-id="f1946-177">5</span></span>|<span data-ttu-id="f1946-178">O trabalho está pendente para ser liberado.</span><span class="sxs-lookup"><span data-stu-id="f1946-178">Job is pending to be released.</span></span>|
|<span data-ttu-id="f1946-179">interpretar</span><span class="sxs-lookup"><span data-stu-id="f1946-179">interpreting</span></span>|<span data-ttu-id="f1946-180">6 </span><span class="sxs-lookup"><span data-stu-id="f1946-180">6</span></span>|<span data-ttu-id="f1946-181">O trabalho está no estado de "processamento", mas, mais especificamente, a carga do documento está sendo interpretada.</span><span class="sxs-lookup"><span data-stu-id="f1946-181">Job is in 'processing' state, but more specifically, document payload is being interpreted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1946-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1946-182">JSON representation</span></span>

<span data-ttu-id="f1946-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1946-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "state": "String",
    "description": "String",
    "isAcquiredByPrinter": true,    
    "details": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJobStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

