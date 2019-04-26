---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
ms.openlocfilehash: b88f7514f7871e3c3850da91e4cd90b32f3a69c4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345404"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="83f8e-102">Tipo de recurso ItemActionSet</span><span class="sxs-lookup"><span data-stu-id="83f8e-102">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83f8e-103">O recurso **ItemActionSet** fornece informações sobre as ações que deram origem a uma [activity][itemActivity] em um item.</span><span class="sxs-lookup"><span data-stu-id="83f8e-103">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="83f8e-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83f8e-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="83f8e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83f8e-105">Properties</span></span>

<span data-ttu-id="83f8e-106">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="83f8e-106">Below are the actions that are available today.</span></span>
<span data-ttu-id="83f8e-107">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActionSet** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="83f8e-107">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="83f8e-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="83f8e-108">Property name</span></span> | <span data-ttu-id="83f8e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="83f8e-109">Type</span></span>              | <span data-ttu-id="83f8e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="83f8e-110">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="83f8e-111">comment</span><span class="sxs-lookup"><span data-stu-id="83f8e-111">comment</span></span>       | <span data-ttu-id="83f8e-112">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-112">[commentAction][]</span></span> | <span data-ttu-id="83f8e-113">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="83f8e-113">A comment was added to the item.</span></span>
| <span data-ttu-id="83f8e-114">create</span><span class="sxs-lookup"><span data-stu-id="83f8e-114">create</span></span>        | <span data-ttu-id="83f8e-115">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-115">[createAction][]</span></span>  | <span data-ttu-id="83f8e-116">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="83f8e-116">An item was created.</span></span>
| <span data-ttu-id="83f8e-117">delete</span><span class="sxs-lookup"><span data-stu-id="83f8e-117">delete</span></span>        | <span data-ttu-id="83f8e-118">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-118">[deleteAction][]</span></span>  | <span data-ttu-id="83f8e-119">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="83f8e-119">An item was deleted.</span></span>
| <span data-ttu-id="83f8e-120">edit</span><span class="sxs-lookup"><span data-stu-id="83f8e-120">edit</span></span>          | <span data-ttu-id="83f8e-121">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-121">[editAction][]</span></span>    | <span data-ttu-id="83f8e-122">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="83f8e-122">An item was edited.</span></span>
| <span data-ttu-id="83f8e-123">mention</span><span class="sxs-lookup"><span data-stu-id="83f8e-123">mention</span></span>       | <span data-ttu-id="83f8e-124">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-124">[mentionAction][]</span></span> | <span data-ttu-id="83f8e-125">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="83f8e-125">A user was mentioned in the item.</span></span>
| <span data-ttu-id="83f8e-126">move</span><span class="sxs-lookup"><span data-stu-id="83f8e-126">move</span></span>          | <span data-ttu-id="83f8e-127">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-127">[moveAction][]</span></span>    | <span data-ttu-id="83f8e-128">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="83f8e-128">An item was moved.</span></span>
| <span data-ttu-id="83f8e-129">rename</span><span class="sxs-lookup"><span data-stu-id="83f8e-129">rename</span></span>        | <span data-ttu-id="83f8e-130">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-130">[renameAction][]</span></span>  | <span data-ttu-id="83f8e-131">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="83f8e-131">An item was renamed.</span></span>
| <span data-ttu-id="83f8e-132">restore</span><span class="sxs-lookup"><span data-stu-id="83f8e-132">restore</span></span>       | <span data-ttu-id="83f8e-133">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-133">[restoreAction][]</span></span> | <span data-ttu-id="83f8e-134">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="83f8e-134">An item was restored.</span></span>
| <span data-ttu-id="83f8e-135">share</span><span class="sxs-lookup"><span data-stu-id="83f8e-135">share</span></span>         | <span data-ttu-id="83f8e-136">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-136">[shareAction][]</span></span>   | <span data-ttu-id="83f8e-137">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="83f8e-137">An item was shared.</span></span>
| <span data-ttu-id="83f8e-138">version</span><span class="sxs-lookup"><span data-stu-id="83f8e-138">version</span></span>       | <span data-ttu-id="83f8e-139">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="83f8e-139">[versionAction][]</span></span> | <span data-ttu-id="83f8e-140">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="83f8e-140">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="83f8e-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="83f8e-151">Remarks</span></span>

<span data-ttu-id="83f8e-152">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="83f8e-152">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
