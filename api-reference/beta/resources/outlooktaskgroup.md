---
title: tipo de recurso outlookTaskGroup
description: 'Um grupo de pastas (outlookTaskFolder) que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8018863ed7fd142b99e0008f860495a4d13d4e01
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463207"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="c32b5-103">tipo de recurso outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c32b5-103">outlookTaskGroup resource type</span></span>

<span data-ttu-id="c32b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c32b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c32b5-105">Um grupo de pastas ([outlookTaskFolder](outlooktaskfolder.md)) que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="c32b5-105">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="c32b5-106">No Outlook, há um grupo `My Tasks` de tarefas padrão que você não pode renomear ou excluir.</span><span class="sxs-lookup"><span data-stu-id="c32b5-106">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="c32b5-107">No entanto, você pode criar grupos de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="c32b5-107">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="c32b5-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c32b5-108">Methods</span></span>

| <span data-ttu-id="c32b5-109">Método</span><span class="sxs-lookup"><span data-stu-id="c32b5-109">Method</span></span>           | <span data-ttu-id="c32b5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c32b5-110">Return Type</span></span>    |<span data-ttu-id="c32b5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c32b5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c32b5-112">Obter outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c32b5-112">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="c32b5-113">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c32b5-113">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="c32b5-114">Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="c32b5-114">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="c32b5-115">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c32b5-115">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="c32b5-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c32b5-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="c32b5-117">Criar uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="c32b5-117">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="c32b5-118">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="c32b5-118">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="c32b5-119">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="c32b5-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="c32b5-120">Obter uma coleção de pastas de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="c32b5-120">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="c32b5-121">Atualizar</span><span class="sxs-lookup"><span data-stu-id="c32b5-121">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="c32b5-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c32b5-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="c32b5-123">Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="c32b5-123">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="c32b5-124">Excluir</span><span class="sxs-lookup"><span data-stu-id="c32b5-124">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="c32b5-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c32b5-125">None</span></span> |<span data-ttu-id="c32b5-126">Excluir o grupo de tarefas do Outlook especificado.</span><span class="sxs-lookup"><span data-stu-id="c32b5-126">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="c32b5-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c32b5-127">Properties</span></span>
| <span data-ttu-id="c32b5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c32b5-128">Property</span></span>     | <span data-ttu-id="c32b5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c32b5-129">Type</span></span>   |<span data-ttu-id="c32b5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c32b5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c32b5-131">changeKey</span><span class="sxs-lookup"><span data-stu-id="c32b5-131">changeKey</span></span>|<span data-ttu-id="c32b5-132">String</span><span class="sxs-lookup"><span data-stu-id="c32b5-132">String</span></span>|<span data-ttu-id="c32b5-133">A versão do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="c32b5-133">The version of the task group.</span></span>|
|<span data-ttu-id="c32b5-134">groupKey</span><span class="sxs-lookup"><span data-stu-id="c32b5-134">groupKey</span></span>|<span data-ttu-id="c32b5-135">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="c32b5-135">Edm.Guid</span></span>|<span data-ttu-id="c32b5-136">O identificador exclusivo do GUID do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="c32b5-136">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="c32b5-137">id</span><span class="sxs-lookup"><span data-stu-id="c32b5-137">id</span></span>|<span data-ttu-id="c32b5-138">String</span><span class="sxs-lookup"><span data-stu-id="c32b5-138">String</span></span>|<span data-ttu-id="c32b5-139">O identificador exclusivo da cadeia de caracteres do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="c32b5-139">The unique string identifier of the task group.</span></span> <span data-ttu-id="c32b5-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c32b5-140">Read-only.</span></span>|
|<span data-ttu-id="c32b5-141">IsDefault</span><span class="sxs-lookup"><span data-stu-id="c32b5-141">isDefaultGroup</span></span>|<span data-ttu-id="c32b5-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="c32b5-142">Boolean</span></span>|<span data-ttu-id="c32b5-143">True se o grupo de tarefas é o grupo de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="c32b5-143">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="c32b5-144">nome</span><span class="sxs-lookup"><span data-stu-id="c32b5-144">name</span></span>|<span data-ttu-id="c32b5-145">String</span><span class="sxs-lookup"><span data-stu-id="c32b5-145">String</span></span>|<span data-ttu-id="c32b5-146">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="c32b5-146">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c32b5-147">Relações</span><span class="sxs-lookup"><span data-stu-id="c32b5-147">Relationships</span></span>
| <span data-ttu-id="c32b5-148">Relação</span><span class="sxs-lookup"><span data-stu-id="c32b5-148">Relationship</span></span> | <span data-ttu-id="c32b5-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="c32b5-149">Type</span></span>   |<span data-ttu-id="c32b5-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="c32b5-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c32b5-151">taskFolders</span><span class="sxs-lookup"><span data-stu-id="c32b5-151">taskFolders</span></span>|<span data-ttu-id="c32b5-152">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="c32b5-152">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="c32b5-153">O conjunto de pastas de tarefas no grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="c32b5-153">The collection of task folders in the task group.</span></span> <span data-ttu-id="c32b5-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c32b5-154">Read-only.</span></span> <span data-ttu-id="c32b5-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c32b5-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c32b5-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c32b5-156">JSON representation</span></span>
<span data-ttu-id="c32b5-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c32b5-157">Here is a JSON representation of the resource.</span></span>

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
