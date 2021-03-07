---
title: Tipo de recurso printTask
description: Representa uma tarefa que está executando ou foi executada como resultado de um evento Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2026706ec46a2408d20231add8203d2f5a622c96
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516860"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="6f017-103">Tipo de recurso printTask</span><span class="sxs-lookup"><span data-stu-id="6f017-103">printTask resource type</span></span>

<span data-ttu-id="6f017-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f017-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="6f017-105">Representa uma tarefa que está executando ou foi executada como resultado de um evento Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="6f017-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="6f017-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="6f017-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="6f017-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6f017-107">Methods</span></span>
|<span data-ttu-id="6f017-108">Método</span><span class="sxs-lookup"><span data-stu-id="6f017-108">Method</span></span>|<span data-ttu-id="6f017-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6f017-109">Return type</span></span>|<span data-ttu-id="6f017-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f017-110">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="6f017-111">Lista (de printTaskDefintion)</span><span class="sxs-lookup"><span data-stu-id="6f017-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="6f017-112">printTask</span><span class="sxs-lookup"><span data-stu-id="6f017-112">printTask</span></span>](printtask.md) | <span data-ttu-id="6f017-113">Obter uma lista de tarefas que foram criadas com base em uma determinada printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="6f017-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="6f017-114">A lista inclui tarefas executadas no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="6f017-114">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="6f017-115">Get</span><span class="sxs-lookup"><span data-stu-id="6f017-115">Get</span></span>](../api/printtask-get.md) | [<span data-ttu-id="6f017-116">printTask</span><span class="sxs-lookup"><span data-stu-id="6f017-116">printTask</span></span>](printtask.md) | <span data-ttu-id="6f017-117">Obter detalhes sobre uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="6f017-117">Get details about a print task.</span></span> |
| [<span data-ttu-id="6f017-118">Update</span><span class="sxs-lookup"><span data-stu-id="6f017-118">Update</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="6f017-119">printTask</span><span class="sxs-lookup"><span data-stu-id="6f017-119">printTask</span></span>](printtask.md) | <span data-ttu-id="6f017-120">Atualiza uma tarefa de impressão.</span><span class="sxs-lookup"><span data-stu-id="6f017-120">Updates a print task.</span></span> |

## <a name="properties"></a><span data-ttu-id="6f017-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f017-121">Properties</span></span>
|<span data-ttu-id="6f017-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f017-122">Property</span></span>|<span data-ttu-id="6f017-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f017-123">Type</span></span>|<span data-ttu-id="6f017-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f017-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f017-125">id</span><span class="sxs-lookup"><span data-stu-id="6f017-125">id</span></span>|<span data-ttu-id="6f017-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f017-126">String</span></span>|<span data-ttu-id="6f017-127">O identificador printTask.</span><span class="sxs-lookup"><span data-stu-id="6f017-127">The printTask's identifier.</span></span> <span data-ttu-id="6f017-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f017-128">Read-only.</span></span>|
|<span data-ttu-id="6f017-129">status</span><span class="sxs-lookup"><span data-stu-id="6f017-129">status</span></span>|[<span data-ttu-id="6f017-130">printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="6f017-130">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="6f017-131">O status de execução atual deste printTask.</span><span class="sxs-lookup"><span data-stu-id="6f017-131">The current execution status of this printTask.</span></span> <span data-ttu-id="6f017-132">**O aplicativo de chamada é responsável por atualizar esse status ao terminar o processamento, a menos que a impressão relacionadaJob tenha sido redirecionada para outra impressora.**</span><span class="sxs-lookup"><span data-stu-id="6f017-132">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="6f017-133">A falha na conclusão do relatório resultará no bloqueio do trabalho de impressão relacionado à impressão e, eventualmente, excluído.</span><span class="sxs-lookup"><span data-stu-id="6f017-133">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="6f017-134">parentUrl</span><span class="sxs-lookup"><span data-stu-id="6f017-134">parentUrl</span></span>|<span data-ttu-id="6f017-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f017-135">String</span></span>|<span data-ttu-id="6f017-136">A URL da entidade de impressão que disparou essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="6f017-136">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="6f017-137">Por exemplo, `https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{jobId}`.</span><span class="sxs-lookup"><span data-stu-id="6f017-137">For example, `https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="6f017-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f017-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f017-139">Relações</span><span class="sxs-lookup"><span data-stu-id="6f017-139">Relationships</span></span>
|<span data-ttu-id="6f017-140">Relação</span><span class="sxs-lookup"><span data-stu-id="6f017-140">Relationship</span></span>|<span data-ttu-id="6f017-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f017-141">Type</span></span>|<span data-ttu-id="6f017-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f017-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f017-143">trigger</span><span class="sxs-lookup"><span data-stu-id="6f017-143">trigger</span></span>|[<span data-ttu-id="6f017-144">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="6f017-144">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="6f017-145">O printTaskTrigger que disparou a execução dessa tarefa.</span><span class="sxs-lookup"><span data-stu-id="6f017-145">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="6f017-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f017-146">Read-only.</span></span>|
|<span data-ttu-id="6f017-147">definition</span><span class="sxs-lookup"><span data-stu-id="6f017-147">definition</span></span>|[<span data-ttu-id="6f017-148">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="6f017-148">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="6f017-149">A printTaskDefinition usada para criar essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="6f017-149">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="6f017-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f017-150">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f017-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f017-151">JSON representation</span></span>
<span data-ttu-id="6f017-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f017-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTask",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printTaskStatus"
  },
  "parentUrl": "String"
}
```

