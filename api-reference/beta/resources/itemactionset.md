---
author: daspek
description: O recurso doactionset fornece informações sobre as ações que fizeram uma [atividade] [item de @ atividade] em um item.
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 86a4713bbeb757fcb700af8f82d1718589f3f58c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075676"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="174a1-103">Tipo de recurso ItemActionSet</span><span class="sxs-lookup"><span data-stu-id="174a1-103">ItemActionSet resource type</span></span>

<span data-ttu-id="174a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="174a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="174a1-105">O recurso **ItemActionSet** fornece informações sobre as ações que deram origem a uma [activity][itemActivity] em um item.</span><span class="sxs-lookup"><span data-stu-id="174a1-105">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="174a1-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="174a1-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="174a1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="174a1-107">Properties</span></span>

<span data-ttu-id="174a1-108">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="174a1-108">Below are the actions that are available today.</span></span>
<span data-ttu-id="174a1-109">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActionSet** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="174a1-109">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="174a1-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="174a1-110">Property name</span></span> | <span data-ttu-id="174a1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="174a1-111">Type</span></span>              | <span data-ttu-id="174a1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="174a1-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="174a1-113">comment</span><span class="sxs-lookup"><span data-stu-id="174a1-113">comment</span></span>       | <span data-ttu-id="174a1-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-114">[commentAction][]</span></span> | <span data-ttu-id="174a1-115">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="174a1-115">A comment was added to the item.</span></span>
| <span data-ttu-id="174a1-116">create</span><span class="sxs-lookup"><span data-stu-id="174a1-116">create</span></span>        | <span data-ttu-id="174a1-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-117">[createAction][]</span></span>  | <span data-ttu-id="174a1-118">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="174a1-118">An item was created.</span></span>
| <span data-ttu-id="174a1-119">delete</span><span class="sxs-lookup"><span data-stu-id="174a1-119">delete</span></span>        | <span data-ttu-id="174a1-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-120">[deleteAction][]</span></span>  | <span data-ttu-id="174a1-121">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="174a1-121">An item was deleted.</span></span>
| <span data-ttu-id="174a1-122">edit</span><span class="sxs-lookup"><span data-stu-id="174a1-122">edit</span></span>          | <span data-ttu-id="174a1-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-123">[editAction][]</span></span>    | <span data-ttu-id="174a1-124">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="174a1-124">An item was edited.</span></span>
| <span data-ttu-id="174a1-125">mention</span><span class="sxs-lookup"><span data-stu-id="174a1-125">mention</span></span>       | <span data-ttu-id="174a1-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-126">[mentionAction][]</span></span> | <span data-ttu-id="174a1-127">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="174a1-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="174a1-128">move</span><span class="sxs-lookup"><span data-stu-id="174a1-128">move</span></span>          | <span data-ttu-id="174a1-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-129">[moveAction][]</span></span>    | <span data-ttu-id="174a1-130">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="174a1-130">An item was moved.</span></span>
| <span data-ttu-id="174a1-131">rename</span><span class="sxs-lookup"><span data-stu-id="174a1-131">rename</span></span>        | <span data-ttu-id="174a1-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-132">[renameAction][]</span></span>  | <span data-ttu-id="174a1-133">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="174a1-133">An item was renamed.</span></span>
| <span data-ttu-id="174a1-134">restore</span><span class="sxs-lookup"><span data-stu-id="174a1-134">restore</span></span>       | <span data-ttu-id="174a1-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-135">[restoreAction][]</span></span> | <span data-ttu-id="174a1-136">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="174a1-136">An item was restored.</span></span>
| <span data-ttu-id="174a1-137">share</span><span class="sxs-lookup"><span data-stu-id="174a1-137">share</span></span>         | <span data-ttu-id="174a1-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-138">[shareAction][]</span></span>   | <span data-ttu-id="174a1-139">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="174a1-139">An item was shared.</span></span>
| <span data-ttu-id="174a1-140">version</span><span class="sxs-lookup"><span data-stu-id="174a1-140">version</span></span>       | <span data-ttu-id="174a1-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="174a1-141">[versionAction][]</span></span> | <span data-ttu-id="174a1-142">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="174a1-142">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="174a1-153">Comentários</span><span class="sxs-lookup"><span data-stu-id="174a1-153">Remarks</span></span>

<span data-ttu-id="174a1-154">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="174a1-154">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


