---
title: tipo de recurso outlookTaskGroup
description: 'Um grupo de pastas (outlookTaskFolder) que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: afd5da7663a9328a87b5df2616b0093a4208caeb
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312114"
---
# <a name="outlooktaskgroup-resource-type-deprecated"></a><span data-ttu-id="d71da-103">tipo de recurso outlookTaskGroup (preterido)</span><span class="sxs-lookup"><span data-stu-id="d71da-103">outlookTaskGroup resource type (deprecated)</span></span>

<span data-ttu-id="d71da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d71da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="d71da-105">Um grupo de pastas ([outlookTaskFolder](outlooktaskfolder.md)) que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="d71da-105">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="d71da-106">No Outlook, há um grupo de tarefas padrão `My Tasks` que você não pode renomear ou excluir.</span><span class="sxs-lookup"><span data-stu-id="d71da-106">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="d71da-107">No entanto, você pode criar grupos de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="d71da-107">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="d71da-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d71da-108">Methods</span></span>

| <span data-ttu-id="d71da-109">Método</span><span class="sxs-lookup"><span data-stu-id="d71da-109">Method</span></span>           | <span data-ttu-id="d71da-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d71da-110">Return Type</span></span>    |<span data-ttu-id="d71da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d71da-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d71da-112">Obter outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d71da-112">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="d71da-113">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d71da-113">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="d71da-114">Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d71da-114">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="d71da-115">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="d71da-115">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="d71da-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="d71da-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="d71da-117">Criar uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d71da-117">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="d71da-118">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="d71da-118">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="d71da-119">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="d71da-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="d71da-120">Obter uma coleção de pastas de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d71da-120">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="d71da-121">Update</span><span class="sxs-lookup"><span data-stu-id="d71da-121">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="d71da-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d71da-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="d71da-123">Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d71da-123">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="d71da-124">Delete</span><span class="sxs-lookup"><span data-stu-id="d71da-124">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="d71da-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d71da-125">None</span></span> |<span data-ttu-id="d71da-126">Excluir o grupo de tarefas do Outlook especificado.</span><span class="sxs-lookup"><span data-stu-id="d71da-126">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="d71da-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d71da-127">Properties</span></span>
| <span data-ttu-id="d71da-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d71da-128">Property</span></span>     | <span data-ttu-id="d71da-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d71da-129">Type</span></span>   |<span data-ttu-id="d71da-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d71da-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d71da-131">changeKey</span><span class="sxs-lookup"><span data-stu-id="d71da-131">changeKey</span></span>|<span data-ttu-id="d71da-132">String</span><span class="sxs-lookup"><span data-stu-id="d71da-132">String</span></span>|<span data-ttu-id="d71da-133">A versão do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d71da-133">The version of the task group.</span></span>|
|<span data-ttu-id="d71da-134">groupKey</span><span class="sxs-lookup"><span data-stu-id="d71da-134">groupKey</span></span>|<span data-ttu-id="d71da-135">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="d71da-135">Edm.Guid</span></span>|<span data-ttu-id="d71da-136">O identificador exclusivo do GUID do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d71da-136">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="d71da-137">id</span><span class="sxs-lookup"><span data-stu-id="d71da-137">id</span></span>|<span data-ttu-id="d71da-138">String</span><span class="sxs-lookup"><span data-stu-id="d71da-138">String</span></span>|<span data-ttu-id="d71da-139">O identificador exclusivo da cadeia de caracteres do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d71da-139">The unique string identifier of the task group.</span></span> <span data-ttu-id="d71da-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d71da-140">Read-only.</span></span>|
|<span data-ttu-id="d71da-141">IsDefault</span><span class="sxs-lookup"><span data-stu-id="d71da-141">isDefaultGroup</span></span>|<span data-ttu-id="d71da-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="d71da-142">Boolean</span></span>|<span data-ttu-id="d71da-143">True se o grupo de tarefas é o grupo de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="d71da-143">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="d71da-144">nome</span><span class="sxs-lookup"><span data-stu-id="d71da-144">name</span></span>|<span data-ttu-id="d71da-145">String</span><span class="sxs-lookup"><span data-stu-id="d71da-145">String</span></span>|<span data-ttu-id="d71da-146">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d71da-146">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d71da-147">Relações</span><span class="sxs-lookup"><span data-stu-id="d71da-147">Relationships</span></span>
| <span data-ttu-id="d71da-148">Relação</span><span class="sxs-lookup"><span data-stu-id="d71da-148">Relationship</span></span> | <span data-ttu-id="d71da-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="d71da-149">Type</span></span>   |<span data-ttu-id="d71da-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="d71da-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d71da-151">taskFolders</span><span class="sxs-lookup"><span data-stu-id="d71da-151">taskFolders</span></span>|<span data-ttu-id="d71da-152">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="d71da-152">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="d71da-153">O conjunto de pastas de tarefas no grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d71da-153">The collection of task folders in the task group.</span></span> <span data-ttu-id="d71da-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d71da-154">Read-only.</span></span> <span data-ttu-id="d71da-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d71da-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d71da-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d71da-156">JSON representation</span></span>
<span data-ttu-id="d71da-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d71da-157">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
