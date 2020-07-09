---
title: tipo de recurso printTaskStatus
description: Representa o status de execução atual de uma multitarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c5d46cd0c8d14b6dc07873bc503d024928e2b2e3
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091547"
---
# <a name="printtaskstatus-resource-type"></a><span data-ttu-id="ff799-103">tipo de recurso printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="ff799-103">printTaskStatus resource type</span></span>

<span data-ttu-id="ff799-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff799-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff799-105">Representa o status de execução atual de uma [multitarefa](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="ff799-105">Represents the current execution status of a [printTask](printtask.md).</span></span> 

><span data-ttu-id="ff799-106">**Observação:** Os aplicativos que registram gatilhos de tarefa são responsáveis por atualizar os status da tarefa quando o processamento for concluído, a menos que o trabalho de impressão relacionado tenha sido Redirecionado para outra impressora.</span><span class="sxs-lookup"><span data-stu-id="ff799-106">**Note:** Applications that register task triggers are responsible for updating task statuses when processing is finished, unless the related print job has been redirected to another printer.</span></span>

<span data-ttu-id="ff799-107">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="ff799-107">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="properties"></a><span data-ttu-id="ff799-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff799-108">Properties</span></span>
| <span data-ttu-id="ff799-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff799-109">Property</span></span>     | <span data-ttu-id="ff799-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff799-110">Type</span></span>        | <span data-ttu-id="ff799-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff799-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff799-112">state</span><span class="sxs-lookup"><span data-stu-id="ff799-112">state</span></span>|<span data-ttu-id="ff799-113">printTaskProcessingState</span><span class="sxs-lookup"><span data-stu-id="ff799-113">printTaskProcessingState</span></span>|<span data-ttu-id="ff799-114">O estado de processamento atual da [multitarefa](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="ff799-114">The current processing state of the [printTask](printtask.md).</span></span> <span data-ttu-id="ff799-115">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="ff799-115">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="ff799-116">description</span><span class="sxs-lookup"><span data-stu-id="ff799-116">description</span></span>|<span data-ttu-id="ff799-117">String</span><span class="sxs-lookup"><span data-stu-id="ff799-117">String</span></span>|<span data-ttu-id="ff799-118">Uma descrição legível do estado atual de processamento da [tarefa](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="ff799-118">A human-readable description of the current processing state of the [printTask](printtask.md).</span></span>|

### <a name="printtaskprocessingstate-values"></a><span data-ttu-id="ff799-119">valores de printTaskProcessingState</span><span class="sxs-lookup"><span data-stu-id="ff799-119">printTaskProcessingState values</span></span>

|<span data-ttu-id="ff799-120">Membro</span><span class="sxs-lookup"><span data-stu-id="ff799-120">Member</span></span>|<span data-ttu-id="ff799-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ff799-121">Value</span></span>|<span data-ttu-id="ff799-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff799-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff799-123">função</span><span class="sxs-lookup"><span data-stu-id="ff799-123">pending</span></span>|<span data-ttu-id="ff799-124">,0</span><span class="sxs-lookup"><span data-stu-id="ff799-124">0</span></span>|<span data-ttu-id="ff799-125">A execução da tarefa está pendente.</span><span class="sxs-lookup"><span data-stu-id="ff799-125">Task execution is pending.</span></span>|
|<span data-ttu-id="ff799-126">processe</span><span class="sxs-lookup"><span data-stu-id="ff799-126">processing</span></span>|<span data-ttu-id="ff799-127">1 </span><span class="sxs-lookup"><span data-stu-id="ff799-127">1</span></span>|<span data-ttu-id="ff799-128">A execução da tarefa está em andamento.</span><span class="sxs-lookup"><span data-stu-id="ff799-128">Task execution is in progress.</span></span>|
|<span data-ttu-id="ff799-129">Completed</span><span class="sxs-lookup"><span data-stu-id="ff799-129">completed</span></span>|<span data-ttu-id="ff799-130">2 </span><span class="sxs-lookup"><span data-stu-id="ff799-130">2</span></span>|<span data-ttu-id="ff799-131">A execução da tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="ff799-131">Task execution has completed.</span></span>|
|<span data-ttu-id="ff799-132">anulada</span><span class="sxs-lookup"><span data-stu-id="ff799-132">aborted</span></span>|<span data-ttu-id="ff799-133">3 </span><span class="sxs-lookup"><span data-stu-id="ff799-133">3</span></span>|<span data-ttu-id="ff799-134">A execução da tarefa foi anulada.</span><span class="sxs-lookup"><span data-stu-id="ff799-134">Task execution was aborted.</span></span>|
|<span data-ttu-id="ff799-135">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="ff799-135">unknownFutureValue</span></span>|<span data-ttu-id="ff799-136">4 </span><span class="sxs-lookup"><span data-stu-id="ff799-136">4</span></span>|<span data-ttu-id="ff799-137">Valor de sentinela de enumeração evolvable.</span><span class="sxs-lookup"><span data-stu-id="ff799-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="ff799-138">Não usar.</span><span class="sxs-lookup"><span data-stu-id="ff799-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff799-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff799-139">JSON representation</span></span>

<span data-ttu-id="ff799-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff799-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskStatus"
}-->

```json
{
  "state": {"@odata.type": "microsoft.graph.printTaskProcessingState"},
  "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
