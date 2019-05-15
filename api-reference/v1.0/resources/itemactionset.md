---
author: daspek
ms.author: dspektor
title: Tipo de recurso ItemActionSet
description: O objeto doactionset fornece informações sobre as ações que foram realizadas como parte de uma atividade em um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 065a6126e2e4a2f78cecfb2ae5497fac28e16899
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970599"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="340a7-103">tipo de recurso doactionset</span><span class="sxs-lookup"><span data-stu-id="340a7-103">itemActionSet resource type</span></span>

<span data-ttu-id="340a7-104">O \*\*\*\* recurso doactionset fornece informações sobre as ações que compõem uma [atividade] [ itemActivity] em um item.</span><span class="sxs-lookup"><span data-stu-id="340a7-104">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="340a7-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="340a7-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="340a7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="340a7-106">Properties</span></span>

<span data-ttu-id="340a7-107">As ações a seguir estão disponíveis no momento.</span><span class="sxs-lookup"><span data-stu-id="340a7-107">The following actions are currently available.</span></span> <span data-ttu-id="340a7-108">Como novas ações podem ser adicionadas no futuro, certifique-se de que seu aplicativo possa \*\*\*\* lidar com um ItemAdded que inclui ações desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="340a7-108">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="340a7-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="340a7-109">Property name</span></span> | <span data-ttu-id="340a7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="340a7-110">Type</span></span>              | <span data-ttu-id="340a7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="340a7-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="340a7-112">comment</span><span class="sxs-lookup"><span data-stu-id="340a7-112">comment</span></span>       | <span data-ttu-id="340a7-113">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-113">[commentAction][]</span></span> | <span data-ttu-id="340a7-114">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="340a7-114">A comment was added to the item.</span></span>
| <span data-ttu-id="340a7-115">create</span><span class="sxs-lookup"><span data-stu-id="340a7-115">create</span></span>        | <span data-ttu-id="340a7-116">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-116">[createAction][]</span></span>  | <span data-ttu-id="340a7-117">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="340a7-117">An item was created.</span></span>
| <span data-ttu-id="340a7-118">delete</span><span class="sxs-lookup"><span data-stu-id="340a7-118">delete</span></span>        | <span data-ttu-id="340a7-119">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-119">[deleteAction][]</span></span>  | <span data-ttu-id="340a7-120">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="340a7-120">An item was deleted.</span></span>
| <span data-ttu-id="340a7-121">edit</span><span class="sxs-lookup"><span data-stu-id="340a7-121">edit</span></span>          | <span data-ttu-id="340a7-122">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-122">[editAction][]</span></span>    | <span data-ttu-id="340a7-123">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="340a7-123">An item was edited.</span></span>
| <span data-ttu-id="340a7-124">mention</span><span class="sxs-lookup"><span data-stu-id="340a7-124">mention</span></span>       | <span data-ttu-id="340a7-125">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-125">[mentionAction][]</span></span> | <span data-ttu-id="340a7-126">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="340a7-126">A user was mentioned in the item.</span></span>
| <span data-ttu-id="340a7-127">move</span><span class="sxs-lookup"><span data-stu-id="340a7-127">move</span></span>          | <span data-ttu-id="340a7-128">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-128">[moveAction][]</span></span>    | <span data-ttu-id="340a7-129">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="340a7-129">An item was moved.</span></span>
| <span data-ttu-id="340a7-130">rename</span><span class="sxs-lookup"><span data-stu-id="340a7-130">rename</span></span>        | <span data-ttu-id="340a7-131">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-131">[renameAction][]</span></span>  | <span data-ttu-id="340a7-132">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="340a7-132">An item was renamed.</span></span>
| <span data-ttu-id="340a7-133">restore</span><span class="sxs-lookup"><span data-stu-id="340a7-133">restore</span></span>       | <span data-ttu-id="340a7-134">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-134">[restoreAction][]</span></span> | <span data-ttu-id="340a7-135">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="340a7-135">An item was restored.</span></span>
| <span data-ttu-id="340a7-136">share</span><span class="sxs-lookup"><span data-stu-id="340a7-136">share</span></span>         | <span data-ttu-id="340a7-137">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-137">[shareAction][]</span></span>   | <span data-ttu-id="340a7-138">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="340a7-138">An item was shared.</span></span>
| <span data-ttu-id="340a7-139">version</span><span class="sxs-lookup"><span data-stu-id="340a7-139">version</span></span>       | <span data-ttu-id="340a7-140">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="340a7-140">[versionAction][]</span></span> | <span data-ttu-id="340a7-141">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="340a7-141">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="340a7-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="340a7-152">JSON representation</span></span>

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
