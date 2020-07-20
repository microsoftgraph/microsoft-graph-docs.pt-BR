---
title: tipo de recurso de multitarefa
description: Representa uma tarefa que está em execução ou foi executada como resultado de um evento de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 9700f81d2f3a1e488bf9c9c61da3d0f649f46194
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091562"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="f875d-103">tipo de recurso de multitarefa</span><span class="sxs-lookup"><span data-stu-id="f875d-103">printTask resource type</span></span>

<span data-ttu-id="f875d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f875d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f875d-105">Representa uma tarefa que está em execução ou foi executada como resultado de um evento de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="f875d-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="f875d-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="f875d-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="f875d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f875d-107">Methods</span></span>

| <span data-ttu-id="f875d-108">Método</span><span class="sxs-lookup"><span data-stu-id="f875d-108">Method</span></span>       | <span data-ttu-id="f875d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f875d-109">Return Type</span></span> | <span data-ttu-id="f875d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f875d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f875d-111">Lista (de printTaskDefintion)</span><span class="sxs-lookup"><span data-stu-id="f875d-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="f875d-112">multitarefa</span><span class="sxs-lookup"><span data-stu-id="f875d-112">printTask</span></span>](printtask.md) | <span data-ttu-id="f875d-113">Obter uma lista de tarefas que foram criadas com base em um determinado printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="f875d-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="f875d-114">A lista inclui tarefas em execução no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="f875d-114">The list includes currently running tasks and recently completed tasks.</span></span> |

## <a name="properties"></a><span data-ttu-id="f875d-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f875d-115">Properties</span></span>
| <span data-ttu-id="f875d-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f875d-116">Property</span></span>     | <span data-ttu-id="f875d-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="f875d-117">Type</span></span>        | <span data-ttu-id="f875d-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f875d-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f875d-119">id</span><span class="sxs-lookup"><span data-stu-id="f875d-119">id</span></span>|<span data-ttu-id="f875d-120">String</span><span class="sxs-lookup"><span data-stu-id="f875d-120">String</span></span>|<span data-ttu-id="f875d-121">O identificador da tarefa.</span><span class="sxs-lookup"><span data-stu-id="f875d-121">The printTask's identifier.</span></span> <span data-ttu-id="f875d-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f875d-122">Read-only.</span></span>|
|<span data-ttu-id="f875d-123">status</span><span class="sxs-lookup"><span data-stu-id="f875d-123">status</span></span>|[<span data-ttu-id="f875d-124">printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="f875d-124">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="f875d-125">O status de execução atual desta multitarefa.</span><span class="sxs-lookup"><span data-stu-id="f875d-125">The current execution status of this printTask.</span></span> <span data-ttu-id="f875d-126">**O aplicativo de chamada é responsável por atualizar esse status quando o processamento for concluído, a menos que o printJob relacionado tenha sido Redirecionado para outra impressora.**</span><span class="sxs-lookup"><span data-stu-id="f875d-126">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="f875d-127">A falha na conclusão do relatório fará com que o trabalho de impressão relacionado seja bloqueado da impressão e, eventualmente, excluído.</span><span class="sxs-lookup"><span data-stu-id="f875d-127">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="f875d-128">parentUrl</span><span class="sxs-lookup"><span data-stu-id="f875d-128">parentUrl</span></span>|<span data-ttu-id="f875d-129">String</span><span class="sxs-lookup"><span data-stu-id="f875d-129">String</span></span>|<span data-ttu-id="f875d-130">A URL da entidade de impressão que disparou essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="f875d-130">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="f875d-131">Por exemplo, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span><span class="sxs-lookup"><span data-stu-id="f875d-131">For example, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="f875d-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f875d-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f875d-133">Relações</span><span class="sxs-lookup"><span data-stu-id="f875d-133">Relationships</span></span>
| <span data-ttu-id="f875d-134">Relação</span><span class="sxs-lookup"><span data-stu-id="f875d-134">Relationship</span></span> | <span data-ttu-id="f875d-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="f875d-135">Type</span></span>        | <span data-ttu-id="f875d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="f875d-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f875d-137">dispara</span><span class="sxs-lookup"><span data-stu-id="f875d-137">trigger</span></span>|[<span data-ttu-id="f875d-138">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="f875d-138">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="f875d-139">O printTaskTrigger que disparou a execução da tarefa.</span><span class="sxs-lookup"><span data-stu-id="f875d-139">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="f875d-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f875d-140">Read-only.</span></span>|
|<span data-ttu-id="f875d-141">definir</span><span class="sxs-lookup"><span data-stu-id="f875d-141">definition</span></span>|[<span data-ttu-id="f875d-142">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="f875d-142">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="f875d-143">O printTaskDefinition que foi usado para criar essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="f875d-143">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="f875d-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f875d-144">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f875d-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f875d-145">JSON representation</span></span>

<span data-ttu-id="f875d-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f875d-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTask",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.printTaskStatus"},
  "parentUrl": "String",
  "trigger": {"@odata.type": "microsoft.graph.printTaskTrigger"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
