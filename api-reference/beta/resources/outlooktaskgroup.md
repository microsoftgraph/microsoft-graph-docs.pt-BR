---
title: tipo de recurso outlookTaskGroup
description: 'Um grupo de pastas (outlookTaskFolder) que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 67439b11cc2067df23c71cf9fc939fbfb250f874
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522071"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="d42fa-103">tipo de recurso outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d42fa-103">outlookTaskGroup resource type</span></span>

<span data-ttu-id="d42fa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d42fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d42fa-105">Um grupo de pastas ([outlookTaskFolder](outlooktaskfolder.md)) que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="d42fa-105">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="d42fa-106">No Outlook, há um grupo `My Tasks` de tarefas padrão que você não pode renomear ou excluir.</span><span class="sxs-lookup"><span data-stu-id="d42fa-106">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="d42fa-107">No entanto, você pode criar grupos de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="d42fa-107">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="d42fa-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d42fa-108">Methods</span></span>

| <span data-ttu-id="d42fa-109">Método</span><span class="sxs-lookup"><span data-stu-id="d42fa-109">Method</span></span>           | <span data-ttu-id="d42fa-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d42fa-110">Return Type</span></span>    |<span data-ttu-id="d42fa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d42fa-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d42fa-112">Obter outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d42fa-112">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="d42fa-113">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d42fa-113">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="d42fa-114">Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d42fa-114">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="d42fa-115">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="d42fa-115">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="d42fa-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="d42fa-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="d42fa-117">Criar uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d42fa-117">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="d42fa-118">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="d42fa-118">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="d42fa-119">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="d42fa-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="d42fa-120">Obter uma coleção de pastas de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d42fa-120">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="d42fa-121">Update</span><span class="sxs-lookup"><span data-stu-id="d42fa-121">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="d42fa-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d42fa-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="d42fa-123">Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d42fa-123">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="d42fa-124">Delete</span><span class="sxs-lookup"><span data-stu-id="d42fa-124">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="d42fa-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d42fa-125">None</span></span> |<span data-ttu-id="d42fa-126">Excluir o grupo de tarefas do Outlook especificado.</span><span class="sxs-lookup"><span data-stu-id="d42fa-126">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="d42fa-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d42fa-127">Properties</span></span>
| <span data-ttu-id="d42fa-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d42fa-128">Property</span></span>     | <span data-ttu-id="d42fa-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d42fa-129">Type</span></span>   |<span data-ttu-id="d42fa-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d42fa-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d42fa-131">changeKey</span><span class="sxs-lookup"><span data-stu-id="d42fa-131">changeKey</span></span>|<span data-ttu-id="d42fa-132">String</span><span class="sxs-lookup"><span data-stu-id="d42fa-132">String</span></span>|<span data-ttu-id="d42fa-133">A versão do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d42fa-133">The version of the task group.</span></span>|
|<span data-ttu-id="d42fa-134">groupKey</span><span class="sxs-lookup"><span data-stu-id="d42fa-134">groupKey</span></span>|<span data-ttu-id="d42fa-135">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="d42fa-135">Edm.Guid</span></span>|<span data-ttu-id="d42fa-136">O identificador exclusivo do GUID do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d42fa-136">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="d42fa-137">id</span><span class="sxs-lookup"><span data-stu-id="d42fa-137">id</span></span>|<span data-ttu-id="d42fa-138">String</span><span class="sxs-lookup"><span data-stu-id="d42fa-138">String</span></span>|<span data-ttu-id="d42fa-139">O identificador exclusivo da cadeia de caracteres do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d42fa-139">The unique string identifier of the task group.</span></span> <span data-ttu-id="d42fa-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d42fa-140">Read-only.</span></span>|
|<span data-ttu-id="d42fa-141">IsDefault</span><span class="sxs-lookup"><span data-stu-id="d42fa-141">isDefaultGroup</span></span>|<span data-ttu-id="d42fa-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="d42fa-142">Boolean</span></span>|<span data-ttu-id="d42fa-143">True se o grupo de tarefas é o grupo de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="d42fa-143">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="d42fa-144">nome</span><span class="sxs-lookup"><span data-stu-id="d42fa-144">name</span></span>|<span data-ttu-id="d42fa-145">String</span><span class="sxs-lookup"><span data-stu-id="d42fa-145">String</span></span>|<span data-ttu-id="d42fa-146">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d42fa-146">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d42fa-147">Relações</span><span class="sxs-lookup"><span data-stu-id="d42fa-147">Relationships</span></span>
| <span data-ttu-id="d42fa-148">Relação</span><span class="sxs-lookup"><span data-stu-id="d42fa-148">Relationship</span></span> | <span data-ttu-id="d42fa-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="d42fa-149">Type</span></span>   |<span data-ttu-id="d42fa-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="d42fa-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d42fa-151">taskFolders</span><span class="sxs-lookup"><span data-stu-id="d42fa-151">taskFolders</span></span>|<span data-ttu-id="d42fa-152">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="d42fa-152">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="d42fa-153">O conjunto de pastas de tarefas no grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d42fa-153">The collection of task folders in the task group.</span></span> <span data-ttu-id="d42fa-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d42fa-154">Read-only.</span></span> <span data-ttu-id="d42fa-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d42fa-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d42fa-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d42fa-156">JSON representation</span></span>
<span data-ttu-id="d42fa-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d42fa-157">Here is a JSON representation of the resource.</span></span>

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
