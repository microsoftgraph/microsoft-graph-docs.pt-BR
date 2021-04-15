---
title: Tipo de recurso printTask
description: Representa uma tarefa que está executando ou foi executada como resultado de um evento Impressão Universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c684ff64aa4c3667214b61b70a422690381525b3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766298"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="0e3bd-103">Tipo de recurso printTask</span><span class="sxs-lookup"><span data-stu-id="0e3bd-103">printTask resource type</span></span>

<span data-ttu-id="0e3bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e3bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e3bd-105">Representa uma tarefa que está executando ou foi executada como resultado de um evento Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="0e3bd-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="0e3bd-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="0e3bd-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0e3bd-107">Methods</span></span>

| <span data-ttu-id="0e3bd-108">Método</span><span class="sxs-lookup"><span data-stu-id="0e3bd-108">Method</span></span>       | <span data-ttu-id="0e3bd-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0e3bd-109">Return Type</span></span> | <span data-ttu-id="0e3bd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e3bd-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0e3bd-111">Lista (de printTaskDefintion)</span><span class="sxs-lookup"><span data-stu-id="0e3bd-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="0e3bd-112">printTask</span><span class="sxs-lookup"><span data-stu-id="0e3bd-112">printTask</span></span>](printtask.md) | <span data-ttu-id="0e3bd-113">Obter uma lista de tarefas que foram criadas com base em uma determinada printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="0e3bd-114">A lista inclui tarefas executadas no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-114">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="0e3bd-115">Get</span><span class="sxs-lookup"><span data-stu-id="0e3bd-115">Get</span></span>](../api/printtask-get.md) | [<span data-ttu-id="0e3bd-116">printTask</span><span class="sxs-lookup"><span data-stu-id="0e3bd-116">printTask</span></span>](printtask.md) | <span data-ttu-id="0e3bd-117">Obter detalhes sobre uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-117">Get details about a print task.</span></span> |
| [<span data-ttu-id="0e3bd-118">Atualizar</span><span class="sxs-lookup"><span data-stu-id="0e3bd-118">Update</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="0e3bd-119">printTask</span><span class="sxs-lookup"><span data-stu-id="0e3bd-119">printTask</span></span>](printtask.md) | <span data-ttu-id="0e3bd-120">Atualiza uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-120">Updates a print task.</span></span> |

## <a name="properties"></a><span data-ttu-id="0e3bd-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e3bd-121">Properties</span></span>
| <span data-ttu-id="0e3bd-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e3bd-122">Property</span></span>     | <span data-ttu-id="0e3bd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e3bd-123">Type</span></span>        | <span data-ttu-id="0e3bd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e3bd-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e3bd-125">id</span><span class="sxs-lookup"><span data-stu-id="0e3bd-125">id</span></span>|<span data-ttu-id="0e3bd-126">String</span><span class="sxs-lookup"><span data-stu-id="0e3bd-126">String</span></span>|<span data-ttu-id="0e3bd-127">O identificador printTask.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-127">The printTask's identifier.</span></span> <span data-ttu-id="0e3bd-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-128">Read-only.</span></span>|
|<span data-ttu-id="0e3bd-129">status</span><span class="sxs-lookup"><span data-stu-id="0e3bd-129">status</span></span>|[<span data-ttu-id="0e3bd-130">printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="0e3bd-130">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="0e3bd-131">O status de execução atual deste printTask.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-131">The current execution status of this printTask.</span></span> <span data-ttu-id="0e3bd-132">**O aplicativo de chamada é responsável por atualizar esse status ao terminar o processamento, a menos que a impressão relacionadaJob tenha sido redirecionada para outra impressora.**</span><span class="sxs-lookup"><span data-stu-id="0e3bd-132">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="0e3bd-133">A falha na conclusão do relatório resultará no bloqueio do trabalho de impressão relacionado à impressão e, eventualmente, excluído.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-133">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="0e3bd-134">parentUrl</span><span class="sxs-lookup"><span data-stu-id="0e3bd-134">parentUrl</span></span>|<span data-ttu-id="0e3bd-135">String</span><span class="sxs-lookup"><span data-stu-id="0e3bd-135">String</span></span>|<span data-ttu-id="0e3bd-136">A URL da entidade de impressão que disparou essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-136">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="0e3bd-137">Por exemplo, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-137">For example, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="0e3bd-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e3bd-139">Relações</span><span class="sxs-lookup"><span data-stu-id="0e3bd-139">Relationships</span></span>
| <span data-ttu-id="0e3bd-140">Relação</span><span class="sxs-lookup"><span data-stu-id="0e3bd-140">Relationship</span></span> | <span data-ttu-id="0e3bd-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e3bd-141">Type</span></span>        | <span data-ttu-id="0e3bd-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e3bd-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e3bd-143">trigger</span><span class="sxs-lookup"><span data-stu-id="0e3bd-143">trigger</span></span>|[<span data-ttu-id="0e3bd-144">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="0e3bd-144">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="0e3bd-145">O printTaskTrigger que disparou a execução dessa tarefa.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-145">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="0e3bd-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-146">Read-only.</span></span>|
|<span data-ttu-id="0e3bd-147">definition</span><span class="sxs-lookup"><span data-stu-id="0e3bd-147">definition</span></span>|[<span data-ttu-id="0e3bd-148">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="0e3bd-148">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="0e3bd-149">A printTaskDefinition usada para criar essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-149">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="0e3bd-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-150">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e3bd-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e3bd-151">JSON representation</span></span>

<span data-ttu-id="0e3bd-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e3bd-152">The following is a JSON representation of the resource.</span></span>

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


