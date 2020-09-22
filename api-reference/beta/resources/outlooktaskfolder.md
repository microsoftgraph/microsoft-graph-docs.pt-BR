---
title: tipo de recurso outlookTaskFolder
description: 'Uma pasta que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c9f9958750cca1aaa40ba9394832e5974bed8cc3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998359"
---
# <a name="outlooktaskfolder-resource-type-deprecated"></a><span data-ttu-id="61d1d-103">tipo de recurso outlookTaskFolder (preterido)</span><span class="sxs-lookup"><span data-stu-id="61d1d-103">outlookTaskFolder resource type (deprecated)</span></span>

<span data-ttu-id="61d1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61d1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="61d1d-105">Uma pasta que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="61d1d-105">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="61d1d-106">No Outlook, o grupo de tarefas padrão, `My Tasks` contém uma pasta de tarefas padrão, `Tasks` , para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="61d1d-106">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="61d1d-107">Não é possível renomear ou excluir essas pastas e o grupo de tarefas padrão, mas você pode criar grupos de tarefas e pastas de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="61d1d-107">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="61d1d-108">Methods</span><span class="sxs-lookup"><span data-stu-id="61d1d-108">Methods</span></span>

| <span data-ttu-id="61d1d-109">Método</span><span class="sxs-lookup"><span data-stu-id="61d1d-109">Method</span></span>           | <span data-ttu-id="61d1d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="61d1d-110">Return Type</span></span>    |<span data-ttu-id="61d1d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d1d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="61d1d-112">Obter outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="61d1d-112">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="61d1d-113">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="61d1d-113">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="61d1d-114">Obtenha as propriedades e os relacionamentos da pasta de tarefas especificada do Outlook.</span><span class="sxs-lookup"><span data-stu-id="61d1d-114">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="61d1d-115">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="61d1d-115">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="61d1d-116">outlookTask</span><span class="sxs-lookup"><span data-stu-id="61d1d-116">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="61d1d-117">Criar uma tarefa do Outlook na pasta de tarefas especificada.</span><span class="sxs-lookup"><span data-stu-id="61d1d-117">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="61d1d-118">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="61d1d-118">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="61d1d-119">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="61d1d-119">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="61d1d-120">Obter todas as tarefas do Outlook na pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="61d1d-120">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="61d1d-121">Atualização</span><span class="sxs-lookup"><span data-stu-id="61d1d-121">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="61d1d-122">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="61d1d-122">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="61d1d-123">Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="61d1d-123">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="61d1d-124">Delete</span><span class="sxs-lookup"><span data-stu-id="61d1d-124">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="61d1d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61d1d-125">None</span></span> |<span data-ttu-id="61d1d-126">Excluir a pasta de tarefas do Outlook especificada.</span><span class="sxs-lookup"><span data-stu-id="61d1d-126">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="61d1d-127">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="61d1d-127">**Extended properties**</span></span>| | |
|[<span data-ttu-id="61d1d-128">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="61d1d-128">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="61d1d-129">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="61d1d-129">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="61d1d-130">Crie uma ou mais propriedades estendidas de valor único em uma pasta de tarefas Nova ou existente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="61d1d-130">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="61d1d-131">Obter pasta de tarefas com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="61d1d-131">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="61d1d-132">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="61d1d-132">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="61d1d-133">Obter pastas de tarefas do Outlook que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter` .</span><span class="sxs-lookup"><span data-stu-id="61d1d-133">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="61d1d-134">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="61d1d-134">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="61d1d-135">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="61d1d-135">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="61d1d-136">Criar uma ou mais propriedades estendidas de vários valores em uma pasta de tarefas Nova ou existente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="61d1d-136">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="61d1d-137">Obter pasta de tarefas com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="61d1d-137">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="61d1d-138">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="61d1d-138">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="61d1d-139">Obtenha uma pasta de tarefas do Outlook que contenha uma propriedade estendida de vários valores usando `$expand` .</span><span class="sxs-lookup"><span data-stu-id="61d1d-139">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="61d1d-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61d1d-140">Properties</span></span>
| <span data-ttu-id="61d1d-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61d1d-141">Property</span></span>     | <span data-ttu-id="61d1d-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="61d1d-142">Type</span></span>   |<span data-ttu-id="61d1d-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d1d-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61d1d-144">changeKey</span><span class="sxs-lookup"><span data-stu-id="61d1d-144">changeKey</span></span>|<span data-ttu-id="61d1d-145">String</span><span class="sxs-lookup"><span data-stu-id="61d1d-145">String</span></span>|<span data-ttu-id="61d1d-146">A versão da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="61d1d-146">The version of the task folder.</span></span>|
|<span data-ttu-id="61d1d-147">id</span><span class="sxs-lookup"><span data-stu-id="61d1d-147">id</span></span>|<span data-ttu-id="61d1d-148">String</span><span class="sxs-lookup"><span data-stu-id="61d1d-148">String</span></span>|<span data-ttu-id="61d1d-149">O identificador da pasta de tarefas, exclusivo na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="61d1d-149">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="61d1d-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61d1d-150">Read-only.</span></span>|
|<span data-ttu-id="61d1d-151">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="61d1d-151">isDefaultFolder</span></span>|<span data-ttu-id="61d1d-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="61d1d-152">Boolean</span></span>|<span data-ttu-id="61d1d-153">True se a pasta é a pasta de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="61d1d-153">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="61d1d-154">nome</span><span class="sxs-lookup"><span data-stu-id="61d1d-154">name</span></span>|<span data-ttu-id="61d1d-155">String</span><span class="sxs-lookup"><span data-stu-id="61d1d-155">String</span></span>|<span data-ttu-id="61d1d-156">O nome da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="61d1d-156">The name of the task folder.</span></span>|
|<span data-ttu-id="61d1d-157">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="61d1d-157">parentGroupKey</span></span>|<span data-ttu-id="61d1d-158">Guid</span><span class="sxs-lookup"><span data-stu-id="61d1d-158">Guid</span></span>|<span data-ttu-id="61d1d-159">O identificador exclusivo do GUID para o grupo pai da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="61d1d-159">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61d1d-160">Relações</span><span class="sxs-lookup"><span data-stu-id="61d1d-160">Relationships</span></span>
| <span data-ttu-id="61d1d-161">Relação</span><span class="sxs-lookup"><span data-stu-id="61d1d-161">Relationship</span></span> | <span data-ttu-id="61d1d-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="61d1d-162">Type</span></span>   |<span data-ttu-id="61d1d-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d1d-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61d1d-164">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="61d1d-164">multiValueExtendedProperties</span></span>|<span data-ttu-id="61d1d-165">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="61d1d-165">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="61d1d-166">A coleção de propriedades estendidas de vários valores definida para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="61d1d-166">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="61d1d-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61d1d-167">Read-only.</span></span> <span data-ttu-id="61d1d-168">Anulável.</span><span class="sxs-lookup"><span data-stu-id="61d1d-168">Nullable.</span></span>|
|<span data-ttu-id="61d1d-169">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="61d1d-169">singleValueExtendedProperties</span></span>|<span data-ttu-id="61d1d-170">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="61d1d-170">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="61d1d-171">A coleção de propriedades estendidas de valor único definidas para a pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="61d1d-171">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="61d1d-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61d1d-172">Read-only.</span></span> <span data-ttu-id="61d1d-173">Anulável.</span><span class="sxs-lookup"><span data-stu-id="61d1d-173">Nullable.</span></span>|
|<span data-ttu-id="61d1d-174">tarefas</span><span class="sxs-lookup"><span data-stu-id="61d1d-174">tasks</span></span>|<span data-ttu-id="61d1d-175">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="61d1d-175">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="61d1d-176">As tarefas nesta pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="61d1d-176">The tasks in this task folder.</span></span> <span data-ttu-id="61d1d-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61d1d-177">Read-only.</span></span> <span data-ttu-id="61d1d-178">Anulável.</span><span class="sxs-lookup"><span data-stu-id="61d1d-178">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61d1d-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61d1d-179">JSON representation</span></span>
<span data-ttu-id="61d1d-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61d1d-180">Here is a JSON representation of the resource.</span></span>

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


