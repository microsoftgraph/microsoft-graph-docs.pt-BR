---
title: tipo de recurso printTaskStatus
description: Representa o status de execução atual de uma multitarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5f340acf8357155893020985aa6036d93ed5b2df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078301"
---
# <a name="printtaskstatus-resource-type"></a><span data-ttu-id="e8832-103">tipo de recurso printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="e8832-103">printTaskStatus resource type</span></span>

<span data-ttu-id="e8832-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8832-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8832-105">Representa o status de execução atual de uma [multitarefa](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="e8832-105">Represents the current execution status of a [printTask](printtask.md).</span></span> 

><span data-ttu-id="e8832-106">**Observação:** Os aplicativos que registram gatilhos de tarefa são responsáveis por atualizar os status da tarefa quando o processamento for concluído, a menos que o trabalho de impressão relacionado tenha sido Redirecionado para outra impressora.</span><span class="sxs-lookup"><span data-stu-id="e8832-106">**Note:** Applications that register task triggers are responsible for updating task statuses when processing is finished, unless the related print job has been redirected to another printer.</span></span>

<span data-ttu-id="e8832-107">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="e8832-107">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="properties"></a><span data-ttu-id="e8832-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8832-108">Properties</span></span>
| <span data-ttu-id="e8832-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8832-109">Property</span></span>     | <span data-ttu-id="e8832-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8832-110">Type</span></span>        | <span data-ttu-id="e8832-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8832-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e8832-112">state</span><span class="sxs-lookup"><span data-stu-id="e8832-112">state</span></span>|<span data-ttu-id="e8832-113">printTaskProcessingState</span><span class="sxs-lookup"><span data-stu-id="e8832-113">printTaskProcessingState</span></span>|<span data-ttu-id="e8832-114">O estado de processamento atual da [multitarefa](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="e8832-114">The current processing state of the [printTask](printtask.md).</span></span> <span data-ttu-id="e8832-115">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="e8832-115">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="e8832-116">description</span><span class="sxs-lookup"><span data-stu-id="e8832-116">description</span></span>|<span data-ttu-id="e8832-117">String</span><span class="sxs-lookup"><span data-stu-id="e8832-117">String</span></span>|<span data-ttu-id="e8832-118">Uma descrição legível do estado atual de processamento da [tarefa](printtask.md).</span><span class="sxs-lookup"><span data-stu-id="e8832-118">A human-readable description of the current processing state of the [printTask](printtask.md).</span></span>|

### <a name="printtaskprocessingstate-values"></a><span data-ttu-id="e8832-119">valores de printTaskProcessingState</span><span class="sxs-lookup"><span data-stu-id="e8832-119">printTaskProcessingState values</span></span>

|<span data-ttu-id="e8832-120">Membro</span><span class="sxs-lookup"><span data-stu-id="e8832-120">Member</span></span>|<span data-ttu-id="e8832-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e8832-121">Value</span></span>|<span data-ttu-id="e8832-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8832-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8832-123">função</span><span class="sxs-lookup"><span data-stu-id="e8832-123">pending</span></span>|<span data-ttu-id="e8832-124">,0</span><span class="sxs-lookup"><span data-stu-id="e8832-124">0</span></span>|<span data-ttu-id="e8832-125">A execução da tarefa está pendente.</span><span class="sxs-lookup"><span data-stu-id="e8832-125">Task execution is pending.</span></span>|
|<span data-ttu-id="e8832-126">processe</span><span class="sxs-lookup"><span data-stu-id="e8832-126">processing</span></span>|<span data-ttu-id="e8832-127">1 </span><span class="sxs-lookup"><span data-stu-id="e8832-127">1</span></span>|<span data-ttu-id="e8832-128">A execução da tarefa está em andamento.</span><span class="sxs-lookup"><span data-stu-id="e8832-128">Task execution is in progress.</span></span>|
|<span data-ttu-id="e8832-129">Completed</span><span class="sxs-lookup"><span data-stu-id="e8832-129">completed</span></span>|<span data-ttu-id="e8832-130">2 </span><span class="sxs-lookup"><span data-stu-id="e8832-130">2</span></span>|<span data-ttu-id="e8832-131">A execução da tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="e8832-131">Task execution has completed.</span></span>|
|<span data-ttu-id="e8832-132">anulada</span><span class="sxs-lookup"><span data-stu-id="e8832-132">aborted</span></span>|<span data-ttu-id="e8832-133">3 </span><span class="sxs-lookup"><span data-stu-id="e8832-133">3</span></span>|<span data-ttu-id="e8832-134">A execução da tarefa foi anulada.</span><span class="sxs-lookup"><span data-stu-id="e8832-134">Task execution was aborted.</span></span>|
|<span data-ttu-id="e8832-135">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="e8832-135">unknownFutureValue</span></span>|<span data-ttu-id="e8832-136">4 </span><span class="sxs-lookup"><span data-stu-id="e8832-136">4</span></span>|<span data-ttu-id="e8832-137">Valor de sentinela de enumeração evolvable.</span><span class="sxs-lookup"><span data-stu-id="e8832-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="e8832-138">Não usar.</span><span class="sxs-lookup"><span data-stu-id="e8832-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8832-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8832-139">JSON representation</span></span>

<span data-ttu-id="e8832-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8832-140">The following is a JSON representation of the resource.</span></span>

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


