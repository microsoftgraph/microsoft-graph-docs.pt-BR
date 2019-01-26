---
title: tipo de recurso de outlookTaskFolder
description: 'Uma pasta que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a117e14ea1cfe4b69cbbf69720a22a0094fb0b72
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575664"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="ca51d-103">tipo de recurso de outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ca51d-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca51d-104">Uma pasta que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="ca51d-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="ca51d-105">No Outlook, o grupo de tarefas padrão, `My Tasks`, contém uma pasta de tarefas padrão, `Tasks`, para caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ca51d-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="ca51d-106">Não é possível renomear ou excluir esses grupo de tarefa padrão e uma pasta, mas você pode criar grupos de tarefas adicionais e pastas de tarefa.</span><span class="sxs-lookup"><span data-stu-id="ca51d-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="ca51d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ca51d-107">Methods</span></span>

| <span data-ttu-id="ca51d-108">Método</span><span class="sxs-lookup"><span data-stu-id="ca51d-108">Method</span></span>           | <span data-ttu-id="ca51d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ca51d-109">Return Type</span></span>    |<span data-ttu-id="ca51d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca51d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca51d-111">Obter outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ca51d-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="ca51d-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ca51d-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="ca51d-113">Obtenha as propriedades e relacionamentos da pasta de tarefas do Outlook especificado.</span><span class="sxs-lookup"><span data-stu-id="ca51d-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="ca51d-114">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="ca51d-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="ca51d-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="ca51d-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="ca51d-116">Crie uma tarefa do Outlook na pasta tarefa especificada.</span><span class="sxs-lookup"><span data-stu-id="ca51d-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="ca51d-117">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="ca51d-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="ca51d-118">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="ca51d-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="ca51d-119">Obtenha todas as tarefas do Outlook na pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="ca51d-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="ca51d-120">Update</span><span class="sxs-lookup"><span data-stu-id="ca51d-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="ca51d-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ca51d-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="ca51d-122">Atualize as propriedades graváveis de uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="ca51d-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="ca51d-123">Delete</span><span class="sxs-lookup"><span data-stu-id="ca51d-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="ca51d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca51d-124">None</span></span> |<span data-ttu-id="ca51d-125">Exclua a pasta de tarefas do Outlook especificada.</span><span class="sxs-lookup"><span data-stu-id="ca51d-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="ca51d-126">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="ca51d-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="ca51d-127">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="ca51d-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="ca51d-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ca51d-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="ca51d-129">Crie um ou mais propriedades estendidas de valor único em uma pasta de tarefas do Outlook nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="ca51d-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="ca51d-130">Obter a pasta de tarefas com a propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="ca51d-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="ca51d-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ca51d-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="ca51d-132">Obtenha as pastas de tarefas do Outlook que contêm um valor único propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ca51d-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="ca51d-133">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="ca51d-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="ca51d-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ca51d-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="ca51d-135">Crie um ou mais propriedades estendidas de valores múltiplos em uma pasta de tarefas do Outlook nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="ca51d-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="ca51d-136">Obter a pasta de tarefas com vários valores de propriedade estendida</span><span class="sxs-lookup"><span data-stu-id="ca51d-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="ca51d-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ca51d-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="ca51d-138">Obtenha uma pasta de tarefas do Outlook que contenha uma propriedade de valor múltiplos estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="ca51d-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="ca51d-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca51d-139">Properties</span></span>
| <span data-ttu-id="ca51d-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca51d-140">Property</span></span>     | <span data-ttu-id="ca51d-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca51d-141">Type</span></span>   |<span data-ttu-id="ca51d-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca51d-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca51d-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="ca51d-143">changeKey</span></span>|<span data-ttu-id="ca51d-144">String</span><span class="sxs-lookup"><span data-stu-id="ca51d-144">String</span></span>|<span data-ttu-id="ca51d-145">A versão da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="ca51d-145">The version of the task folder.</span></span>|
|<span data-ttu-id="ca51d-146">id</span><span class="sxs-lookup"><span data-stu-id="ca51d-146">id</span></span>|<span data-ttu-id="ca51d-147">String</span><span class="sxs-lookup"><span data-stu-id="ca51d-147">String</span></span>|<span data-ttu-id="ca51d-148">O identificador da pasta de tarefas, exclusivo na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ca51d-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="ca51d-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca51d-149">Read-only.</span></span>|
|<span data-ttu-id="ca51d-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="ca51d-150">isDefaultFolder</span></span>|<span data-ttu-id="ca51d-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca51d-151">Boolean</span></span>|<span data-ttu-id="ca51d-152">True se a pasta está na pasta de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="ca51d-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="ca51d-153">name</span><span class="sxs-lookup"><span data-stu-id="ca51d-153">name</span></span>|<span data-ttu-id="ca51d-154">String</span><span class="sxs-lookup"><span data-stu-id="ca51d-154">String</span></span>|<span data-ttu-id="ca51d-155">O nome da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="ca51d-155">The name of the task folder.</span></span>|
|<span data-ttu-id="ca51d-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="ca51d-156">parentGroupKey</span></span>|<span data-ttu-id="ca51d-157">Guid</span><span class="sxs-lookup"><span data-stu-id="ca51d-157">Guid</span></span>|<span data-ttu-id="ca51d-158">O identificador GUID exclusivo para o grupo do pai da pasta tarefa.</span><span class="sxs-lookup"><span data-stu-id="ca51d-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca51d-159">Relações</span><span class="sxs-lookup"><span data-stu-id="ca51d-159">Relationships</span></span>
| <span data-ttu-id="ca51d-160">Relação</span><span class="sxs-lookup"><span data-stu-id="ca51d-160">Relationship</span></span> | <span data-ttu-id="ca51d-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca51d-161">Type</span></span>   |<span data-ttu-id="ca51d-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca51d-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca51d-163">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ca51d-163">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="ca51d-164">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ca51d-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="ca51d-165">A coleção de propriedades estendidas de múltiplos valores definidos para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="ca51d-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="ca51d-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca51d-166">Read-only.</span></span> <span data-ttu-id="ca51d-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ca51d-167">Nullable.</span></span>|
|<span data-ttu-id="ca51d-168">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ca51d-168">singleValueLegacyExtendedProperty</span></span>|<span data-ttu-id="ca51d-169">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ca51d-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="ca51d-170">A coleção de propriedades estendidas de valor único definidos para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="ca51d-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="ca51d-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca51d-171">Read-only.</span></span> <span data-ttu-id="ca51d-172">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ca51d-172">Nullable.</span></span>|
|<span data-ttu-id="ca51d-173">tarefas</span><span class="sxs-lookup"><span data-stu-id="ca51d-173">tasks</span></span>|<span data-ttu-id="ca51d-174">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="ca51d-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="ca51d-175">As tarefas nesta pasta tarefa.</span><span class="sxs-lookup"><span data-stu-id="ca51d-175">The tasks in this task folder.</span></span> <span data-ttu-id="ca51d-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca51d-176">Read-only.</span></span> <span data-ttu-id="ca51d-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ca51d-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca51d-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca51d-178">JSON representation</span></span>
<span data-ttu-id="ca51d-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca51d-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty",
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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
