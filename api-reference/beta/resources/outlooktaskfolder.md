---
title: tipo de recurso outlookTaskFolder
description: 'Uma pasta que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f950028bef8bcdcdcd8252ca16348c235ef31d3f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849783"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="05784-103">tipo de recurso outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="05784-103">outlookTaskFolder resource type</span></span>

<span data-ttu-id="05784-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05784-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="05784-105">Uma pasta que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="05784-105">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="05784-106">No Outlook, o grupo de tarefas padrão, `My Tasks` contém uma pasta de tarefas padrão, `Tasks` , para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="05784-106">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="05784-107">Não é possível renomear ou excluir essas pastas e o grupo de tarefas padrão, mas você pode criar grupos de tarefas e pastas de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="05784-107">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="05784-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="05784-108">Methods</span></span>

| <span data-ttu-id="05784-109">Método</span><span class="sxs-lookup"><span data-stu-id="05784-109">Method</span></span>           | <span data-ttu-id="05784-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="05784-110">Return Type</span></span>    |<span data-ttu-id="05784-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="05784-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="05784-112">Obter outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="05784-112">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="05784-113">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="05784-113">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="05784-114">Obtenha as propriedades e os relacionamentos da pasta de tarefas especificada do Outlook.</span><span class="sxs-lookup"><span data-stu-id="05784-114">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="05784-115">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="05784-115">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="05784-116">outlookTask</span><span class="sxs-lookup"><span data-stu-id="05784-116">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="05784-117">Criar uma tarefa do Outlook na pasta de tarefas especificada.</span><span class="sxs-lookup"><span data-stu-id="05784-117">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="05784-118">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="05784-118">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="05784-119">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="05784-119">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="05784-120">Obter todas as tarefas do Outlook na pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="05784-120">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="05784-121">Update</span><span class="sxs-lookup"><span data-stu-id="05784-121">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="05784-122">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="05784-122">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="05784-123">Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="05784-123">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="05784-124">Delete</span><span class="sxs-lookup"><span data-stu-id="05784-124">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="05784-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="05784-125">None</span></span> |<span data-ttu-id="05784-126">Excluir a pasta de tarefas do Outlook especificada.</span><span class="sxs-lookup"><span data-stu-id="05784-126">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="05784-127">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="05784-127">**Extended properties**</span></span>| | |
|[<span data-ttu-id="05784-128">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="05784-128">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="05784-129">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="05784-129">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="05784-130">Crie uma ou mais propriedades estendidas de valor único em uma pasta de tarefas Nova ou existente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="05784-130">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="05784-131">Obter pasta de tarefas com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="05784-131">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="05784-132">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="05784-132">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="05784-133">Obter pastas de tarefas do Outlook que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter` .</span><span class="sxs-lookup"><span data-stu-id="05784-133">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="05784-134">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="05784-134">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="05784-135">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="05784-135">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="05784-136">Criar uma ou mais propriedades estendidas de vários valores em uma pasta de tarefas Nova ou existente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="05784-136">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="05784-137">Obter pasta de tarefas com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="05784-137">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="05784-138">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="05784-138">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="05784-139">Obtenha uma pasta de tarefas do Outlook que contenha uma propriedade estendida de vários valores usando `$expand` .</span><span class="sxs-lookup"><span data-stu-id="05784-139">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="05784-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05784-140">Properties</span></span>
| <span data-ttu-id="05784-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05784-141">Property</span></span>     | <span data-ttu-id="05784-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="05784-142">Type</span></span>   |<span data-ttu-id="05784-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="05784-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05784-144">changeKey</span><span class="sxs-lookup"><span data-stu-id="05784-144">changeKey</span></span>|<span data-ttu-id="05784-145">String</span><span class="sxs-lookup"><span data-stu-id="05784-145">String</span></span>|<span data-ttu-id="05784-146">A versão da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="05784-146">The version of the task folder.</span></span>|
|<span data-ttu-id="05784-147">id</span><span class="sxs-lookup"><span data-stu-id="05784-147">id</span></span>|<span data-ttu-id="05784-148">String</span><span class="sxs-lookup"><span data-stu-id="05784-148">String</span></span>|<span data-ttu-id="05784-149">O identificador da pasta de tarefas, exclusivo na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="05784-149">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="05784-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05784-150">Read-only.</span></span>|
|<span data-ttu-id="05784-151">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="05784-151">isDefaultFolder</span></span>|<span data-ttu-id="05784-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="05784-152">Boolean</span></span>|<span data-ttu-id="05784-153">True se a pasta é a pasta de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="05784-153">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="05784-154">nome</span><span class="sxs-lookup"><span data-stu-id="05784-154">name</span></span>|<span data-ttu-id="05784-155">String</span><span class="sxs-lookup"><span data-stu-id="05784-155">String</span></span>|<span data-ttu-id="05784-156">O nome da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="05784-156">The name of the task folder.</span></span>|
|<span data-ttu-id="05784-157">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="05784-157">parentGroupKey</span></span>|<span data-ttu-id="05784-158">Guid</span><span class="sxs-lookup"><span data-stu-id="05784-158">Guid</span></span>|<span data-ttu-id="05784-159">O identificador exclusivo do GUID para o grupo pai da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="05784-159">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05784-160">Relações</span><span class="sxs-lookup"><span data-stu-id="05784-160">Relationships</span></span>
| <span data-ttu-id="05784-161">Relação</span><span class="sxs-lookup"><span data-stu-id="05784-161">Relationship</span></span> | <span data-ttu-id="05784-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="05784-162">Type</span></span>   |<span data-ttu-id="05784-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="05784-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05784-164">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="05784-164">multiValueExtendedProperties</span></span>|<span data-ttu-id="05784-165">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="05784-165">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="05784-166">A coleção de propriedades estendidas de vários valores definida para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="05784-166">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="05784-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05784-167">Read-only.</span></span> <span data-ttu-id="05784-168">Anulável.</span><span class="sxs-lookup"><span data-stu-id="05784-168">Nullable.</span></span>|
|<span data-ttu-id="05784-169">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="05784-169">singleValueExtendedProperties</span></span>|<span data-ttu-id="05784-170">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="05784-170">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="05784-171">A coleção de propriedades estendidas de valor único definidas para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="05784-171">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="05784-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05784-172">Read-only.</span></span> <span data-ttu-id="05784-173">Anulável.</span><span class="sxs-lookup"><span data-stu-id="05784-173">Nullable.</span></span>|
|<span data-ttu-id="05784-174">tarefas</span><span class="sxs-lookup"><span data-stu-id="05784-174">tasks</span></span>|<span data-ttu-id="05784-175">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="05784-175">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="05784-176">As tarefas nesta pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="05784-176">The tasks in this task folder.</span></span> <span data-ttu-id="05784-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05784-177">Read-only.</span></span> <span data-ttu-id="05784-178">Anulável.</span><span class="sxs-lookup"><span data-stu-id="05784-178">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05784-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05784-179">JSON representation</span></span>
<span data-ttu-id="05784-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05784-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
