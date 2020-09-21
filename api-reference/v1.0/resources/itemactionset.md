---
author: daspek
ms.author: dspektor
title: Tipo de recurso ItemActionSet
description: O objeto doactionset fornece informações sobre as ações que foram realizadas como parte de uma atividade em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9563f138c5074e1317927e8e9636eeba42beed35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967447"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="dcac0-103">tipo de recurso doactionset</span><span class="sxs-lookup"><span data-stu-id="dcac0-103">itemActionSet resource type</span></span>

<span data-ttu-id="dcac0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcac0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dcac0-105">O recurso **Doactionset** fornece informações sobre as ações que compõem uma [atividade][itemActivity] em um item.</span><span class="sxs-lookup"><span data-stu-id="dcac0-105">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="dcac0-106">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="dcac0-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="dcac0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dcac0-107">Properties</span></span>

<span data-ttu-id="dcac0-108">As ações a seguir estão disponíveis no momento.</span><span class="sxs-lookup"><span data-stu-id="dcac0-108">The following actions are currently available.</span></span> <span data-ttu-id="dcac0-109">Como novas ações podem ser adicionadas no futuro, certifique-se de que seu aplicativo possa lidar **com um ItemAdded** que inclui ações desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="dcac0-109">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="dcac0-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="dcac0-110">Property name</span></span> | <span data-ttu-id="dcac0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcac0-111">Type</span></span>              | <span data-ttu-id="dcac0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcac0-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="dcac0-113">comment</span><span class="sxs-lookup"><span data-stu-id="dcac0-113">comment</span></span>       | <span data-ttu-id="dcac0-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-114">[commentAction][]</span></span> | <span data-ttu-id="dcac0-115">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="dcac0-115">A comment was added to the item.</span></span>
| <span data-ttu-id="dcac0-116">create</span><span class="sxs-lookup"><span data-stu-id="dcac0-116">create</span></span>        | <span data-ttu-id="dcac0-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-117">[createAction][]</span></span>  | <span data-ttu-id="dcac0-118">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="dcac0-118">An item was created.</span></span>
| <span data-ttu-id="dcac0-119">delete</span><span class="sxs-lookup"><span data-stu-id="dcac0-119">delete</span></span>        | <span data-ttu-id="dcac0-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-120">[deleteAction][]</span></span>  | <span data-ttu-id="dcac0-121">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="dcac0-121">An item was deleted.</span></span>
| <span data-ttu-id="dcac0-122">edit</span><span class="sxs-lookup"><span data-stu-id="dcac0-122">edit</span></span>          | <span data-ttu-id="dcac0-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-123">[editAction][]</span></span>    | <span data-ttu-id="dcac0-124">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="dcac0-124">An item was edited.</span></span>
| <span data-ttu-id="dcac0-125">mention</span><span class="sxs-lookup"><span data-stu-id="dcac0-125">mention</span></span>       | <span data-ttu-id="dcac0-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-126">[mentionAction][]</span></span> | <span data-ttu-id="dcac0-127">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="dcac0-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="dcac0-128">move</span><span class="sxs-lookup"><span data-stu-id="dcac0-128">move</span></span>          | <span data-ttu-id="dcac0-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-129">[moveAction][]</span></span>    | <span data-ttu-id="dcac0-130">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="dcac0-130">An item was moved.</span></span>
| <span data-ttu-id="dcac0-131">rename</span><span class="sxs-lookup"><span data-stu-id="dcac0-131">rename</span></span>        | <span data-ttu-id="dcac0-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-132">[renameAction][]</span></span>  | <span data-ttu-id="dcac0-133">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="dcac0-133">An item was renamed.</span></span>
| <span data-ttu-id="dcac0-134">restore</span><span class="sxs-lookup"><span data-stu-id="dcac0-134">restore</span></span>       | <span data-ttu-id="dcac0-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-135">[restoreAction][]</span></span> | <span data-ttu-id="dcac0-136">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="dcac0-136">An item was restored.</span></span>
| <span data-ttu-id="dcac0-137">share</span><span class="sxs-lookup"><span data-stu-id="dcac0-137">share</span></span>         | <span data-ttu-id="dcac0-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-138">[shareAction][]</span></span>   | <span data-ttu-id="dcac0-139">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="dcac0-139">An item was shared.</span></span>
| <span data-ttu-id="dcac0-140">version</span><span class="sxs-lookup"><span data-stu-id="dcac0-140">version</span></span>       | <span data-ttu-id="dcac0-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="dcac0-141">[versionAction][]</span></span> | <span data-ttu-id="dcac0-142">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="dcac0-142">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="dcac0-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dcac0-153">JSON representation</span></span>

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

