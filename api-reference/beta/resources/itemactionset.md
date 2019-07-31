---
author: daspek
description: O recurso doactionset fornece informações sobre as ações que fizeram uma [atividade] [item de @ atividade] em um item.
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8053942fe96011b018e46681d69d308f65aa5d5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967144"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="6a7bf-103">Tipo de recurso ItemActionSet</span><span class="sxs-lookup"><span data-stu-id="6a7bf-103">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a7bf-104">O recurso **ItemActionSet** fornece informações sobre as ações que deram origem a uma [activity][itemActivity] em um item.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-104">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="6a7bf-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a7bf-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6a7bf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a7bf-106">Properties</span></span>

<span data-ttu-id="6a7bf-107">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-107">Below are the actions that are available today.</span></span>
<span data-ttu-id="6a7bf-108">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActionSet** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-108">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="6a7bf-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6a7bf-109">Property name</span></span> | <span data-ttu-id="6a7bf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a7bf-110">Type</span></span>              | <span data-ttu-id="6a7bf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a7bf-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="6a7bf-112">comment</span><span class="sxs-lookup"><span data-stu-id="6a7bf-112">comment</span></span>       | <span data-ttu-id="6a7bf-113">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-113">[commentAction][]</span></span> | <span data-ttu-id="6a7bf-114">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-114">A comment was added to the item.</span></span>
| <span data-ttu-id="6a7bf-115">create</span><span class="sxs-lookup"><span data-stu-id="6a7bf-115">create</span></span>        | <span data-ttu-id="6a7bf-116">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-116">[createAction][]</span></span>  | <span data-ttu-id="6a7bf-117">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-117">An item was created.</span></span>
| <span data-ttu-id="6a7bf-118">delete</span><span class="sxs-lookup"><span data-stu-id="6a7bf-118">delete</span></span>        | <span data-ttu-id="6a7bf-119">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-119">[deleteAction][]</span></span>  | <span data-ttu-id="6a7bf-120">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-120">An item was deleted.</span></span>
| <span data-ttu-id="6a7bf-121">edit</span><span class="sxs-lookup"><span data-stu-id="6a7bf-121">edit</span></span>          | <span data-ttu-id="6a7bf-122">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-122">[editAction][]</span></span>    | <span data-ttu-id="6a7bf-123">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-123">An item was edited.</span></span>
| <span data-ttu-id="6a7bf-124">mention</span><span class="sxs-lookup"><span data-stu-id="6a7bf-124">mention</span></span>       | <span data-ttu-id="6a7bf-125">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-125">[mentionAction][]</span></span> | <span data-ttu-id="6a7bf-126">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-126">A user was mentioned in the item.</span></span>
| <span data-ttu-id="6a7bf-127">move</span><span class="sxs-lookup"><span data-stu-id="6a7bf-127">move</span></span>          | <span data-ttu-id="6a7bf-128">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-128">[moveAction][]</span></span>    | <span data-ttu-id="6a7bf-129">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-129">An item was moved.</span></span>
| <span data-ttu-id="6a7bf-130">rename</span><span class="sxs-lookup"><span data-stu-id="6a7bf-130">rename</span></span>        | <span data-ttu-id="6a7bf-131">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-131">[renameAction][]</span></span>  | <span data-ttu-id="6a7bf-132">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-132">An item was renamed.</span></span>
| <span data-ttu-id="6a7bf-133">restore</span><span class="sxs-lookup"><span data-stu-id="6a7bf-133">restore</span></span>       | <span data-ttu-id="6a7bf-134">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-134">[restoreAction][]</span></span> | <span data-ttu-id="6a7bf-135">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-135">An item was restored.</span></span>
| <span data-ttu-id="6a7bf-136">share</span><span class="sxs-lookup"><span data-stu-id="6a7bf-136">share</span></span>         | <span data-ttu-id="6a7bf-137">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-137">[shareAction][]</span></span>   | <span data-ttu-id="6a7bf-138">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-138">An item was shared.</span></span>
| <span data-ttu-id="6a7bf-139">version</span><span class="sxs-lookup"><span data-stu-id="6a7bf-139">version</span></span>       | <span data-ttu-id="6a7bf-140">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="6a7bf-140">[versionAction][]</span></span> | <span data-ttu-id="6a7bf-141">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-141">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="6a7bf-152">Comentários</span><span class="sxs-lookup"><span data-stu-id="6a7bf-152">Remarks</span></span>

<span data-ttu-id="6a7bf-153">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="6a7bf-153">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
