---
title: tipo de recurso printTaskDefinition
description: Representa uma tarefa que pode ser disparada quando vários eventos ocorrem dentro da impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 013d2756455abebc0f20bbe5a1d186a0a4d65648
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091546"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="5e5b5-103">tipo de recurso printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5e5b5-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="5e5b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e5b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e5b5-105">Representa uma definição abstrata de uma tarefa que pode ser disparada quando vários eventos ocorrem dentro da impressão universal.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="5e5b5-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="5e5b5-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="5e5b5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e5b5-107">Methods</span></span>

| <span data-ttu-id="5e5b5-108">Método</span><span class="sxs-lookup"><span data-stu-id="5e5b5-108">Method</span></span>       | <span data-ttu-id="5e5b5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e5b5-109">Return Type</span></span> | <span data-ttu-id="5e5b5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e5b5-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5e5b5-111">Listar</span><span class="sxs-lookup"><span data-stu-id="5e5b5-111">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="5e5b5-112">coleção [printTaskDefinition](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e5b5-112">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="5e5b5-113">Obtenha uma lista completa de printTaskDefinitions criadas dentro da impressão universal.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-113">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="5e5b5-114">Criar</span><span class="sxs-lookup"><span data-stu-id="5e5b5-114">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="5e5b5-115">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5e5b5-115">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="5e5b5-116">Criar um novo printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-116">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="5e5b5-117">Update</span><span class="sxs-lookup"><span data-stu-id="5e5b5-117">Update</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="5e5b5-118">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5e5b5-118">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="5e5b5-119">Atualizar um printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-119">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="5e5b5-120">Delete</span><span class="sxs-lookup"><span data-stu-id="5e5b5-120">Delete</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="5e5b5-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e5b5-121">None</span></span> | <span data-ttu-id="5e5b5-122">Excluir um printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-122">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="5e5b5-123">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="5e5b5-123">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="5e5b5-124">multitarefa</span><span class="sxs-lookup"><span data-stu-id="5e5b5-124">printTask</span></span>](printtask.md) | <span data-ttu-id="5e5b5-125">Obtém uma lista de tarefas que foram criadas com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-125">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="5e5b5-126">A lista inclui tarefas em execução no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-126">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="5e5b5-127">Obter tarefa</span><span class="sxs-lookup"><span data-stu-id="5e5b5-127">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="5e5b5-128">multitarefa</span><span class="sxs-lookup"><span data-stu-id="5e5b5-128">printTask</span></span>](printtask.md) | <span data-ttu-id="5e5b5-129">Obtém uma tarefa que foi criada com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-129">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="5e5b5-130">Atualizar tarefa</span><span class="sxs-lookup"><span data-stu-id="5e5b5-130">Update task</span></span>](../api/printtaskdefinition-update-task.md) | <span data-ttu-id="5e5b5-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e5b5-131">None</span></span> | <span data-ttu-id="5e5b5-132">Atualizar uma tarefa que foi criada com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-132">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="5e5b5-133">**Os aplicativos que registram gatilhos de tarefa são responsáveis por atualizar o status da tarefa quando o processamento é concluído, a menos que o printJob relacionado tenha sido Redirecionado para outra impressora.**</span><span class="sxs-lookup"><span data-stu-id="5e5b5-133">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="5e5b5-134">A falha na conclusão do relatório fará com que o trabalho de impressão relacionado seja bloqueado da impressão e, eventualmente, excluído.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-134">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="5e5b5-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e5b5-135">Properties</span></span>
| <span data-ttu-id="5e5b5-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e5b5-136">Property</span></span>     | <span data-ttu-id="5e5b5-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e5b5-137">Type</span></span>        | <span data-ttu-id="5e5b5-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e5b5-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e5b5-139">id</span><span class="sxs-lookup"><span data-stu-id="5e5b5-139">id</span></span>|<span data-ttu-id="5e5b5-140">String</span><span class="sxs-lookup"><span data-stu-id="5e5b5-140">String</span></span>|<span data-ttu-id="5e5b5-141">O identificador do printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-141">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="5e5b5-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-142">Read-only.</span></span>|
|<span data-ttu-id="5e5b5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="5e5b5-143">displayName</span></span>|<span data-ttu-id="5e5b5-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e5b5-144">String</span></span>|<span data-ttu-id="5e5b5-145">O nome do printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-145">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="5e5b5-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="5e5b5-146">createdBy</span></span>|[<span data-ttu-id="5e5b5-147">appIdentity</span><span class="sxs-lookup"><span data-stu-id="5e5b5-147">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="5e5b5-148">O aplicativo que criou o printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-148">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="5e5b5-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-149">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e5b5-150">Relações</span><span class="sxs-lookup"><span data-stu-id="5e5b5-150">Relationships</span></span>
| <span data-ttu-id="5e5b5-151">Relação</span><span class="sxs-lookup"><span data-stu-id="5e5b5-151">Relationship</span></span> | <span data-ttu-id="5e5b5-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e5b5-152">Type</span></span>        | <span data-ttu-id="5e5b5-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e5b5-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e5b5-154">tarefas</span><span class="sxs-lookup"><span data-stu-id="5e5b5-154">tasks</span></span>|<span data-ttu-id="5e5b5-155">coleção [multitask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="5e5b5-155">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="5e5b5-156">Uma lista de tarefas que foram criadas com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-156">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="5e5b5-157">A lista inclui tarefas em execução no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-157">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="5e5b5-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-158">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e5b5-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e5b5-159">JSON representation</span></span>

<span data-ttu-id="5e5b5-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-160">The following is a JSON representation of the resource.</span></span>

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