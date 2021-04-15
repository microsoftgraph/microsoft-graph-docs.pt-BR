---
title: Tipo de recurso printTaskDefinition
description: Representa uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2495825ec64d73bb440d16e4eae9125f8dbd38eb
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766305"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="bdbad-103">Tipo de recurso printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="bdbad-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="bdbad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdbad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdbad-105">Representa uma definição abstrata para uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="bdbad-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="bdbad-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="bdbad-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

<span data-ttu-id="bdbad-107">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="bdbad-107">This resource supports:</span></span>
* <span data-ttu-id="bdbad-108">[Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).</span><span class="sxs-lookup"><span data-stu-id="bdbad-108">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="bdbad-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="bdbad-109">Methods</span></span>

| <span data-ttu-id="bdbad-110">Método</span><span class="sxs-lookup"><span data-stu-id="bdbad-110">Method</span></span>       | <span data-ttu-id="bdbad-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bdbad-111">Return Type</span></span> | <span data-ttu-id="bdbad-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdbad-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bdbad-113">List</span><span class="sxs-lookup"><span data-stu-id="bdbad-113">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="bdbad-114">[Coleção printTaskDefinition](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bdbad-114">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="bdbad-115">Obter uma lista completa de printTaskDefinitions criados em Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="bdbad-115">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="bdbad-116">Create</span><span class="sxs-lookup"><span data-stu-id="bdbad-116">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="bdbad-117">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="bdbad-117">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="bdbad-118">Crie uma nova printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="bdbad-118">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="bdbad-119">Atualizar</span><span class="sxs-lookup"><span data-stu-id="bdbad-119">Update</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="bdbad-120">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="bdbad-120">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="bdbad-121">Atualize um printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="bdbad-121">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="bdbad-122">Delete</span><span class="sxs-lookup"><span data-stu-id="bdbad-122">Delete</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="bdbad-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdbad-123">None</span></span> | <span data-ttu-id="bdbad-124">Exclua um printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="bdbad-124">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="bdbad-125">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="bdbad-125">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="bdbad-126">printTask</span><span class="sxs-lookup"><span data-stu-id="bdbad-126">printTask</span></span>](printtask.md) | <span data-ttu-id="bdbad-127">Obter uma lista de tarefas que foram criadas com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="bdbad-127">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="bdbad-128">A lista inclui tarefas executadas no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="bdbad-128">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="bdbad-129">Obter tarefa</span><span class="sxs-lookup"><span data-stu-id="bdbad-129">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="bdbad-130">printTask</span><span class="sxs-lookup"><span data-stu-id="bdbad-130">printTask</span></span>](printtask.md) | <span data-ttu-id="bdbad-131">Obtém uma tarefa que foi criada com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="bdbad-131">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="bdbad-132">Atualizar tarefa</span><span class="sxs-lookup"><span data-stu-id="bdbad-132">Update task</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="bdbad-133">printTask</span><span class="sxs-lookup"><span data-stu-id="bdbad-133">printTask</span></span>](printtask.md) | <span data-ttu-id="bdbad-134">Atualize uma tarefa criada com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="bdbad-134">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="bdbad-135">**Os aplicativos que registram gatilhos de tarefas são responsáveis por atualizar o status da tarefa ao terminar o processamento, a menos que a impressão relacionadaJob tenha sido redirecionada para outra impressora.**</span><span class="sxs-lookup"><span data-stu-id="bdbad-135">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="bdbad-136">A falha na conclusão do relatório resultará no bloqueio do trabalho de impressão relacionado à impressão e, eventualmente, excluído.</span><span class="sxs-lookup"><span data-stu-id="bdbad-136">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="bdbad-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdbad-137">Properties</span></span>
| <span data-ttu-id="bdbad-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdbad-138">Property</span></span>     | <span data-ttu-id="bdbad-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdbad-139">Type</span></span>        | <span data-ttu-id="bdbad-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdbad-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bdbad-141">id</span><span class="sxs-lookup"><span data-stu-id="bdbad-141">id</span></span>|<span data-ttu-id="bdbad-142">String</span><span class="sxs-lookup"><span data-stu-id="bdbad-142">String</span></span>|<span data-ttu-id="bdbad-143">O identificador printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="bdbad-143">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="bdbad-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdbad-144">Read-only.</span></span>|
|<span data-ttu-id="bdbad-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bdbad-145">displayName</span></span>|<span data-ttu-id="bdbad-146">String</span><span class="sxs-lookup"><span data-stu-id="bdbad-146">String</span></span>|<span data-ttu-id="bdbad-147">O nome da printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="bdbad-147">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="bdbad-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="bdbad-148">createdBy</span></span>|[<span data-ttu-id="bdbad-149">appIdentity</span><span class="sxs-lookup"><span data-stu-id="bdbad-149">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="bdbad-150">O aplicativo que criou o printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="bdbad-150">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="bdbad-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdbad-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdbad-152">Relações</span><span class="sxs-lookup"><span data-stu-id="bdbad-152">Relationships</span></span>
| <span data-ttu-id="bdbad-153">Relação</span><span class="sxs-lookup"><span data-stu-id="bdbad-153">Relationship</span></span> | <span data-ttu-id="bdbad-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdbad-154">Type</span></span>        | <span data-ttu-id="bdbad-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdbad-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bdbad-156">tarefas</span><span class="sxs-lookup"><span data-stu-id="bdbad-156">tasks</span></span>|<span data-ttu-id="bdbad-157">[Coleção printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="bdbad-157">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="bdbad-158">Uma lista de tarefas que foram criadas com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="bdbad-158">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="bdbad-159">A lista inclui tarefas executadas no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="bdbad-159">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="bdbad-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdbad-160">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdbad-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdbad-161">JSON representation</span></span>

<span data-ttu-id="bdbad-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdbad-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {"@odata.type": "microsoft.graph.appIdentity"},
  "tasks": [{"@odata.type": "microsoft.graph.printTask"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

