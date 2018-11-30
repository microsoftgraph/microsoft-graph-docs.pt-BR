---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
ms.openlocfilehash: 3b2f77ea21f2352b0a8fa647af84d9b0af08a2ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033454"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="340b8-102">Tipo de recurso ItemActionSet</span><span class="sxs-lookup"><span data-stu-id="340b8-102">ItemActionSet resource type</span></span>

> <span data-ttu-id="340b8-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="340b8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="340b8-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="340b8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="340b8-105">O recurso **ItemActionSet** fornece informações sobre as ações que deram origem a uma [activity][itemActivity] em um item.</span><span class="sxs-lookup"><span data-stu-id="340b8-105">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="340b8-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="340b8-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="340b8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="340b8-107">Properties</span></span>

<span data-ttu-id="340b8-108">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="340b8-108">Below are the actions that are available today.</span></span>
<span data-ttu-id="340b8-109">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActionSet** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="340b8-109">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="340b8-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="340b8-110">Property name</span></span> | <span data-ttu-id="340b8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="340b8-111">Type</span></span>              | <span data-ttu-id="340b8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="340b8-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="340b8-113">comment</span><span class="sxs-lookup"><span data-stu-id="340b8-113">comment</span></span>       | <span data-ttu-id="340b8-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-114">[commentAction][]</span></span> | <span data-ttu-id="340b8-115">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="340b8-115">A comment was added to the item.</span></span>
| <span data-ttu-id="340b8-116">create</span><span class="sxs-lookup"><span data-stu-id="340b8-116">create</span></span>        | <span data-ttu-id="340b8-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-117">[createAction][]</span></span>  | <span data-ttu-id="340b8-118">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="340b8-118">An item was created.</span></span>
| <span data-ttu-id="340b8-119">delete</span><span class="sxs-lookup"><span data-stu-id="340b8-119">delete</span></span>        | <span data-ttu-id="340b8-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-120">[deleteAction][]</span></span>  | <span data-ttu-id="340b8-121">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="340b8-121">An item was deleted.</span></span>
| <span data-ttu-id="340b8-122">edit</span><span class="sxs-lookup"><span data-stu-id="340b8-122">edit</span></span>          | <span data-ttu-id="340b8-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-123">[editAction][]</span></span>    | <span data-ttu-id="340b8-124">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="340b8-124">An item was edited.</span></span>
| <span data-ttu-id="340b8-125">mention</span><span class="sxs-lookup"><span data-stu-id="340b8-125">mention</span></span>       | <span data-ttu-id="340b8-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-126">[mentionAction][]</span></span> | <span data-ttu-id="340b8-127">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="340b8-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="340b8-128">move</span><span class="sxs-lookup"><span data-stu-id="340b8-128">move</span></span>          | <span data-ttu-id="340b8-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-129">[moveAction][]</span></span>    | <span data-ttu-id="340b8-130">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="340b8-130">An item was moved.</span></span>
| <span data-ttu-id="340b8-131">rename</span><span class="sxs-lookup"><span data-stu-id="340b8-131">rename</span></span>        | <span data-ttu-id="340b8-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-132">[renameAction][]</span></span>  | <span data-ttu-id="340b8-133">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="340b8-133">An item was renamed.</span></span>
| <span data-ttu-id="340b8-134">restore</span><span class="sxs-lookup"><span data-stu-id="340b8-134">restore</span></span>       | <span data-ttu-id="340b8-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-135">[restoreAction][]</span></span> | <span data-ttu-id="340b8-136">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="340b8-136">An item was restored.</span></span>
| <span data-ttu-id="340b8-137">share</span><span class="sxs-lookup"><span data-stu-id="340b8-137">share</span></span>         | <span data-ttu-id="340b8-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-138">[shareAction][]</span></span>   | <span data-ttu-id="340b8-139">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="340b8-139">An item was shared.</span></span>
| <span data-ttu-id="340b8-140">version</span><span class="sxs-lookup"><span data-stu-id="340b8-140">version</span></span>       | <span data-ttu-id="340b8-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="340b8-141">[versionAction][]</span></span> | <span data-ttu-id="340b8-142">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="340b8-142">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="340b8-153">Comentários</span><span class="sxs-lookup"><span data-stu-id="340b8-153">Remarks</span></span>

<span data-ttu-id="340b8-154">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="340b8-154">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
