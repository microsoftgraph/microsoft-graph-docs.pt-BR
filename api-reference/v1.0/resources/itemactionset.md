---
author: daspek
title: Tipo de recurso ItemActionSet
description: O objeto itemActionSet fornece informações sobre as ações que ocorreram como parte de uma atividade em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 6dcc630b76adcbec3c719a43280e4b28d1d933e5
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239251"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="4fe60-103">Tipo de recurso itemActionSet</span><span class="sxs-lookup"><span data-stu-id="4fe60-103">itemActionSet resource type</span></span>

<span data-ttu-id="4fe60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fe60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4fe60-105">O **recurso itemActionSet** fornece informações sobre as ações que comviam uma [atividade][itemActivity] em um item.</span><span class="sxs-lookup"><span data-stu-id="4fe60-105">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="4fe60-106">**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="4fe60-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="4fe60-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4fe60-107">Properties</span></span>

<span data-ttu-id="4fe60-108">As ações a seguir estão disponíveis no momento.</span><span class="sxs-lookup"><span data-stu-id="4fe60-108">The following actions are currently available.</span></span> <span data-ttu-id="4fe60-109">Como novas ações podem ser adicionadas no futuro, certifique-se de que seu aplicativo possa manipular um **itemActionSet** que inclui ações desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="4fe60-109">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="4fe60-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4fe60-110">Property name</span></span> | <span data-ttu-id="4fe60-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fe60-111">Type</span></span>              | <span data-ttu-id="4fe60-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fe60-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="4fe60-113">comment</span><span class="sxs-lookup"><span data-stu-id="4fe60-113">comment</span></span>       | <span data-ttu-id="4fe60-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-114">[commentAction][]</span></span> | <span data-ttu-id="4fe60-115">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="4fe60-115">A comment was added to the item.</span></span>
| <span data-ttu-id="4fe60-116">create</span><span class="sxs-lookup"><span data-stu-id="4fe60-116">create</span></span>        | <span data-ttu-id="4fe60-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-117">[createAction][]</span></span>  | <span data-ttu-id="4fe60-118">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="4fe60-118">An item was created.</span></span>
| <span data-ttu-id="4fe60-119">delete</span><span class="sxs-lookup"><span data-stu-id="4fe60-119">delete</span></span>        | <span data-ttu-id="4fe60-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-120">[deleteAction][]</span></span>  | <span data-ttu-id="4fe60-121">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="4fe60-121">An item was deleted.</span></span>
| <span data-ttu-id="4fe60-122">edit</span><span class="sxs-lookup"><span data-stu-id="4fe60-122">edit</span></span>          | <span data-ttu-id="4fe60-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-123">[editAction][]</span></span>    | <span data-ttu-id="4fe60-124">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="4fe60-124">An item was edited.</span></span>
| <span data-ttu-id="4fe60-125">mention</span><span class="sxs-lookup"><span data-stu-id="4fe60-125">mention</span></span>       | <span data-ttu-id="4fe60-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-126">[mentionAction][]</span></span> | <span data-ttu-id="4fe60-127">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="4fe60-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="4fe60-128">move</span><span class="sxs-lookup"><span data-stu-id="4fe60-128">move</span></span>          | <span data-ttu-id="4fe60-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-129">[moveAction][]</span></span>    | <span data-ttu-id="4fe60-130">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="4fe60-130">An item was moved.</span></span>
| <span data-ttu-id="4fe60-131">rename</span><span class="sxs-lookup"><span data-stu-id="4fe60-131">rename</span></span>        | <span data-ttu-id="4fe60-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-132">[renameAction][]</span></span>  | <span data-ttu-id="4fe60-133">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="4fe60-133">An item was renamed.</span></span>
| <span data-ttu-id="4fe60-134">restore</span><span class="sxs-lookup"><span data-stu-id="4fe60-134">restore</span></span>       | <span data-ttu-id="4fe60-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-135">[restoreAction][]</span></span> | <span data-ttu-id="4fe60-136">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="4fe60-136">An item was restored.</span></span>
| <span data-ttu-id="4fe60-137">share</span><span class="sxs-lookup"><span data-stu-id="4fe60-137">share</span></span>         | <span data-ttu-id="4fe60-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-138">[shareAction][]</span></span>   | <span data-ttu-id="4fe60-139">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4fe60-139">An item was shared.</span></span>
| <span data-ttu-id="4fe60-140">version</span><span class="sxs-lookup"><span data-stu-id="4fe60-140">version</span></span>       | <span data-ttu-id="4fe60-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="4fe60-141">[versionAction][]</span></span> | <span data-ttu-id="4fe60-142">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="4fe60-142">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="4fe60-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4fe60-153">JSON representation</span></span>

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

