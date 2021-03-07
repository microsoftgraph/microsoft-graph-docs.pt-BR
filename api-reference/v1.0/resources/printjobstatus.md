---
title: Tipo de recurso printJobStatus
description: Representa o status atual de um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7a6f5e0c728c1de122f9b642b9de2f1db050cf09
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517036"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="5bc37-103">Tipo de recurso printJobStatus</span><span class="sxs-lookup"><span data-stu-id="5bc37-103">printJobStatus resource type</span></span>

<span data-ttu-id="5bc37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bc37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5bc37-105">Representa o status atual de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="5bc37-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="5bc37-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5bc37-106">Properties</span></span>
|<span data-ttu-id="5bc37-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bc37-107">Property</span></span>|<span data-ttu-id="5bc37-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bc37-108">Type</span></span>|<span data-ttu-id="5bc37-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bc37-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bc37-110">state</span><span class="sxs-lookup"><span data-stu-id="5bc37-110">state</span></span>|<span data-ttu-id="5bc37-111">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="5bc37-111">printJobProcessingState</span></span>|<span data-ttu-id="5bc37-112">O estado de processamento atual do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="5bc37-112">The print job's current processing state.</span></span> <span data-ttu-id="5bc37-113">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5bc37-113">Valid values are described in the following table.</span></span> <span data-ttu-id="5bc37-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5bc37-114">Read-only.</span></span>|
|<span data-ttu-id="5bc37-115">detalhes</span><span class="sxs-lookup"><span data-stu-id="5bc37-115">details</span></span>|<span data-ttu-id="5bc37-116">Coleção printJobProcessingDetail</span><span class="sxs-lookup"><span data-stu-id="5bc37-116">printJobProcessingDetail collection</span></span>|<span data-ttu-id="5bc37-117">Detalhes adicionais para o estado do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="5bc37-117">Additional details for print job state.</span></span> <span data-ttu-id="5bc37-118">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5bc37-118">Valid values are described in the following table.</span></span> <span data-ttu-id="5bc37-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5bc37-119">Read-only.</span></span>|
|<span data-ttu-id="5bc37-120">description</span><span class="sxs-lookup"><span data-stu-id="5bc37-120">description</span></span>|<span data-ttu-id="5bc37-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bc37-121">String</span></span>|<span data-ttu-id="5bc37-122">Uma descrição aceitável para humanos do estado de processamento atual do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="5bc37-122">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="5bc37-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5bc37-123">Read-only.</span></span>|
|<span data-ttu-id="5bc37-124">isAcquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="5bc37-124">isAcquiredByPrinter</span></span>|<span data-ttu-id="5bc37-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="5bc37-125">Boolean</span></span>|<span data-ttu-id="5bc37-126">True se o trabalho foi reconhecido por uma impressora; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="5bc37-126">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="5bc37-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5bc37-127">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="5bc37-128">valores printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="5bc37-128">printJobProcessingState values</span></span>

|<span data-ttu-id="5bc37-129">Membro</span><span class="sxs-lookup"><span data-stu-id="5bc37-129">Member</span></span>|<span data-ttu-id="5bc37-130">Valor</span><span class="sxs-lookup"><span data-stu-id="5bc37-130">Value</span></span>|<span data-ttu-id="5bc37-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bc37-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bc37-132">desconhecido</span><span class="sxs-lookup"><span data-stu-id="5bc37-132">unknown</span></span>|<span data-ttu-id="5bc37-133">0</span><span class="sxs-lookup"><span data-stu-id="5bc37-133">0</span></span>|<span data-ttu-id="5bc37-134">O estado de processamento relatado pela impressora não é reconhecido.</span><span class="sxs-lookup"><span data-stu-id="5bc37-134">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="5bc37-135">pendente</span><span class="sxs-lookup"><span data-stu-id="5bc37-135">pending</span></span>|<span data-ttu-id="5bc37-136">1 </span><span class="sxs-lookup"><span data-stu-id="5bc37-136">1</span></span>|<span data-ttu-id="5bc37-137">O trabalho de impressão está aguardando processamento pela impressora.</span><span class="sxs-lookup"><span data-stu-id="5bc37-137">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="5bc37-138">processamento</span><span class="sxs-lookup"><span data-stu-id="5bc37-138">processing</span></span>|<span data-ttu-id="5bc37-139">2 </span><span class="sxs-lookup"><span data-stu-id="5bc37-139">2</span></span>|<span data-ttu-id="5bc37-140">O trabalho de impressão está sendo processado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="5bc37-140">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="5bc37-141">pausado</span><span class="sxs-lookup"><span data-stu-id="5bc37-141">paused</span></span>|<span data-ttu-id="5bc37-142">3 </span><span class="sxs-lookup"><span data-stu-id="5bc37-142">3</span></span>|<span data-ttu-id="5bc37-143">O trabalho de impressão foi pausado.</span><span class="sxs-lookup"><span data-stu-id="5bc37-143">The print job has been paused.</span></span>|
|<span data-ttu-id="5bc37-144">stopped</span><span class="sxs-lookup"><span data-stu-id="5bc37-144">stopped</span></span>|<span data-ttu-id="5bc37-145">4 </span><span class="sxs-lookup"><span data-stu-id="5bc37-145">4</span></span>|<span data-ttu-id="5bc37-146">O trabalho de impressão foi interrompido porque um problema com a impressora precisa ser resolvido antes que o trabalho possa continuar.</span><span class="sxs-lookup"><span data-stu-id="5bc37-146">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="5bc37-147">Mais informações podem ser encontradas no recurso estado da impressora.</span><span class="sxs-lookup"><span data-stu-id="5bc37-147">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="5bc37-148">completed</span><span class="sxs-lookup"><span data-stu-id="5bc37-148">completed</span></span>|<span data-ttu-id="5bc37-149">5 </span><span class="sxs-lookup"><span data-stu-id="5bc37-149">5</span></span>|<span data-ttu-id="5bc37-150">O trabalho de impressão foi concluído com êxito e nenhum processamento posterior ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="5bc37-150">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="5bc37-151">cancelado</span><span class="sxs-lookup"><span data-stu-id="5bc37-151">canceled</span></span>|<span data-ttu-id="5bc37-152">6 </span><span class="sxs-lookup"><span data-stu-id="5bc37-152">6</span></span>|<span data-ttu-id="5bc37-153">O trabalho de impressão foi cancelado por um usuário e nenhum outro processamento ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="5bc37-153">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="5bc37-154">abortado</span><span class="sxs-lookup"><span data-stu-id="5bc37-154">aborted</span></span>|<span data-ttu-id="5bc37-155">7 </span><span class="sxs-lookup"><span data-stu-id="5bc37-155">7</span></span>|<span data-ttu-id="5bc37-156">O trabalho de impressão foi abortado por um usuário ou pela impressora e nenhum outro processamento ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="5bc37-156">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

### <a name="printjobprocessingdetail-values"></a><span data-ttu-id="5bc37-157">valores printJobProcessingDetail</span><span class="sxs-lookup"><span data-stu-id="5bc37-157">printJobProcessingDetail values</span></span>

|<span data-ttu-id="5bc37-158">Membro</span><span class="sxs-lookup"><span data-stu-id="5bc37-158">Member</span></span>|<span data-ttu-id="5bc37-159">Valor</span><span class="sxs-lookup"><span data-stu-id="5bc37-159">Value</span></span>|<span data-ttu-id="5bc37-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bc37-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bc37-161">uploadPending</span><span class="sxs-lookup"><span data-stu-id="5bc37-161">uploadPending</span></span>|<span data-ttu-id="5bc37-162">0</span><span class="sxs-lookup"><span data-stu-id="5bc37-162">0</span></span>|<span data-ttu-id="5bc37-163">A carga do documento não foi carregada.</span><span class="sxs-lookup"><span data-stu-id="5bc37-163">Document payload has not been uploaded.</span></span>|
|<span data-ttu-id="5bc37-164">transformando</span><span class="sxs-lookup"><span data-stu-id="5bc37-164">transforming</span></span>|<span data-ttu-id="5bc37-165">1 </span><span class="sxs-lookup"><span data-stu-id="5bc37-165">1</span></span>|<span data-ttu-id="5bc37-166">A carga do documento está sendo transformada.</span><span class="sxs-lookup"><span data-stu-id="5bc37-166">Document payload is being transformed.</span></span>|
|<span data-ttu-id="5bc37-167">completedSuccessfully</span><span class="sxs-lookup"><span data-stu-id="5bc37-167">completedSuccessfully</span></span>|<span data-ttu-id="5bc37-168">2 </span><span class="sxs-lookup"><span data-stu-id="5bc37-168">2</span></span>|<span data-ttu-id="5bc37-169">O trabalho foi concluído com êxito.</span><span class="sxs-lookup"><span data-stu-id="5bc37-169">Job has been completed successfully.</span></span>|
|<span data-ttu-id="5bc37-170">completedWithWarnings</span><span class="sxs-lookup"><span data-stu-id="5bc37-170">completedWithWarnings</span></span>|<span data-ttu-id="5bc37-171">3 </span><span class="sxs-lookup"><span data-stu-id="5bc37-171">3</span></span>|<span data-ttu-id="5bc37-172">O trabalho foi concluído com avisos.</span><span class="sxs-lookup"><span data-stu-id="5bc37-172">Job has been completed with warnings.</span></span>|
|<span data-ttu-id="5bc37-173">completedWithErrors</span><span class="sxs-lookup"><span data-stu-id="5bc37-173">completedWithErrors</span></span>|<span data-ttu-id="5bc37-174">4 </span><span class="sxs-lookup"><span data-stu-id="5bc37-174">4</span></span>|<span data-ttu-id="5bc37-175">O trabalho foi concluído com erros.</span><span class="sxs-lookup"><span data-stu-id="5bc37-175">Job has been completed with errors.</span></span>|
|<span data-ttu-id="5bc37-176">releaseWait</span><span class="sxs-lookup"><span data-stu-id="5bc37-176">releaseWait</span></span>|<span data-ttu-id="5bc37-177">5 </span><span class="sxs-lookup"><span data-stu-id="5bc37-177">5</span></span>|<span data-ttu-id="5bc37-178">O trabalho está pendente para ser liberado.</span><span class="sxs-lookup"><span data-stu-id="5bc37-178">Job is pending to be released.</span></span>|
|<span data-ttu-id="5bc37-179">interpretando</span><span class="sxs-lookup"><span data-stu-id="5bc37-179">interpreting</span></span>|<span data-ttu-id="5bc37-180">6 </span><span class="sxs-lookup"><span data-stu-id="5bc37-180">6</span></span>|<span data-ttu-id="5bc37-181">O trabalho está em estado de 'processamento', mas, mais especificamente, a carga do documento está sendo interpretada.</span><span class="sxs-lookup"><span data-stu-id="5bc37-181">Job is in 'processing' state, but more specifically, document payload is being interpreted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bc37-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5bc37-182">JSON representation</span></span>
<span data-ttu-id="5bc37-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5bc37-183">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobStatus",
  "state": "String",
  "description": "String",
  "isAcquiredByPrinter": "Boolean",
  "details": [
    "String"
  ]
}
```

