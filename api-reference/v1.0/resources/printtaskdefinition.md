---
title: Tipo de recurso printTaskDefinition
description: Representa uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9a8a8c78d1e165dfe0f9417c5aa052f9f0b2383b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517057"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="cfebb-103">Tipo de recurso printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="cfebb-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="cfebb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfebb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="cfebb-105">Representa uma definição abstrata para uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="cfebb-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="cfebb-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="cfebb-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

<span data-ttu-id="cfebb-107">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="cfebb-107">This resource supports:</span></span>
* <span data-ttu-id="cfebb-108">[Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).</span><span class="sxs-lookup"><span data-stu-id="cfebb-108">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="cfebb-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="cfebb-109">Methods</span></span>
| <span data-ttu-id="cfebb-110">Método</span><span class="sxs-lookup"><span data-stu-id="cfebb-110">Method</span></span>       | <span data-ttu-id="cfebb-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cfebb-111">Return Type</span></span> | <span data-ttu-id="cfebb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfebb-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cfebb-113">List</span><span class="sxs-lookup"><span data-stu-id="cfebb-113">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="cfebb-114">[Coleção printTaskDefinition](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cfebb-114">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="cfebb-115">Obter uma lista completa de printTaskDefinitions criados em Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="cfebb-115">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="cfebb-116">Create</span><span class="sxs-lookup"><span data-stu-id="cfebb-116">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="cfebb-117">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="cfebb-117">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="cfebb-118">Crie uma nova printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="cfebb-118">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="cfebb-119">Update</span><span class="sxs-lookup"><span data-stu-id="cfebb-119">Update</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="cfebb-120">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="cfebb-120">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="cfebb-121">Atualize um printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="cfebb-121">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="cfebb-122">Delete</span><span class="sxs-lookup"><span data-stu-id="cfebb-122">Delete</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="cfebb-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cfebb-123">None</span></span> | <span data-ttu-id="cfebb-124">Exclua um printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="cfebb-124">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="cfebb-125">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="cfebb-125">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="cfebb-126">printTask</span><span class="sxs-lookup"><span data-stu-id="cfebb-126">printTask</span></span>](printtask.md) | <span data-ttu-id="cfebb-127">Obter uma lista de tarefas que foram criadas com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="cfebb-127">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="cfebb-128">A lista inclui tarefas executadas no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="cfebb-128">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="cfebb-129">Obter tarefa</span><span class="sxs-lookup"><span data-stu-id="cfebb-129">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="cfebb-130">printTask</span><span class="sxs-lookup"><span data-stu-id="cfebb-130">printTask</span></span>](printtask.md) | <span data-ttu-id="cfebb-131">Obtém uma tarefa que foi criada com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="cfebb-131">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="cfebb-132">Atualizar tarefa</span><span class="sxs-lookup"><span data-stu-id="cfebb-132">Update task</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="cfebb-133">printTask</span><span class="sxs-lookup"><span data-stu-id="cfebb-133">printTask</span></span>](printtask.md) | <span data-ttu-id="cfebb-134">Atualize uma tarefa criada com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="cfebb-134">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="cfebb-135">**Os aplicativos que registram gatilhos de tarefas são responsáveis por atualizar o status da tarefa ao terminar o processamento, a menos que a impressão relacionadaJob tenha sido redirecionada para outra impressora.**</span><span class="sxs-lookup"><span data-stu-id="cfebb-135">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="cfebb-136">A falha na conclusão do relatório resultará no bloqueio do trabalho de impressão relacionado à impressão e, eventualmente, excluído.</span><span class="sxs-lookup"><span data-stu-id="cfebb-136">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="cfebb-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfebb-137">Properties</span></span>
|<span data-ttu-id="cfebb-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfebb-138">Property</span></span>|<span data-ttu-id="cfebb-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfebb-139">Type</span></span>|<span data-ttu-id="cfebb-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfebb-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfebb-141">id</span><span class="sxs-lookup"><span data-stu-id="cfebb-141">id</span></span>|<span data-ttu-id="cfebb-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfebb-142">String</span></span>|<span data-ttu-id="cfebb-143">O identificador printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="cfebb-143">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="cfebb-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cfebb-144">Read-only.</span></span>|
|<span data-ttu-id="cfebb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="cfebb-145">displayName</span></span>|<span data-ttu-id="cfebb-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfebb-146">String</span></span>|<span data-ttu-id="cfebb-147">O nome da printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="cfebb-147">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="cfebb-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="cfebb-148">createdBy</span></span>|[<span data-ttu-id="cfebb-149">appIdentity</span><span class="sxs-lookup"><span data-stu-id="cfebb-149">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="cfebb-150">O aplicativo que criou o printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="cfebb-150">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="cfebb-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cfebb-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfebb-152">Relações</span><span class="sxs-lookup"><span data-stu-id="cfebb-152">Relationships</span></span>
|<span data-ttu-id="cfebb-153">Relação</span><span class="sxs-lookup"><span data-stu-id="cfebb-153">Relationship</span></span>|<span data-ttu-id="cfebb-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfebb-154">Type</span></span>|<span data-ttu-id="cfebb-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfebb-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfebb-156">tarefas</span><span class="sxs-lookup"><span data-stu-id="cfebb-156">tasks</span></span>|<span data-ttu-id="cfebb-157">[Coleção printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="cfebb-157">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="cfebb-158">Uma lista de tarefas que foram criadas com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="cfebb-158">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="cfebb-159">A lista inclui tarefas executadas no momento e tarefas concluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="cfebb-159">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="cfebb-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cfebb-160">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfebb-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfebb-161">JSON representation</span></span>
<span data-ttu-id="cfebb-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfebb-162">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.appIdentity"
  }
}
```

