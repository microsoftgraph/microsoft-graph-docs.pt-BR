---
title: tipo de recurso outlookTaskFolder
description: 'Uma pasta que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 631da782e47325a2ff28eb6ae9eb1447e1b0a14d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009255"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="55d7c-103">tipo de recurso outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55d7c-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55d7c-104">Uma pasta que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="55d7c-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="55d7c-105">No Outlook, o grupo de tarefas padrão `My Tasks`, contém uma pasta de tarefas padrão `Tasks`,, para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="55d7c-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="55d7c-106">Não é possível renomear ou excluir essas pastas e o grupo de tarefas padrão, mas você pode criar grupos de tarefas e pastas de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="55d7c-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="55d7c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="55d7c-107">Methods</span></span>

| <span data-ttu-id="55d7c-108">Método</span><span class="sxs-lookup"><span data-stu-id="55d7c-108">Method</span></span>           | <span data-ttu-id="55d7c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="55d7c-109">Return Type</span></span>    |<span data-ttu-id="55d7c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="55d7c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55d7c-111">Obter outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55d7c-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="55d7c-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55d7c-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="55d7c-113">Obtenha as propriedades e os relacionamentos da pasta de tarefas especificada do Outlook.</span><span class="sxs-lookup"><span data-stu-id="55d7c-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="55d7c-114">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="55d7c-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="55d7c-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="55d7c-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="55d7c-116">Criar uma tarefa do Outlook na pasta de tarefas especificada.</span><span class="sxs-lookup"><span data-stu-id="55d7c-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="55d7c-117">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="55d7c-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="55d7c-118">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="55d7c-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="55d7c-119">Obter todas as tarefas do Outlook na pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="55d7c-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="55d7c-120">Atualização</span><span class="sxs-lookup"><span data-stu-id="55d7c-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="55d7c-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55d7c-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="55d7c-122">Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="55d7c-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="55d7c-123">Delete</span><span class="sxs-lookup"><span data-stu-id="55d7c-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="55d7c-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55d7c-124">None</span></span> |<span data-ttu-id="55d7c-125">Excluir a pasta de tarefas do Outlook especificada.</span><span class="sxs-lookup"><span data-stu-id="55d7c-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="55d7c-126">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="55d7c-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="55d7c-127">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="55d7c-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="55d7c-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55d7c-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="55d7c-129">Crie uma ou mais propriedades estendidas de valor único em uma pasta de tarefas Nova ou existente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="55d7c-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="55d7c-130">Obter pasta de tarefas com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="55d7c-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="55d7c-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55d7c-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="55d7c-132">Obter pastas de tarefas do Outlook que contenham uma propriedade estendida `$expand` de `$filter`valor único usando ou.</span><span class="sxs-lookup"><span data-stu-id="55d7c-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="55d7c-133">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="55d7c-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="55d7c-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55d7c-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="55d7c-135">Criar uma ou mais propriedades estendidas de vários valores em uma pasta de tarefas Nova ou existente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="55d7c-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="55d7c-136">Obter pasta de tarefas com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="55d7c-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="55d7c-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55d7c-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="55d7c-138">Obtenha uma pasta de tarefas do Outlook que contenha uma propriedade estendida de `$expand`vários valores usando.</span><span class="sxs-lookup"><span data-stu-id="55d7c-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="55d7c-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55d7c-139">Properties</span></span>
| <span data-ttu-id="55d7c-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55d7c-140">Property</span></span>     | <span data-ttu-id="55d7c-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="55d7c-141">Type</span></span>   |<span data-ttu-id="55d7c-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="55d7c-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55d7c-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="55d7c-143">changeKey</span></span>|<span data-ttu-id="55d7c-144">String</span><span class="sxs-lookup"><span data-stu-id="55d7c-144">String</span></span>|<span data-ttu-id="55d7c-145">A versão da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="55d7c-145">The version of the task folder.</span></span>|
|<span data-ttu-id="55d7c-146">id</span><span class="sxs-lookup"><span data-stu-id="55d7c-146">id</span></span>|<span data-ttu-id="55d7c-147">String</span><span class="sxs-lookup"><span data-stu-id="55d7c-147">String</span></span>|<span data-ttu-id="55d7c-148">O identificador da pasta de tarefas, exclusivo na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="55d7c-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="55d7c-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55d7c-149">Read-only.</span></span>|
|<span data-ttu-id="55d7c-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="55d7c-150">isDefaultFolder</span></span>|<span data-ttu-id="55d7c-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="55d7c-151">Boolean</span></span>|<span data-ttu-id="55d7c-152">True se a pasta é a pasta de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="55d7c-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="55d7c-153">name</span><span class="sxs-lookup"><span data-stu-id="55d7c-153">name</span></span>|<span data-ttu-id="55d7c-154">String</span><span class="sxs-lookup"><span data-stu-id="55d7c-154">String</span></span>|<span data-ttu-id="55d7c-155">O nome da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="55d7c-155">The name of the task folder.</span></span>|
|<span data-ttu-id="55d7c-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="55d7c-156">parentGroupKey</span></span>|<span data-ttu-id="55d7c-157">Guid</span><span class="sxs-lookup"><span data-stu-id="55d7c-157">Guid</span></span>|<span data-ttu-id="55d7c-158">O identificador exclusivo do GUID para o grupo pai da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="55d7c-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55d7c-159">Relações</span><span class="sxs-lookup"><span data-stu-id="55d7c-159">Relationships</span></span>
| <span data-ttu-id="55d7c-160">Relação</span><span class="sxs-lookup"><span data-stu-id="55d7c-160">Relationship</span></span> | <span data-ttu-id="55d7c-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="55d7c-161">Type</span></span>   |<span data-ttu-id="55d7c-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="55d7c-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55d7c-163">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="55d7c-163">multiValueExtendedProperties</span></span>|<span data-ttu-id="55d7c-164">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="55d7c-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="55d7c-165">A coleção de propriedades estendidas de vários valores definida para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="55d7c-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="55d7c-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55d7c-166">Read-only.</span></span> <span data-ttu-id="55d7c-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="55d7c-167">Nullable.</span></span>|
|<span data-ttu-id="55d7c-168">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="55d7c-168">singleValueExtendedProperties</span></span>|<span data-ttu-id="55d7c-169">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="55d7c-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="55d7c-170">A coleção de propriedades estendidas de valor único definidas para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="55d7c-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="55d7c-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55d7c-171">Read-only.</span></span> <span data-ttu-id="55d7c-172">Anulável.</span><span class="sxs-lookup"><span data-stu-id="55d7c-172">Nullable.</span></span>|
|<span data-ttu-id="55d7c-173">tarefas</span><span class="sxs-lookup"><span data-stu-id="55d7c-173">tasks</span></span>|<span data-ttu-id="55d7c-174">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="55d7c-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="55d7c-175">As tarefas nesta pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="55d7c-175">The tasks in this task folder.</span></span> <span data-ttu-id="55d7c-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55d7c-176">Read-only.</span></span> <span data-ttu-id="55d7c-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="55d7c-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55d7c-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55d7c-178">JSON representation</span></span>
<span data-ttu-id="55d7c-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55d7c-179">Here is a JSON representation of the resource.</span></span>

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
