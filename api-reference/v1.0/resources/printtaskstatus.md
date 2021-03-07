---
title: Tipo de recurso printTaskStatus
description: Representa o status de execução atual de um printTask.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ef5587050926fef5fa924f6d541de63d5b1d33aa
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517014"
---
# <a name="printtaskstatus-resource-type"></a><span data-ttu-id="c606a-103">Tipo de recurso printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="c606a-103">printTaskStatus resource type</span></span>

<span data-ttu-id="c606a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c606a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c606a-105">Representa o status de execução atual de [um printTask](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="c606a-105">Represents the current execution status of a [printTask](printtask.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="c606a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c606a-106">Properties</span></span>
|<span data-ttu-id="c606a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c606a-107">Property</span></span>|<span data-ttu-id="c606a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c606a-108">Type</span></span>|<span data-ttu-id="c606a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c606a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c606a-110">state</span><span class="sxs-lookup"><span data-stu-id="c606a-110">state</span></span>|<span data-ttu-id="c606a-111">printTaskProcessingState</span><span class="sxs-lookup"><span data-stu-id="c606a-111">printTaskProcessingState</span></span>|<span data-ttu-id="c606a-112">O estado de processamento atual do [printTask](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="c606a-112">The current processing state of the [printTask](printtask.md).</span></span> <span data-ttu-id="c606a-113">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c606a-113">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="c606a-114">description</span><span class="sxs-lookup"><span data-stu-id="c606a-114">description</span></span>|<span data-ttu-id="c606a-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c606a-115">String</span></span>|<span data-ttu-id="c606a-116">Uma descrição aceitável para humanos do estado de processamento atual do [printTask](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="c606a-116">A human-readable description of the current processing state of the [printTask](printtask.md).</span></span>|

### <a name="printtaskprocessingstate-values"></a><span data-ttu-id="c606a-117">valores printTaskProcessingState</span><span class="sxs-lookup"><span data-stu-id="c606a-117">printTaskProcessingState values</span></span>

|<span data-ttu-id="c606a-118">Membro</span><span class="sxs-lookup"><span data-stu-id="c606a-118">Member</span></span>|<span data-ttu-id="c606a-119">Valor</span><span class="sxs-lookup"><span data-stu-id="c606a-119">Value</span></span>|<span data-ttu-id="c606a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c606a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c606a-121">pendente</span><span class="sxs-lookup"><span data-stu-id="c606a-121">pending</span></span>|<span data-ttu-id="c606a-122">0</span><span class="sxs-lookup"><span data-stu-id="c606a-122">0</span></span>|<span data-ttu-id="c606a-123">A execução da tarefa está pendente.</span><span class="sxs-lookup"><span data-stu-id="c606a-123">Task execution is pending.</span></span>|
|<span data-ttu-id="c606a-124">processamento</span><span class="sxs-lookup"><span data-stu-id="c606a-124">processing</span></span>|<span data-ttu-id="c606a-125">1 </span><span class="sxs-lookup"><span data-stu-id="c606a-125">1</span></span>|<span data-ttu-id="c606a-126">A execução da tarefa está em andamento.</span><span class="sxs-lookup"><span data-stu-id="c606a-126">Task execution is in progress.</span></span>|
|<span data-ttu-id="c606a-127">completed</span><span class="sxs-lookup"><span data-stu-id="c606a-127">completed</span></span>|<span data-ttu-id="c606a-128">2 </span><span class="sxs-lookup"><span data-stu-id="c606a-128">2</span></span>|<span data-ttu-id="c606a-129">A execução da tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="c606a-129">Task execution has completed.</span></span>|
|<span data-ttu-id="c606a-130">abortado</span><span class="sxs-lookup"><span data-stu-id="c606a-130">aborted</span></span>|<span data-ttu-id="c606a-131">3 </span><span class="sxs-lookup"><span data-stu-id="c606a-131">3</span></span>|<span data-ttu-id="c606a-132">A execução da tarefa foi abortada.</span><span class="sxs-lookup"><span data-stu-id="c606a-132">Task execution was aborted.</span></span>|
|<span data-ttu-id="c606a-133">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="c606a-133">unknownFutureValue</span></span>|<span data-ttu-id="c606a-134">4 </span><span class="sxs-lookup"><span data-stu-id="c606a-134">4</span></span>|<span data-ttu-id="c606a-135">Valor de sentinela de enumeração evolvável.</span><span class="sxs-lookup"><span data-stu-id="c606a-135">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="c606a-136">Não usar.</span><span class="sxs-lookup"><span data-stu-id="c606a-136">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c606a-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c606a-137">JSON representation</span></span>
<span data-ttu-id="c606a-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c606a-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printTaskStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskStatus",
  "state": "String",
  "description": "String"
}
```

