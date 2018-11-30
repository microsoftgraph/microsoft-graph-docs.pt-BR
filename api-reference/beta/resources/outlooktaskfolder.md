---
title: tipo de recurso de outlookTaskFolder
description: 'Uma pasta que contém tarefas do Outlook (coleção de objetos outlookTask). '
ms.openlocfilehash: e3fb9d73dbd9458048749331d14f933d838d4243
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038651"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="b3c02-103">tipo de recurso de outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b3c02-103">outlookTaskFolder resource type</span></span>

> <span data-ttu-id="b3c02-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b3c02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3c02-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b3c02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3c02-106">Uma pasta que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="b3c02-106">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="b3c02-107">No Outlook, o grupo de tarefas padrão, `My Tasks`, contém uma pasta de tarefas padrão, `Tasks`, para caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="b3c02-107">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="b3c02-108">Não é possível renomear ou excluir esses grupo de tarefa padrão e uma pasta, mas você pode criar grupos de tarefas adicionais e pastas de tarefa.</span><span class="sxs-lookup"><span data-stu-id="b3c02-108">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="b3c02-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3c02-109">Methods</span></span>

| <span data-ttu-id="b3c02-110">Método</span><span class="sxs-lookup"><span data-stu-id="b3c02-110">Method</span></span>           | <span data-ttu-id="b3c02-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3c02-111">Return Type</span></span>    |<span data-ttu-id="b3c02-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3c02-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b3c02-113">Obter outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b3c02-113">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="b3c02-114">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b3c02-114">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="b3c02-115">Obtenha as propriedades e relacionamentos da pasta de tarefas do Outlook especificado.</span><span class="sxs-lookup"><span data-stu-id="b3c02-115">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="b3c02-116">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="b3c02-116">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="b3c02-117">outlookTask</span><span class="sxs-lookup"><span data-stu-id="b3c02-117">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="b3c02-118">Crie uma tarefa do Outlook na pasta tarefa especificada.</span><span class="sxs-lookup"><span data-stu-id="b3c02-118">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="b3c02-119">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="b3c02-119">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="b3c02-120">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="b3c02-120">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="b3c02-121">Obtenha todas as tarefas do Outlook na pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="b3c02-121">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="b3c02-122">Update</span><span class="sxs-lookup"><span data-stu-id="b3c02-122">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="b3c02-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b3c02-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="b3c02-124">Atualize as propriedades graváveis de uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="b3c02-124">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="b3c02-125">Delete</span><span class="sxs-lookup"><span data-stu-id="b3c02-125">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="b3c02-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3c02-126">None</span></span> |<span data-ttu-id="b3c02-127">Exclua a pasta de tarefas do Outlook especificada.</span><span class="sxs-lookup"><span data-stu-id="b3c02-127">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="b3c02-128">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="b3c02-128">**Extended properties**</span></span>| | |
|[<span data-ttu-id="b3c02-129">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="b3c02-129">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="b3c02-130">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b3c02-130">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="b3c02-131">Crie um ou mais propriedades estendidas de valor único em uma pasta de tarefas do Outlook nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="b3c02-131">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="b3c02-132">Obter a pasta de tarefas com a propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="b3c02-132">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b3c02-133">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b3c02-133">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="b3c02-134">Obtenha as pastas de tarefas do Outlook que contêm um valor único propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b3c02-134">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b3c02-135">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="b3c02-135">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="b3c02-136">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b3c02-136">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="b3c02-137">Crie um ou mais propriedades estendidas de valores múltiplos em uma pasta de tarefas do Outlook nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="b3c02-137">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="b3c02-138">Obter a pasta de tarefas com vários valores de propriedade estendida</span><span class="sxs-lookup"><span data-stu-id="b3c02-138">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b3c02-139">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b3c02-139">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="b3c02-140">Obtenha uma pasta de tarefas do Outlook que contenha uma propriedade de valor múltiplos estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="b3c02-140">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="b3c02-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3c02-141">Properties</span></span>
| <span data-ttu-id="b3c02-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3c02-142">Property</span></span>     | <span data-ttu-id="b3c02-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3c02-143">Type</span></span>   |<span data-ttu-id="b3c02-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3c02-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3c02-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="b3c02-145">changeKey</span></span>|<span data-ttu-id="b3c02-146">String</span><span class="sxs-lookup"><span data-stu-id="b3c02-146">String</span></span>|<span data-ttu-id="b3c02-147">A versão da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="b3c02-147">The version of the task folder.</span></span>|
|<span data-ttu-id="b3c02-148">id</span><span class="sxs-lookup"><span data-stu-id="b3c02-148">id</span></span>|<span data-ttu-id="b3c02-149">String</span><span class="sxs-lookup"><span data-stu-id="b3c02-149">String</span></span>|<span data-ttu-id="b3c02-150">O identificador da pasta de tarefas, exclusivo na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="b3c02-150">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="b3c02-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c02-151">Read-only.</span></span>|
|<span data-ttu-id="b3c02-152">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="b3c02-152">isDefaultFolder</span></span>|<span data-ttu-id="b3c02-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3c02-153">Boolean</span></span>|<span data-ttu-id="b3c02-154">True se a pasta está na pasta de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="b3c02-154">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="b3c02-155">name</span><span class="sxs-lookup"><span data-stu-id="b3c02-155">name</span></span>|<span data-ttu-id="b3c02-156">String</span><span class="sxs-lookup"><span data-stu-id="b3c02-156">String</span></span>|<span data-ttu-id="b3c02-157">O nome da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="b3c02-157">The name of the task folder.</span></span>|
|<span data-ttu-id="b3c02-158">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="b3c02-158">parentGroupKey</span></span>|<span data-ttu-id="b3c02-159">Guid</span><span class="sxs-lookup"><span data-stu-id="b3c02-159">Guid</span></span>|<span data-ttu-id="b3c02-160">O identificador GUID exclusivo para o grupo do pai da pasta tarefa.</span><span class="sxs-lookup"><span data-stu-id="b3c02-160">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3c02-161">Relações</span><span class="sxs-lookup"><span data-stu-id="b3c02-161">Relationships</span></span>
| <span data-ttu-id="b3c02-162">Relação</span><span class="sxs-lookup"><span data-stu-id="b3c02-162">Relationship</span></span> | <span data-ttu-id="b3c02-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3c02-163">Type</span></span>   |<span data-ttu-id="b3c02-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3c02-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3c02-165">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b3c02-165">multiValueExtendedProperties</span></span>|<span data-ttu-id="b3c02-166">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b3c02-166">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="b3c02-167">A coleção de propriedades estendidas de múltiplos valores definidos para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="b3c02-167">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="b3c02-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c02-168">Read-only.</span></span> <span data-ttu-id="b3c02-169">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b3c02-169">Nullable.</span></span>|
|<span data-ttu-id="b3c02-170">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b3c02-170">singleValueExtendedProperties</span></span>|<span data-ttu-id="b3c02-171">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b3c02-171">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="b3c02-172">A coleção de propriedades estendidas de valor único definidos para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="b3c02-172">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="b3c02-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c02-173">Read-only.</span></span> <span data-ttu-id="b3c02-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b3c02-174">Nullable.</span></span>|
|<span data-ttu-id="b3c02-175">tarefas</span><span class="sxs-lookup"><span data-stu-id="b3c02-175">tasks</span></span>|<span data-ttu-id="b3c02-176">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="b3c02-176">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="b3c02-177">As tarefas nesta pasta tarefa.</span><span class="sxs-lookup"><span data-stu-id="b3c02-177">The tasks in this task folder.</span></span> <span data-ttu-id="b3c02-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c02-178">Read-only.</span></span> <span data-ttu-id="b3c02-179">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b3c02-179">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3c02-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3c02-180">JSON representation</span></span>
<span data-ttu-id="b3c02-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3c02-181">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->