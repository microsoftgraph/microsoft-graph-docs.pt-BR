---
author: daspek
ms.author: dspektor
title: Tipo de recurso ItemActionSet
description: O objeto doactionset fornece informações sobre as ações que foram realizadas como parte de uma atividade em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 76778f959f52518ca4055a0da471bffeca5a73e7
ms.sourcegitcommit: 8a84ee922acd2946a3ffae9f8f7f7b485567bc05
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2020
ms.locfileid: "42619078"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="efc08-103">tipo de recurso doactionset</span><span class="sxs-lookup"><span data-stu-id="efc08-103">itemActionSet resource type</span></span>

<span data-ttu-id="efc08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efc08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efc08-105">O recurso **Doactionset** fornece informações sobre as ações que compõem uma [atividade][itemActivity] em um item.</span><span class="sxs-lookup"><span data-stu-id="efc08-105">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="efc08-106">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="efc08-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="efc08-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efc08-107">Properties</span></span>

<span data-ttu-id="efc08-108">As ações a seguir estão disponíveis no momento.</span><span class="sxs-lookup"><span data-stu-id="efc08-108">The following actions are currently available.</span></span> <span data-ttu-id="efc08-109">Como novas ações podem ser adicionadas no futuro, certifique-se de que seu aplicativo possa lidar **com um ItemAdded** que inclui ações desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="efc08-109">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="efc08-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="efc08-110">Property name</span></span> | <span data-ttu-id="efc08-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="efc08-111">Type</span></span>              | <span data-ttu-id="efc08-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="efc08-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="efc08-113">comment</span><span class="sxs-lookup"><span data-stu-id="efc08-113">comment</span></span>       | <span data-ttu-id="efc08-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-114">[commentAction][]</span></span> | <span data-ttu-id="efc08-115">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="efc08-115">A comment was added to the item.</span></span>
| <span data-ttu-id="efc08-116">create</span><span class="sxs-lookup"><span data-stu-id="efc08-116">create</span></span>        | <span data-ttu-id="efc08-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-117">[createAction][]</span></span>  | <span data-ttu-id="efc08-118">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="efc08-118">An item was created.</span></span>
| <span data-ttu-id="efc08-119">delete</span><span class="sxs-lookup"><span data-stu-id="efc08-119">delete</span></span>        | <span data-ttu-id="efc08-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-120">[deleteAction][]</span></span>  | <span data-ttu-id="efc08-121">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="efc08-121">An item was deleted.</span></span>
| <span data-ttu-id="efc08-122">edit</span><span class="sxs-lookup"><span data-stu-id="efc08-122">edit</span></span>          | <span data-ttu-id="efc08-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-123">[editAction][]</span></span>    | <span data-ttu-id="efc08-124">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="efc08-124">An item was edited.</span></span>
| <span data-ttu-id="efc08-125">mention</span><span class="sxs-lookup"><span data-stu-id="efc08-125">mention</span></span>       | <span data-ttu-id="efc08-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-126">[mentionAction][]</span></span> | <span data-ttu-id="efc08-127">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="efc08-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="efc08-128">move</span><span class="sxs-lookup"><span data-stu-id="efc08-128">move</span></span>          | <span data-ttu-id="efc08-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-129">[moveAction][]</span></span>    | <span data-ttu-id="efc08-130">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="efc08-130">An item was moved.</span></span>
| <span data-ttu-id="efc08-131">rename</span><span class="sxs-lookup"><span data-stu-id="efc08-131">rename</span></span>        | <span data-ttu-id="efc08-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-132">[renameAction][]</span></span>  | <span data-ttu-id="efc08-133">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="efc08-133">An item was renamed.</span></span>
| <span data-ttu-id="efc08-134">restore</span><span class="sxs-lookup"><span data-stu-id="efc08-134">restore</span></span>       | <span data-ttu-id="efc08-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-135">[restoreAction][]</span></span> | <span data-ttu-id="efc08-136">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="efc08-136">An item was restored.</span></span>
| <span data-ttu-id="efc08-137">share</span><span class="sxs-lookup"><span data-stu-id="efc08-137">share</span></span>         | <span data-ttu-id="efc08-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-138">[shareAction][]</span></span>   | <span data-ttu-id="efc08-139">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="efc08-139">An item was shared.</span></span>
| <span data-ttu-id="efc08-140">version</span><span class="sxs-lookup"><span data-stu-id="efc08-140">version</span></span>       | <span data-ttu-id="efc08-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="efc08-141">[versionAction][]</span></span> | <span data-ttu-id="efc08-142">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="efc08-142">An item was versioned.</span></span>

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="json-representation"></a><span data-ttu-id="efc08-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efc08-153">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
