---
title: Tipo de recurso printOperationStatus
description: Representa o status atual de uma operação de Impressão Universal de longa duração.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 787a584b32c6f34d78d14fa4d676b1be30a62c25
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516865"
---
# <a name="printoperationstatus-resource-type"></a><span data-ttu-id="1e467-103">Tipo de recurso printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="1e467-103">printOperationStatus resource type</span></span>

<span data-ttu-id="1e467-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e467-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="1e467-105">Representa o status atual de uma operação de Impressão Universal de longa duração.</span><span class="sxs-lookup"><span data-stu-id="1e467-105">Represents the current status of a long-running Universal Print operation.</span></span>

## <a name="properties"></a><span data-ttu-id="1e467-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e467-106">Properties</span></span>
|<span data-ttu-id="1e467-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e467-107">Property</span></span>|<span data-ttu-id="1e467-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e467-108">Type</span></span>|<span data-ttu-id="1e467-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e467-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e467-110">state</span><span class="sxs-lookup"><span data-stu-id="1e467-110">state</span></span>|<span data-ttu-id="1e467-111">printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="1e467-111">printOperationProcessingState</span></span>|<span data-ttu-id="1e467-112">O estado de processamento atual da printOperation.</span><span class="sxs-lookup"><span data-stu-id="1e467-112">The printOperation's current processing state.</span></span> <span data-ttu-id="1e467-113">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1e467-113">Valid values are described in the following table.</span></span> <span data-ttu-id="1e467-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e467-114">Read-only.</span></span>|
|<span data-ttu-id="1e467-115">description</span><span class="sxs-lookup"><span data-stu-id="1e467-115">description</span></span>|<span data-ttu-id="1e467-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e467-116">String</span></span>|<span data-ttu-id="1e467-117">Uma descrição aceitável para humanos do estado de processamento atual do printOperation.</span><span class="sxs-lookup"><span data-stu-id="1e467-117">A human-readable description of the printOperation's current processing state.</span></span> <span data-ttu-id="1e467-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e467-118">Read-only.</span></span>|

### <a name="printoperationprocessingstate-values"></a><span data-ttu-id="1e467-119">valores printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="1e467-119">printOperationProcessingState values</span></span>

|<span data-ttu-id="1e467-120">Membro</span><span class="sxs-lookup"><span data-stu-id="1e467-120">Member</span></span>|<span data-ttu-id="1e467-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e467-121">Value</span></span>|<span data-ttu-id="1e467-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e467-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e467-123">notStarted</span><span class="sxs-lookup"><span data-stu-id="1e467-123">notStarted</span></span>|<span data-ttu-id="1e467-124">0</span><span class="sxs-lookup"><span data-stu-id="1e467-124">0</span></span>|<span data-ttu-id="1e467-125">A operação ainda não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="1e467-125">The operation has not yet started.</span></span>|
|<span data-ttu-id="1e467-126">running</span><span class="sxs-lookup"><span data-stu-id="1e467-126">running</span></span>|<span data-ttu-id="1e467-127">1 </span><span class="sxs-lookup"><span data-stu-id="1e467-127">1</span></span>|<span data-ttu-id="1e467-128">A operação está em execução.</span><span class="sxs-lookup"><span data-stu-id="1e467-128">The operation is running.</span></span>|
|<span data-ttu-id="1e467-129">bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="1e467-129">succeeded</span></span>|<span data-ttu-id="1e467-130">2 </span><span class="sxs-lookup"><span data-stu-id="1e467-130">2</span></span>|<span data-ttu-id="1e467-131">A operação foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="1e467-131">The operation completed successfully.</span></span>|
|<span data-ttu-id="1e467-132">failed</span><span class="sxs-lookup"><span data-stu-id="1e467-132">failed</span></span>|<span data-ttu-id="1e467-133">3 </span><span class="sxs-lookup"><span data-stu-id="1e467-133">3</span></span>|<span data-ttu-id="1e467-134">Falha na operação.</span><span class="sxs-lookup"><span data-stu-id="1e467-134">The operation failed.</span></span>|
|<span data-ttu-id="1e467-135">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="1e467-135">unknownFutureValue</span></span>|<span data-ttu-id="1e467-136">4 </span><span class="sxs-lookup"><span data-stu-id="1e467-136">4</span></span>|<span data-ttu-id="1e467-137">Valor de sentinela de enumeração evolvável.</span><span class="sxs-lookup"><span data-stu-id="1e467-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="1e467-138">Não usar.</span><span class="sxs-lookup"><span data-stu-id="1e467-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e467-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e467-139">JSON representation</span></span>
<span data-ttu-id="1e467-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e467-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printOperationStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperationStatus",
  "state": "String",
  "description": "String"
}
```

