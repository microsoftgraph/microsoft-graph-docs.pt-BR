---
title: Tipo de recurso printTaskDefinition
description: Representa uma tarefa que pode ser disparada quando vários eventos ocorrem na Impressão Universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: bbffceb08be336cd816d80f03236078b39348339
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934853"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="52a0b-103">Tipo de recurso printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="52a0b-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="52a0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52a0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52a0b-105">Representa uma definição abstrata para uma tarefa que pode ser disparada quando vários eventos ocorrem na Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="52a0b-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="52a0b-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte de impressão pull à Impressão Universal, consulte Estendendo a impressão universal para dar suporte [à impressão pull.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="52a0b-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

<span data-ttu-id="52a0b-107">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="52a0b-107">This resource supports:</span></span>
* <span data-ttu-id="52a0b-108">[Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).</span><span class="sxs-lookup"><span data-stu-id="52a0b-108">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="52a0b-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="52a0b-109">Methods</span></span>

| <span data-ttu-id="52a0b-110">Método</span><span class="sxs-lookup"><span data-stu-id="52a0b-110">Method</span></span>       | <span data-ttu-id="52a0b-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52a0b-111">Return Type</span></span> | <span data-ttu-id="52a0b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="52a0b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="52a0b-113">List</span><span class="sxs-lookup"><span data-stu-id="52a0b-113">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="52a0b-114">[Coleção printTaskDefinition](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52a0b-114">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="52a0b-115">Obter uma lista completa de printTaskDefinitions criadas na Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="52a0b-115">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="52a0b-116">Create</span><span class="sxs-lookup"><span data-stu-id="52a0b-116">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="52a0b-117">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="52a0b-117">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="52a0b-118">Crie uma nova printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="52a0b-118">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="52a0b-119">Update</span><span class="sxs-lookup"><span data-stu-id="52a0b-119">Update</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="52a0b-120">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="52a0b-120">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="52a0b-121">Atualize uma printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="52a0b-121">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="52a0b-122">Delete</span><span class="sxs-lookup"><span data-stu-id="52a0b-122">Delete</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="52a0b-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52a0b-123">None</span></span> | <span data-ttu-id="52a0b-124">Exclua uma printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="52a0b-124">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="52a0b-125">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="52a0b-125">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="52a0b-126">printTask</span><span class="sxs-lookup"><span data-stu-id="52a0b-126">printTask</span></span>](printtask.md) | <span data-ttu-id="52a0b-127">Obter uma lista de tarefas que foram criadas com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="52a0b-127">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="52a0b-128">A lista inclui tarefas em execução no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="52a0b-128">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="52a0b-129">Obter tarefa</span><span class="sxs-lookup"><span data-stu-id="52a0b-129">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="52a0b-130">printTask</span><span class="sxs-lookup"><span data-stu-id="52a0b-130">printTask</span></span>](printtask.md) | <span data-ttu-id="52a0b-131">Obtém uma tarefa que foi criada com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="52a0b-131">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="52a0b-132">Atualizar tarefa</span><span class="sxs-lookup"><span data-stu-id="52a0b-132">Update task</span></span>](../api/printtaskdefinition-update-task.md) | <span data-ttu-id="52a0b-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52a0b-133">None</span></span> | <span data-ttu-id="52a0b-134">Atualize uma tarefa que foi criada com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="52a0b-134">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="52a0b-135">**Os aplicativos que registram gatilhos de tarefa são responsáveis por atualizar o status da tarefa quando o processamento é concluído, a menos que o printJob relacionado tenha sido redirecionado para outra impressora.**</span><span class="sxs-lookup"><span data-stu-id="52a0b-135">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="52a0b-136">A falha ao relatar a conclusão fará com que o trabalho de impressão relacionado seja impedido de imprimir e, eventualmente, excluído.</span><span class="sxs-lookup"><span data-stu-id="52a0b-136">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="52a0b-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52a0b-137">Properties</span></span>
| <span data-ttu-id="52a0b-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52a0b-138">Property</span></span>     | <span data-ttu-id="52a0b-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="52a0b-139">Type</span></span>        | <span data-ttu-id="52a0b-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="52a0b-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52a0b-141">id</span><span class="sxs-lookup"><span data-stu-id="52a0b-141">id</span></span>|<span data-ttu-id="52a0b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52a0b-142">String</span></span>|<span data-ttu-id="52a0b-143">O identificador de printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="52a0b-143">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="52a0b-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52a0b-144">Read-only.</span></span>|
|<span data-ttu-id="52a0b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="52a0b-145">displayName</span></span>|<span data-ttu-id="52a0b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52a0b-146">String</span></span>|<span data-ttu-id="52a0b-147">O nome da printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="52a0b-147">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="52a0b-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="52a0b-148">createdBy</span></span>|[<span data-ttu-id="52a0b-149">appIdentity</span><span class="sxs-lookup"><span data-stu-id="52a0b-149">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="52a0b-150">O aplicativo que criou a printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="52a0b-150">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="52a0b-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52a0b-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52a0b-152">Relações</span><span class="sxs-lookup"><span data-stu-id="52a0b-152">Relationships</span></span>
| <span data-ttu-id="52a0b-153">Relação</span><span class="sxs-lookup"><span data-stu-id="52a0b-153">Relationship</span></span> | <span data-ttu-id="52a0b-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="52a0b-154">Type</span></span>        | <span data-ttu-id="52a0b-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="52a0b-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52a0b-156">tarefas</span><span class="sxs-lookup"><span data-stu-id="52a0b-156">tasks</span></span>|<span data-ttu-id="52a0b-157">[Coleção printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="52a0b-157">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="52a0b-158">Uma lista de tarefas que foram criadas com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="52a0b-158">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="52a0b-159">A lista inclui tarefas em execução no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="52a0b-159">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="52a0b-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52a0b-160">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52a0b-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52a0b-161">JSON representation</span></span>

<span data-ttu-id="52a0b-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52a0b-162">The following is a JSON representation of the resource.</span></span>

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

