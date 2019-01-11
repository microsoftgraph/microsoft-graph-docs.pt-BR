---
title: tipo de recurso de outlookTaskGroup
description: 'Um grupo de pastas (outlookTaskFolder) que contêm tarefas do Outlook (coleção de objetos outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5e885c4c8cc2abe4b3890635e010d495267dc877
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878768"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="f2782-103">tipo de recurso de outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f2782-103">outlookTaskGroup resource type</span></span>

> <span data-ttu-id="f2782-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2782-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2782-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2782-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2782-106">Um grupo de pastas ([outlookTaskFolder](outlooktaskfolder.md)) que contêm tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="f2782-106">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="f2782-107">No Outlook, há um grupo de tarefas padrão `My Tasks` que não é possível renomear ou excluir.</span><span class="sxs-lookup"><span data-stu-id="f2782-107">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="f2782-108">No entanto, você pode criar grupos de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="f2782-108">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="f2782-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2782-109">Methods</span></span>

| <span data-ttu-id="f2782-110">Método</span><span class="sxs-lookup"><span data-stu-id="f2782-110">Method</span></span>           | <span data-ttu-id="f2782-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2782-111">Return Type</span></span>    |<span data-ttu-id="f2782-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2782-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2782-113">Obter outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f2782-113">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="f2782-114">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f2782-114">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="f2782-115">Obtenha as propriedades e relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f2782-115">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="f2782-116">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="f2782-116">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="f2782-117">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="f2782-117">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="f2782-118">Crie uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f2782-118">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="f2782-119">Lista taskFolders</span><span class="sxs-lookup"><span data-stu-id="f2782-119">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="f2782-120">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="f2782-120">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="f2782-121">Obtenha uma coleção de pastas de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f2782-121">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="f2782-122">Update</span><span class="sxs-lookup"><span data-stu-id="f2782-122">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="f2782-123">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f2782-123">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="f2782-124">Atualize as propriedades graváveis de um grupo de tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f2782-124">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="f2782-125">Delete</span><span class="sxs-lookup"><span data-stu-id="f2782-125">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="f2782-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2782-126">None</span></span> |<span data-ttu-id="f2782-127">Exclua o grupo de tarefas do Outlook especificado.</span><span class="sxs-lookup"><span data-stu-id="f2782-127">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="f2782-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2782-128">Properties</span></span>
| <span data-ttu-id="f2782-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2782-129">Property</span></span>     | <span data-ttu-id="f2782-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2782-130">Type</span></span>   |<span data-ttu-id="f2782-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2782-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2782-132">changeKey</span><span class="sxs-lookup"><span data-stu-id="f2782-132">changeKey</span></span>|<span data-ttu-id="f2782-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2782-133">String</span></span>|<span data-ttu-id="f2782-134">A versão do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="f2782-134">The version of the task group.</span></span>|
|<span data-ttu-id="f2782-135">groupKey</span><span class="sxs-lookup"><span data-stu-id="f2782-135">groupKey</span></span>|<span data-ttu-id="f2782-136">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="f2782-136">Edm.Guid</span></span>|<span data-ttu-id="f2782-137">O identificador GUID exclusivo para o grupo de tarefa.</span><span class="sxs-lookup"><span data-stu-id="f2782-137">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="f2782-138">id</span><span class="sxs-lookup"><span data-stu-id="f2782-138">id</span></span>|<span data-ttu-id="f2782-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2782-139">String</span></span>|<span data-ttu-id="f2782-140">O identificador de cadeia de caracteres exclusiva do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="f2782-140">The unique string identifier of the task group.</span></span> <span data-ttu-id="f2782-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2782-141">Read-only.</span></span>|
|<span data-ttu-id="f2782-142">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="f2782-142">isDefaultGroup</span></span>|<span data-ttu-id="f2782-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="f2782-143">Boolean</span></span>|<span data-ttu-id="f2782-144">True se o grupo de tarefa é o grupo de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="f2782-144">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="f2782-145">name</span><span class="sxs-lookup"><span data-stu-id="f2782-145">name</span></span>|<span data-ttu-id="f2782-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2782-146">String</span></span>|<span data-ttu-id="f2782-147">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="f2782-147">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2782-148">Relações</span><span class="sxs-lookup"><span data-stu-id="f2782-148">Relationships</span></span>
| <span data-ttu-id="f2782-149">Relação</span><span class="sxs-lookup"><span data-stu-id="f2782-149">Relationship</span></span> | <span data-ttu-id="f2782-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2782-150">Type</span></span>   |<span data-ttu-id="f2782-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2782-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2782-152">taskFolders</span><span class="sxs-lookup"><span data-stu-id="f2782-152">taskFolders</span></span>|<span data-ttu-id="f2782-153">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="f2782-153">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="f2782-154">A coleção de pastas de tarefa no grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="f2782-154">The collection of task folders in the task group.</span></span> <span data-ttu-id="f2782-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2782-155">Read-only.</span></span> <span data-ttu-id="f2782-156">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f2782-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2782-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2782-157">JSON representation</span></span>
<span data-ttu-id="f2782-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2782-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
