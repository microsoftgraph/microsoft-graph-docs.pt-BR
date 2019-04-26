---
title: tipo de recurso outlookTaskGroup
description: 'Um grupo de pastas (outlookTaskFolder) que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af5599773c6a4edef97356e99daa522760d9b37a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345526"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="2015e-103">tipo de recurso outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="2015e-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2015e-104">Um grupo de pastas ([outlookTaskFolder](outlooktaskfolder.md)) que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="2015e-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="2015e-105">No Outlook, há um grupo `My Tasks` de tarefas padrão que você não pode renomear ou excluir.</span><span class="sxs-lookup"><span data-stu-id="2015e-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="2015e-106">No entanto, você pode criar grupos de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="2015e-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="2015e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2015e-107">Methods</span></span>

| <span data-ttu-id="2015e-108">Método</span><span class="sxs-lookup"><span data-stu-id="2015e-108">Method</span></span>           | <span data-ttu-id="2015e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2015e-109">Return Type</span></span>    |<span data-ttu-id="2015e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2015e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2015e-111">Obter outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="2015e-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="2015e-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="2015e-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="2015e-113">Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2015e-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="2015e-114">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2015e-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="2015e-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2015e-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="2015e-116">Criar uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2015e-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="2015e-117">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="2015e-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="2015e-118">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="2015e-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="2015e-119">Obter uma coleção de pastas de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2015e-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="2015e-120">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2015e-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="2015e-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="2015e-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="2015e-122">Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2015e-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="2015e-123">Delete</span><span class="sxs-lookup"><span data-stu-id="2015e-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="2015e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2015e-124">None</span></span> |<span data-ttu-id="2015e-125">Excluir o grupo de tarefas do Outlook especificado.</span><span class="sxs-lookup"><span data-stu-id="2015e-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="2015e-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2015e-126">Properties</span></span>
| <span data-ttu-id="2015e-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2015e-127">Property</span></span>     | <span data-ttu-id="2015e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2015e-128">Type</span></span>   |<span data-ttu-id="2015e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2015e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2015e-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="2015e-130">changeKey</span></span>|<span data-ttu-id="2015e-131">String</span><span class="sxs-lookup"><span data-stu-id="2015e-131">String</span></span>|<span data-ttu-id="2015e-132">A versão do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="2015e-132">The version of the task group.</span></span>|
|<span data-ttu-id="2015e-133">groupKey</span><span class="sxs-lookup"><span data-stu-id="2015e-133">groupKey</span></span>|<span data-ttu-id="2015e-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="2015e-134">Edm.Guid</span></span>|<span data-ttu-id="2015e-135">O identificador exclusivo do GUID do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="2015e-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="2015e-136">id</span><span class="sxs-lookup"><span data-stu-id="2015e-136">id</span></span>|<span data-ttu-id="2015e-137">String</span><span class="sxs-lookup"><span data-stu-id="2015e-137">String</span></span>|<span data-ttu-id="2015e-138">O identificador exclusivo da cadeia de caracteres do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="2015e-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="2015e-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2015e-139">Read-only.</span></span>|
|<span data-ttu-id="2015e-140">isDefault</span><span class="sxs-lookup"><span data-stu-id="2015e-140">isDefaultGroup</span></span>|<span data-ttu-id="2015e-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="2015e-141">Boolean</span></span>|<span data-ttu-id="2015e-142">True se o grupo de tarefas é o grupo de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="2015e-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="2015e-143">name</span><span class="sxs-lookup"><span data-stu-id="2015e-143">name</span></span>|<span data-ttu-id="2015e-144">String</span><span class="sxs-lookup"><span data-stu-id="2015e-144">String</span></span>|<span data-ttu-id="2015e-145">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="2015e-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2015e-146">Relações</span><span class="sxs-lookup"><span data-stu-id="2015e-146">Relationships</span></span>
| <span data-ttu-id="2015e-147">Relação</span><span class="sxs-lookup"><span data-stu-id="2015e-147">Relationship</span></span> | <span data-ttu-id="2015e-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="2015e-148">Type</span></span>   |<span data-ttu-id="2015e-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="2015e-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2015e-150">taskFolders</span><span class="sxs-lookup"><span data-stu-id="2015e-150">taskFolders</span></span>|<span data-ttu-id="2015e-151">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="2015e-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="2015e-152">O conjunto de pastas de tarefas no grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="2015e-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="2015e-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2015e-153">Read-only.</span></span> <span data-ttu-id="2015e-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2015e-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2015e-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2015e-155">JSON representation</span></span>
<span data-ttu-id="2015e-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2015e-156">Here is a JSON representation of the resource.</span></span>

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
