---
author: daspek
description: O recurso ItemActivity fornece informações sobre atividades que ocorreram em um item ou dentro de um repositório.
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4cac403e44abaf9ae69f78005555772b9979046f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523118"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="b2a32-103">Tipo de recurso ItemActivity</span><span class="sxs-lookup"><span data-stu-id="b2a32-103">ItemActivity resource type</span></span>

<span data-ttu-id="b2a32-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b2a32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2a32-105">O recurso **ItemActivity** fornece informações sobre atividades que ocorreram em um item ou dentro de um repositório.</span><span class="sxs-lookup"><span data-stu-id="b2a32-105">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="b2a32-106">Disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b2a32-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2a32-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2a32-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a><span data-ttu-id="b2a32-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2a32-108">Properties</span></span>

| <span data-ttu-id="b2a32-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2a32-109">Property</span></span> | <span data-ttu-id="b2a32-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2a32-110">Type</span></span>                    | <span data-ttu-id="b2a32-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2a32-111">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="b2a32-112">id</span><span class="sxs-lookup"><span data-stu-id="b2a32-112">id</span></span>       | <span data-ttu-id="b2a32-113">string</span><span class="sxs-lookup"><span data-stu-id="b2a32-113">string</span></span>                  | <span data-ttu-id="b2a32-114">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="b2a32-114">The unique identifier of the activity.</span></span> <span data-ttu-id="b2a32-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2a32-115">Read-only.</span></span>
| <span data-ttu-id="b2a32-116">Access</span><span class="sxs-lookup"><span data-stu-id="b2a32-116">access</span></span>   | <span data-ttu-id="b2a32-117">[accessaction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-117">[accessAction][]</span></span>        | <span data-ttu-id="b2a32-118">Um item foi acessado.</span><span class="sxs-lookup"><span data-stu-id="b2a32-118">An item was accessed.</span></span>
| <span data-ttu-id="b2a32-119">action</span><span class="sxs-lookup"><span data-stu-id="b2a32-119">action</span></span>   | <span data-ttu-id="b2a32-120">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-120">[itemActionSet][]</span></span>       | <span data-ttu-id="b2a32-121">Detalhes sobre a ação que ocorreu.</span><span class="sxs-lookup"><span data-stu-id="b2a32-121">Details about the action that took place.</span></span> <span data-ttu-id="b2a32-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2a32-122">Read-only.</span></span>
| <span data-ttu-id="b2a32-123">actor</span><span class="sxs-lookup"><span data-stu-id="b2a32-123">actor</span></span>    | <span data-ttu-id="b2a32-124">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-124">[identitySet][]</span></span>         | <span data-ttu-id="b2a32-125">Identidade de quem executou a ação.</span><span class="sxs-lookup"><span data-stu-id="b2a32-125">Identity of who performed the action.</span></span> <span data-ttu-id="b2a32-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2a32-126">Read-only.</span></span>
| <span data-ttu-id="b2a32-127">location</span><span class="sxs-lookup"><span data-stu-id="b2a32-127">location</span></span> | <span data-ttu-id="b2a32-128">[location][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-128">[location][]</span></span>            | <span data-ttu-id="b2a32-129">Local físico em que a ação foi executada.</span><span class="sxs-lookup"><span data-stu-id="b2a32-129">Physical location where the action was performed.</span></span> <span data-ttu-id="b2a32-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2a32-130">Read-only.</span></span>
| <span data-ttu-id="b2a32-131">times</span><span class="sxs-lookup"><span data-stu-id="b2a32-131">times</span></span>    | <span data-ttu-id="b2a32-132">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-132">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="b2a32-133">Detalhes sobre quando ocorreu a atividade.</span><span class="sxs-lookup"><span data-stu-id="b2a32-133">Details about when the activity took place.</span></span> <span data-ttu-id="b2a32-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2a32-134">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="b2a32-138">Relações</span><span class="sxs-lookup"><span data-stu-id="b2a32-138">Relationships</span></span>

| <span data-ttu-id="b2a32-139">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="b2a32-139">Relationship name</span></span> | <span data-ttu-id="b2a32-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2a32-140">Type</span></span>          | <span data-ttu-id="b2a32-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2a32-141">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="b2a32-142">driveItem</span><span class="sxs-lookup"><span data-stu-id="b2a32-142">driveItem</span></span>         | <span data-ttu-id="b2a32-143">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-143">[driveItem][]</span></span> | <span data-ttu-id="b2a32-144">Expõe o **driveItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="b2a32-144">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="b2a32-145">listItem</span><span class="sxs-lookup"><span data-stu-id="b2a32-145">listItem</span></span>          | <span data-ttu-id="b2a32-146">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-146">[listItem][]</span></span>  | <span data-ttu-id="b2a32-147">Expõe o **listItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="b2a32-147">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="b2a32-150">Ações</span><span class="sxs-lookup"><span data-stu-id="b2a32-150">Actions</span></span>

<span data-ttu-id="b2a32-151">As ações que ocorreram dentro de uma atividade são detalhadas na propriedade **action**.</span><span class="sxs-lookup"><span data-stu-id="b2a32-151">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="b2a32-152">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="b2a32-152">Below are the actions that are available today.</span></span>
<span data-ttu-id="b2a32-153">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActivity** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="b2a32-153">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="b2a32-154">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="b2a32-154">Action name</span></span> | <span data-ttu-id="b2a32-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2a32-155">Type</span></span>              | <span data-ttu-id="b2a32-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2a32-156">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="b2a32-157">comment</span><span class="sxs-lookup"><span data-stu-id="b2a32-157">comment</span></span>     | <span data-ttu-id="b2a32-158">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-158">[commentAction][]</span></span> | <span data-ttu-id="b2a32-159">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="b2a32-159">A comment was added to the item.</span></span>
| <span data-ttu-id="b2a32-160">create</span><span class="sxs-lookup"><span data-stu-id="b2a32-160">create</span></span>      | <span data-ttu-id="b2a32-161">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-161">[createAction][]</span></span>  | <span data-ttu-id="b2a32-162">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="b2a32-162">An item was created.</span></span>
| <span data-ttu-id="b2a32-163">delete</span><span class="sxs-lookup"><span data-stu-id="b2a32-163">delete</span></span>      | <span data-ttu-id="b2a32-164">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-164">[deleteAction][]</span></span>  | <span data-ttu-id="b2a32-165">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="b2a32-165">An item was deleted.</span></span>
| <span data-ttu-id="b2a32-166">edit</span><span class="sxs-lookup"><span data-stu-id="b2a32-166">edit</span></span>        | <span data-ttu-id="b2a32-167">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-167">[editAction][]</span></span>    | <span data-ttu-id="b2a32-168">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="b2a32-168">An item was edited.</span></span>
| <span data-ttu-id="b2a32-169">mention</span><span class="sxs-lookup"><span data-stu-id="b2a32-169">mention</span></span>     | <span data-ttu-id="b2a32-170">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-170">[mentionAction][]</span></span> | <span data-ttu-id="b2a32-171">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="b2a32-171">A user was mentioned in the item.</span></span>
| <span data-ttu-id="b2a32-172">move</span><span class="sxs-lookup"><span data-stu-id="b2a32-172">move</span></span>        | <span data-ttu-id="b2a32-173">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-173">[moveAction][]</span></span>    | <span data-ttu-id="b2a32-174">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="b2a32-174">An item was moved.</span></span>
| <span data-ttu-id="b2a32-175">rename</span><span class="sxs-lookup"><span data-stu-id="b2a32-175">rename</span></span>      | <span data-ttu-id="b2a32-176">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-176">[renameAction][]</span></span>  | <span data-ttu-id="b2a32-177">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="b2a32-177">An item was renamed.</span></span>
| <span data-ttu-id="b2a32-178">restore</span><span class="sxs-lookup"><span data-stu-id="b2a32-178">restore</span></span>     | <span data-ttu-id="b2a32-179">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-179">[restoreAction][]</span></span> | <span data-ttu-id="b2a32-180">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="b2a32-180">An item was restored.</span></span>
| <span data-ttu-id="b2a32-181">share</span><span class="sxs-lookup"><span data-stu-id="b2a32-181">share</span></span>       | <span data-ttu-id="b2a32-182">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-182">[shareAction][]</span></span>   | <span data-ttu-id="b2a32-183">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b2a32-183">An item was shared.</span></span>
| <span data-ttu-id="b2a32-184">version</span><span class="sxs-lookup"><span data-stu-id="b2a32-184">version</span></span>     | <span data-ttu-id="b2a32-185">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="b2a32-185">[versionAction][]</span></span> | <span data-ttu-id="b2a32-186">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="b2a32-186">An item was versioned.</span></span>

[accessaction]: accessaction.md
[accessAction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a><span data-ttu-id="b2a32-199">Comentários</span><span class="sxs-lookup"><span data-stu-id="b2a32-199">Remarks</span></span>

<span data-ttu-id="b2a32-200">**ItemActivity** está disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b2a32-200">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": []
}
-->
