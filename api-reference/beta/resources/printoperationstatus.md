---
title: tipo de recurso printOperationStatus
description: Representa o status atual de uma operação de impressão universal de execução longa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 14c66cf59dc1715a16bd786657202a554d7c1753
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052548"
---
# <a name="printoperationstatus-complex-type"></a><span data-ttu-id="3a5cb-103">tipo complexo printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="3a5cb-103">printOperationStatus complex type</span></span>

<span data-ttu-id="3a5cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a5cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a5cb-105">Representa o status atual de uma operação de impressão universal de execução longa.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-105">Represents the current status of a long-running Universal Print operation.</span></span>

## <a name="properties"></a><span data-ttu-id="3a5cb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a5cb-106">Properties</span></span>
| <span data-ttu-id="3a5cb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a5cb-107">Property</span></span>     | <span data-ttu-id="3a5cb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a5cb-108">Type</span></span>        | <span data-ttu-id="3a5cb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a5cb-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a5cb-110">state</span><span class="sxs-lookup"><span data-stu-id="3a5cb-110">state</span></span>|<span data-ttu-id="3a5cb-111">printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="3a5cb-111">printOperationProcessingState</span></span>|<span data-ttu-id="3a5cb-112">O estado de processamento atual da operação.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-112">The printOperation's current processing state.</span></span> <span data-ttu-id="3a5cb-113">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-113">Valid values are described in the following table.</span></span> <span data-ttu-id="3a5cb-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-114">Read-only.</span></span>|
|<span data-ttu-id="3a5cb-115">description</span><span class="sxs-lookup"><span data-stu-id="3a5cb-115">description</span></span>|<span data-ttu-id="3a5cb-116">String</span><span class="sxs-lookup"><span data-stu-id="3a5cb-116">String</span></span>|<span data-ttu-id="3a5cb-117">Uma descrição legível do estado de processamento atual da operação.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-117">A human-readable description of the printOperation's current processing state.</span></span> <span data-ttu-id="3a5cb-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-118">Read-only.</span></span>|

### <a name="printoperationprocessingstate-values"></a><span data-ttu-id="3a5cb-119">valores de printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="3a5cb-119">printOperationProcessingState values</span></span>

|<span data-ttu-id="3a5cb-120">Membro</span><span class="sxs-lookup"><span data-stu-id="3a5cb-120">Member</span></span>|<span data-ttu-id="3a5cb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3a5cb-121">Value</span></span>|<span data-ttu-id="3a5cb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a5cb-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a5cb-123">notStarted</span><span class="sxs-lookup"><span data-stu-id="3a5cb-123">notStarted</span></span>|<span data-ttu-id="3a5cb-124">,0</span><span class="sxs-lookup"><span data-stu-id="3a5cb-124">0</span></span>|<span data-ttu-id="3a5cb-125">A operação ainda não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-125">The operation has not yet started.</span></span>|
|<span data-ttu-id="3a5cb-126">com</span><span class="sxs-lookup"><span data-stu-id="3a5cb-126">running</span></span>|<span data-ttu-id="3a5cb-127">1 </span><span class="sxs-lookup"><span data-stu-id="3a5cb-127">1</span></span>|<span data-ttu-id="3a5cb-128">A operação está sendo executada.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-128">The operation is running.</span></span>|
|<span data-ttu-id="3a5cb-129">adicionada</span><span class="sxs-lookup"><span data-stu-id="3a5cb-129">succeeded</span></span>|<span data-ttu-id="3a5cb-130">2 </span><span class="sxs-lookup"><span data-stu-id="3a5cb-130">2</span></span>|<span data-ttu-id="3a5cb-131">A operação foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-131">The operation completed successfully.</span></span>|
|<span data-ttu-id="3a5cb-132">falhou</span><span class="sxs-lookup"><span data-stu-id="3a5cb-132">failed</span></span>|<span data-ttu-id="3a5cb-133">3 </span><span class="sxs-lookup"><span data-stu-id="3a5cb-133">3</span></span>|<span data-ttu-id="3a5cb-134">Falha na operação.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-134">The operation failed.</span></span>|
|<span data-ttu-id="3a5cb-135">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="3a5cb-135">unknownFutureValue</span></span>|<span data-ttu-id="3a5cb-136">4 </span><span class="sxs-lookup"><span data-stu-id="3a5cb-136">4</span></span>|<span data-ttu-id="3a5cb-137">Valor de sentinela de enumeração evolvable.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="3a5cb-138">Não usar.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a5cb-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a5cb-139">JSON representation</span></span>

<span data-ttu-id="3a5cb-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a5cb-140">The following is a JSON representation of the resource.</span></span>

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

