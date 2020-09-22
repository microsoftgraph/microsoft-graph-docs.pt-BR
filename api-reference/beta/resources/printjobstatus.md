---
title: tipo de recurso printJobStatus
description: Representa o status atual de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bebf2081dafe6412a22b66b8a371b67ba0e53548
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048734"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="01bf5-103">tipo de recurso printJobStatus</span><span class="sxs-lookup"><span data-stu-id="01bf5-103">printJobStatus resource type</span></span>

<span data-ttu-id="01bf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01bf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01bf5-105">Representa o status atual de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="01bf5-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="01bf5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01bf5-106">Properties</span></span>
| <span data-ttu-id="01bf5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01bf5-107">Property</span></span>     | <span data-ttu-id="01bf5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="01bf5-108">Type</span></span>        | <span data-ttu-id="01bf5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="01bf5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="01bf5-110">ProcessingState</span><span class="sxs-lookup"><span data-stu-id="01bf5-110">processingState</span></span>|<span data-ttu-id="01bf5-111">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="01bf5-111">printJobProcessingState</span></span>|<span data-ttu-id="01bf5-112">O estado atual de processamento do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="01bf5-112">The print job's current processing state.</span></span> <span data-ttu-id="01bf5-113">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="01bf5-113">Valid values are described in the following table.</span></span> <span data-ttu-id="01bf5-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01bf5-114">Read-only.</span></span>|
|<span data-ttu-id="01bf5-115">processingStateDescription</span><span class="sxs-lookup"><span data-stu-id="01bf5-115">processingStateDescription</span></span>|<span data-ttu-id="01bf5-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01bf5-116">String</span></span>|<span data-ttu-id="01bf5-117">Uma descrição legível do estado de processamento atual do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="01bf5-117">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="01bf5-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01bf5-118">Read-only.</span></span>|
|<span data-ttu-id="01bf5-119">acquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="01bf5-119">acquiredByPrinter</span></span>|<span data-ttu-id="01bf5-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="01bf5-120">Boolean</span></span>|<span data-ttu-id="01bf5-121">True se o trabalho foi confirmado por uma impressora; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="01bf5-121">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="01bf5-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01bf5-122">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="01bf5-123">valores de printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="01bf5-123">printJobProcessingState values</span></span>

|<span data-ttu-id="01bf5-124">Membro</span><span class="sxs-lookup"><span data-stu-id="01bf5-124">Member</span></span>|<span data-ttu-id="01bf5-125">Valor</span><span class="sxs-lookup"><span data-stu-id="01bf5-125">Value</span></span>|<span data-ttu-id="01bf5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="01bf5-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01bf5-127">desconhecido</span><span class="sxs-lookup"><span data-stu-id="01bf5-127">unknown</span></span>|<span data-ttu-id="01bf5-128">,0</span><span class="sxs-lookup"><span data-stu-id="01bf5-128">0</span></span>|<span data-ttu-id="01bf5-129">O estado de processamento relatado pela impressora não é reconhecido.</span><span class="sxs-lookup"><span data-stu-id="01bf5-129">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="01bf5-130">função</span><span class="sxs-lookup"><span data-stu-id="01bf5-130">pending</span></span>|<span data-ttu-id="01bf5-131">1 </span><span class="sxs-lookup"><span data-stu-id="01bf5-131">1</span></span>|<span data-ttu-id="01bf5-132">O trabalho de impressão está aguardando o processamento da impressora.</span><span class="sxs-lookup"><span data-stu-id="01bf5-132">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="01bf5-133">pendingHeld</span><span class="sxs-lookup"><span data-stu-id="01bf5-133">pendingHeld</span></span>|<span data-ttu-id="01bf5-134">2 </span><span class="sxs-lookup"><span data-stu-id="01bf5-134">2</span></span>|<span data-ttu-id="01bf5-135">O trabalho ainda não é um candidato para processamento.</span><span class="sxs-lookup"><span data-stu-id="01bf5-135">The job is not a candidate for processing yet.</span></span> <span data-ttu-id="01bf5-136">Certifique-se de que não haja erros ou limitações de recursos que impeçam o início do trabalho.</span><span class="sxs-lookup"><span data-stu-id="01bf5-136">Ensure that there are no errors or resource limitations preventing the job from starting.</span></span>|
|<span data-ttu-id="01bf5-137">processe</span><span class="sxs-lookup"><span data-stu-id="01bf5-137">processing</span></span>|<span data-ttu-id="01bf5-138">3 </span><span class="sxs-lookup"><span data-stu-id="01bf5-138">3</span></span>|<span data-ttu-id="01bf5-139">O trabalho de impressão está sendo processado pela impressora no momento.</span><span class="sxs-lookup"><span data-stu-id="01bf5-139">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="01bf5-140">pausado</span><span class="sxs-lookup"><span data-stu-id="01bf5-140">paused</span></span>|<span data-ttu-id="01bf5-141">4 </span><span class="sxs-lookup"><span data-stu-id="01bf5-141">4</span></span>|<span data-ttu-id="01bf5-142">O trabalho de impressão foi pausado por um usuário.</span><span class="sxs-lookup"><span data-stu-id="01bf5-142">The print job has been paused by a user.</span></span>|
|<span data-ttu-id="01bf5-143">parar</span><span class="sxs-lookup"><span data-stu-id="01bf5-143">stopped</span></span>|<span data-ttu-id="01bf5-144">5 </span><span class="sxs-lookup"><span data-stu-id="01bf5-144">5</span></span>|<span data-ttu-id="01bf5-145">O trabalho de impressão foi interrompido porque um problema com a impressora precisa ser resolvido para que o trabalho possa continuar.</span><span class="sxs-lookup"><span data-stu-id="01bf5-145">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="01bf5-146">Mais informações podem ser encontradas no recurso de estado da impressora.</span><span class="sxs-lookup"><span data-stu-id="01bf5-146">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="01bf5-147">Completed</span><span class="sxs-lookup"><span data-stu-id="01bf5-147">completed</span></span>|<span data-ttu-id="01bf5-148">6 </span><span class="sxs-lookup"><span data-stu-id="01bf5-148">6</span></span>|<span data-ttu-id="01bf5-149">O trabalho de impressão foi concluído com êxito e nenhum processamento adicional ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="01bf5-149">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="01bf5-150">foi</span><span class="sxs-lookup"><span data-stu-id="01bf5-150">canceled</span></span>|<span data-ttu-id="01bf5-151">7 </span><span class="sxs-lookup"><span data-stu-id="01bf5-151">7</span></span>|<span data-ttu-id="01bf5-152">O trabalho de impressão foi cancelado por um usuário e nenhum processamento adicional ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="01bf5-152">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="01bf5-153">anulada</span><span class="sxs-lookup"><span data-stu-id="01bf5-153">aborted</span></span>|<span data-ttu-id="01bf5-154">8 </span><span class="sxs-lookup"><span data-stu-id="01bf5-154">8</span></span>|<span data-ttu-id="01bf5-155">O trabalho de impressão foi anulado por um usuário ou pela impressora e nenhum processamento adicional ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="01bf5-155">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01bf5-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01bf5-156">JSON representation</span></span>

<span data-ttu-id="01bf5-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01bf5-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "processingState": "String",
    "processingStateDescription": "String",
    "acquiredByPrinter": true
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

