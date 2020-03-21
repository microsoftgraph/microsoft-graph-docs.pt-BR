---
title: tipo de recurso printJobStatus
description: Representa o status atual de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 1973d00ff8ca544f0acd1992626de9a3eaf59700
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895476"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="5a1e8-103">tipo de recurso printJobStatus</span><span class="sxs-lookup"><span data-stu-id="5a1e8-103">printJobStatus resource type</span></span>

<span data-ttu-id="5a1e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a1e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a1e8-105">Representa o status atual de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="5a1e8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a1e8-106">Properties</span></span>
| <span data-ttu-id="5a1e8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a1e8-107">Property</span></span>     | <span data-ttu-id="5a1e8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a1e8-108">Type</span></span>        | <span data-ttu-id="5a1e8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a1e8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a1e8-110">ProcessingState</span><span class="sxs-lookup"><span data-stu-id="5a1e8-110">processingState</span></span>|<span data-ttu-id="5a1e8-111">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="5a1e8-111">printJobProcessingState</span></span>|<span data-ttu-id="5a1e8-112">O estado atual de processamento do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-112">The print job's current processing state.</span></span> <span data-ttu-id="5a1e8-113">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-113">Valid values are described in the following table.</span></span> <span data-ttu-id="5a1e8-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-114">Read-only.</span></span>|
|<span data-ttu-id="5a1e8-115">processingStateDescription</span><span class="sxs-lookup"><span data-stu-id="5a1e8-115">processingStateDescription</span></span>|<span data-ttu-id="5a1e8-116">String</span><span class="sxs-lookup"><span data-stu-id="5a1e8-116">String</span></span>|<span data-ttu-id="5a1e8-117">Uma descrição legível do estado de processamento atual do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-117">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="5a1e8-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-118">Read-only.</span></span>|
|<span data-ttu-id="5a1e8-119">acquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="5a1e8-119">acquiredByPrinter</span></span>|<span data-ttu-id="5a1e8-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a1e8-120">Boolean</span></span>|<span data-ttu-id="5a1e8-121">True se o trabalho foi confirmado por uma impressora; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-121">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="5a1e8-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-122">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="5a1e8-123">valores de printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="5a1e8-123">printJobProcessingState values</span></span>

|<span data-ttu-id="5a1e8-124">Membro</span><span class="sxs-lookup"><span data-stu-id="5a1e8-124">Member</span></span>|<span data-ttu-id="5a1e8-125">Valor</span><span class="sxs-lookup"><span data-stu-id="5a1e8-125">Value</span></span>|<span data-ttu-id="5a1e8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a1e8-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a1e8-127">desconhecido</span><span class="sxs-lookup"><span data-stu-id="5a1e8-127">unknown</span></span>|<span data-ttu-id="5a1e8-128">,0</span><span class="sxs-lookup"><span data-stu-id="5a1e8-128">0</span></span>|<span data-ttu-id="5a1e8-129">O estado de processamento relatado pela impressora não é reconhecido.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-129">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="5a1e8-130">função</span><span class="sxs-lookup"><span data-stu-id="5a1e8-130">pending</span></span>|<span data-ttu-id="5a1e8-131">1</span><span class="sxs-lookup"><span data-stu-id="5a1e8-131">1</span></span>|<span data-ttu-id="5a1e8-132">O trabalho de impressão está aguardando o processamento da impressora.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-132">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="5a1e8-133">pendingHeld</span><span class="sxs-lookup"><span data-stu-id="5a1e8-133">pendingHeld</span></span>|<span data-ttu-id="5a1e8-134">duas</span><span class="sxs-lookup"><span data-stu-id="5a1e8-134">2</span></span>|<span data-ttu-id="5a1e8-135">O trabalho ainda não é um candidato para processamento.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-135">The job is not a candidate for processing yet.</span></span> <span data-ttu-id="5a1e8-136">Certifique-se de que não haja erros ou limitações de recursos que impeçam o início do trabalho.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-136">Ensure that there are no errors or resource limitations preventing the job from starting.</span></span>|
|<span data-ttu-id="5a1e8-137">processe</span><span class="sxs-lookup"><span data-stu-id="5a1e8-137">processing</span></span>|<span data-ttu-id="5a1e8-138">3D</span><span class="sxs-lookup"><span data-stu-id="5a1e8-138">3</span></span>|<span data-ttu-id="5a1e8-139">O trabalho de impressão está sendo processado pela impressora no momento.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-139">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="5a1e8-140">pausado</span><span class="sxs-lookup"><span data-stu-id="5a1e8-140">paused</span></span>|<span data-ttu-id="5a1e8-141">4 </span><span class="sxs-lookup"><span data-stu-id="5a1e8-141">4</span></span>|<span data-ttu-id="5a1e8-142">O trabalho de impressão foi pausado por um usuário.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-142">The print job has been paused by a user.</span></span>|
|<span data-ttu-id="5a1e8-143">parar</span><span class="sxs-lookup"><span data-stu-id="5a1e8-143">stopped</span></span>|<span data-ttu-id="5a1e8-144">5 </span><span class="sxs-lookup"><span data-stu-id="5a1e8-144">5</span></span>|<span data-ttu-id="5a1e8-145">O trabalho de impressão foi interrompido porque um problema com a impressora precisa ser resolvido para que o trabalho possa continuar.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-145">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="5a1e8-146">Mais informações podem ser encontradas no recurso de estado da impressora.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-146">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="5a1e8-147">Completed</span><span class="sxs-lookup"><span data-stu-id="5a1e8-147">completed</span></span>|<span data-ttu-id="5a1e8-148">6 </span><span class="sxs-lookup"><span data-stu-id="5a1e8-148">6</span></span>|<span data-ttu-id="5a1e8-149">O trabalho de impressão foi concluído com êxito e nenhum processamento adicional ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-149">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="5a1e8-150">foi</span><span class="sxs-lookup"><span data-stu-id="5a1e8-150">canceled</span></span>|<span data-ttu-id="5a1e8-151">7 </span><span class="sxs-lookup"><span data-stu-id="5a1e8-151">7</span></span>|<span data-ttu-id="5a1e8-152">O trabalho de impressão foi cancelado por um usuário e nenhum processamento adicional ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-152">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="5a1e8-153">anulada</span><span class="sxs-lookup"><span data-stu-id="5a1e8-153">aborted</span></span>|<span data-ttu-id="5a1e8-154">8 </span><span class="sxs-lookup"><span data-stu-id="5a1e8-154">8</span></span>|<span data-ttu-id="5a1e8-155">O trabalho de impressão foi anulado por um usuário ou pela impressora e nenhum processamento adicional ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-155">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a1e8-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a1e8-156">JSON representation</span></span>

<span data-ttu-id="5a1e8-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a1e8-157">The following is a JSON representation of the resource.</span></span>

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