---
title: tipo de recurso printOperationStatus
description: Representa o status atual de uma operação de impressão universal de execução longa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a7400a3170b104646607c16852a796d01b64200e
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007146"
---
# <a name="printoperationstatus-complex-type"></a><span data-ttu-id="61508-103">tipo complexo printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="61508-103">printOperationStatus complex type</span></span>

<span data-ttu-id="61508-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61508-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61508-105">Representa o status atual de uma operação de impressão universal de execução longa.</span><span class="sxs-lookup"><span data-stu-id="61508-105">Represents the current status of a long-running Universal Print operation.</span></span>

## <a name="properties"></a><span data-ttu-id="61508-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61508-106">Properties</span></span>
| <span data-ttu-id="61508-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61508-107">Property</span></span>     | <span data-ttu-id="61508-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="61508-108">Type</span></span>        | <span data-ttu-id="61508-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="61508-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61508-110">state</span><span class="sxs-lookup"><span data-stu-id="61508-110">state</span></span>|<span data-ttu-id="61508-111">printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="61508-111">printOperationProcessingState</span></span>|<span data-ttu-id="61508-112">O estado de processamento atual da operação.</span><span class="sxs-lookup"><span data-stu-id="61508-112">The printOperation's current processing state.</span></span> <span data-ttu-id="61508-113">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="61508-113">Valid values are described in the following table.</span></span> <span data-ttu-id="61508-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61508-114">Read-only.</span></span>|
|<span data-ttu-id="61508-115">description</span><span class="sxs-lookup"><span data-stu-id="61508-115">description</span></span>|<span data-ttu-id="61508-116">String</span><span class="sxs-lookup"><span data-stu-id="61508-116">String</span></span>|<span data-ttu-id="61508-117">Uma descrição legível do estado de processamento atual da operação.</span><span class="sxs-lookup"><span data-stu-id="61508-117">A human-readable description of the printOperation's current processing state.</span></span> <span data-ttu-id="61508-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61508-118">Read-only.</span></span>|

### <a name="printoperationprocessingstate-values"></a><span data-ttu-id="61508-119">valores de printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="61508-119">printOperationProcessingState values</span></span>

|<span data-ttu-id="61508-120">Membro</span><span class="sxs-lookup"><span data-stu-id="61508-120">Member</span></span>|<span data-ttu-id="61508-121">Valor</span><span class="sxs-lookup"><span data-stu-id="61508-121">Value</span></span>|<span data-ttu-id="61508-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="61508-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61508-123">notStarted</span><span class="sxs-lookup"><span data-stu-id="61508-123">notStarted</span></span>|<span data-ttu-id="61508-124">,0</span><span class="sxs-lookup"><span data-stu-id="61508-124">0</span></span>|<span data-ttu-id="61508-125">A operação ainda não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="61508-125">The operation has not yet started.</span></span>|
|<span data-ttu-id="61508-126">com</span><span class="sxs-lookup"><span data-stu-id="61508-126">running</span></span>|<span data-ttu-id="61508-127">1 </span><span class="sxs-lookup"><span data-stu-id="61508-127">1</span></span>|<span data-ttu-id="61508-128">A operação está sendo executada.</span><span class="sxs-lookup"><span data-stu-id="61508-128">The operation is running.</span></span>|
|<span data-ttu-id="61508-129">adicionada</span><span class="sxs-lookup"><span data-stu-id="61508-129">succeeded</span></span>|<span data-ttu-id="61508-130">2 </span><span class="sxs-lookup"><span data-stu-id="61508-130">2</span></span>|<span data-ttu-id="61508-131">A operação foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="61508-131">The operation completed successfully.</span></span>|
|<span data-ttu-id="61508-132">falhou</span><span class="sxs-lookup"><span data-stu-id="61508-132">failed</span></span>|<span data-ttu-id="61508-133">3 </span><span class="sxs-lookup"><span data-stu-id="61508-133">3</span></span>|<span data-ttu-id="61508-134">Falha na operação.</span><span class="sxs-lookup"><span data-stu-id="61508-134">The operation failed.</span></span>|
|<span data-ttu-id="61508-135">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="61508-135">unknownFutureValue</span></span>|<span data-ttu-id="61508-136">4 </span><span class="sxs-lookup"><span data-stu-id="61508-136">4</span></span>|<span data-ttu-id="61508-137">Valor de sentinela de enumeração evolvable.</span><span class="sxs-lookup"><span data-stu-id="61508-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="61508-138">Não usar.</span><span class="sxs-lookup"><span data-stu-id="61508-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61508-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61508-139">JSON representation</span></span>

<span data-ttu-id="61508-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61508-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperationStatus"
}-->

```json
{
    "state": "String",
    "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->