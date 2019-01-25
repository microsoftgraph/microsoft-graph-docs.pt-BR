---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
ms.openlocfilehash: 3fab75c6a63630f57dae8d0578691ba10622231d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518797"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="57af7-102">Tipo de recurso ItemActionSet</span><span class="sxs-lookup"><span data-stu-id="57af7-102">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57af7-103">O recurso **ItemActionSet** fornece informações sobre as ações que deram origem a uma [activity][itemActivity] em um item.</span><span class="sxs-lookup"><span data-stu-id="57af7-103">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="57af7-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57af7-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="57af7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57af7-105">Properties</span></span>

<span data-ttu-id="57af7-106">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="57af7-106">Below are the actions that are available today.</span></span>
<span data-ttu-id="57af7-107">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActionSet** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="57af7-107">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="57af7-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="57af7-108">Property name</span></span> | <span data-ttu-id="57af7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="57af7-109">Type</span></span>              | <span data-ttu-id="57af7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="57af7-110">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="57af7-111">comment</span><span class="sxs-lookup"><span data-stu-id="57af7-111">comment</span></span>       | <span data-ttu-id="57af7-112">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-112">[commentAction][]</span></span> | <span data-ttu-id="57af7-113">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="57af7-113">A comment was added to the item.</span></span>
| <span data-ttu-id="57af7-114">create</span><span class="sxs-lookup"><span data-stu-id="57af7-114">create</span></span>        | <span data-ttu-id="57af7-115">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-115">[createAction][]</span></span>  | <span data-ttu-id="57af7-116">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="57af7-116">An item was created.</span></span>
| <span data-ttu-id="57af7-117">delete</span><span class="sxs-lookup"><span data-stu-id="57af7-117">delete</span></span>        | <span data-ttu-id="57af7-118">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-118">[deleteAction][]</span></span>  | <span data-ttu-id="57af7-119">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="57af7-119">An item was deleted.</span></span>
| <span data-ttu-id="57af7-120">edit</span><span class="sxs-lookup"><span data-stu-id="57af7-120">edit</span></span>          | <span data-ttu-id="57af7-121">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-121">[editAction][]</span></span>    | <span data-ttu-id="57af7-122">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="57af7-122">An item was edited.</span></span>
| <span data-ttu-id="57af7-123">mention</span><span class="sxs-lookup"><span data-stu-id="57af7-123">mention</span></span>       | <span data-ttu-id="57af7-124">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-124">[mentionAction][]</span></span> | <span data-ttu-id="57af7-125">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="57af7-125">A user was mentioned in the item.</span></span>
| <span data-ttu-id="57af7-126">move</span><span class="sxs-lookup"><span data-stu-id="57af7-126">move</span></span>          | <span data-ttu-id="57af7-127">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-127">[moveAction][]</span></span>    | <span data-ttu-id="57af7-128">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="57af7-128">An item was moved.</span></span>
| <span data-ttu-id="57af7-129">rename</span><span class="sxs-lookup"><span data-stu-id="57af7-129">rename</span></span>        | <span data-ttu-id="57af7-130">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-130">[renameAction][]</span></span>  | <span data-ttu-id="57af7-131">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="57af7-131">An item was renamed.</span></span>
| <span data-ttu-id="57af7-132">restore</span><span class="sxs-lookup"><span data-stu-id="57af7-132">restore</span></span>       | <span data-ttu-id="57af7-133">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-133">[restoreAction][]</span></span> | <span data-ttu-id="57af7-134">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="57af7-134">An item was restored.</span></span>
| <span data-ttu-id="57af7-135">share</span><span class="sxs-lookup"><span data-stu-id="57af7-135">share</span></span>         | <span data-ttu-id="57af7-136">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-136">[shareAction][]</span></span>   | <span data-ttu-id="57af7-137">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="57af7-137">An item was shared.</span></span>
| <span data-ttu-id="57af7-138">version</span><span class="sxs-lookup"><span data-stu-id="57af7-138">version</span></span>       | <span data-ttu-id="57af7-139">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="57af7-139">[versionAction][]</span></span> | <span data-ttu-id="57af7-140">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="57af7-140">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="57af7-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="57af7-151">Remarks</span></span>

<span data-ttu-id="57af7-152">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="57af7-152">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactionset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
