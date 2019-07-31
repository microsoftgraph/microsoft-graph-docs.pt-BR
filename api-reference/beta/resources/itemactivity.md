---
author: daspek
description: O recurso ItemActivity fornece informações sobre atividades que ocorreram em um item ou dentro de um repositório.
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab96c3169a2d2dc37e6b94ab325866e93fa4d6c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967089"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="0efef-103">Tipo de recurso ItemActivity</span><span class="sxs-lookup"><span data-stu-id="0efef-103">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0efef-104">O recurso **ItemActivity** fornece informações sobre atividades que ocorreram em um item ou dentro de um repositório.</span><span class="sxs-lookup"><span data-stu-id="0efef-104">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="0efef-105">Disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="0efef-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0efef-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0efef-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0efef-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0efef-107">Properties</span></span>

| <span data-ttu-id="0efef-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0efef-108">Property</span></span> | <span data-ttu-id="0efef-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0efef-109">Type</span></span>                    | <span data-ttu-id="0efef-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0efef-110">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="0efef-111">id</span><span class="sxs-lookup"><span data-stu-id="0efef-111">id</span></span>       | <span data-ttu-id="0efef-112">string</span><span class="sxs-lookup"><span data-stu-id="0efef-112">string</span></span>                  | <span data-ttu-id="0efef-113">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="0efef-113">The unique identifier of the activity.</span></span> <span data-ttu-id="0efef-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0efef-114">Read-only.</span></span>
| <span data-ttu-id="0efef-115">Access</span><span class="sxs-lookup"><span data-stu-id="0efef-115">access</span></span>   | <span data-ttu-id="0efef-116">[accessaction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-116">[accessAction][]</span></span>        | <span data-ttu-id="0efef-117">Um item foi acessado.</span><span class="sxs-lookup"><span data-stu-id="0efef-117">An item was accessed.</span></span>
| <span data-ttu-id="0efef-118">action</span><span class="sxs-lookup"><span data-stu-id="0efef-118">action</span></span>   | <span data-ttu-id="0efef-119">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="0efef-119">[itemActionSet][]</span></span>       | <span data-ttu-id="0efef-120">Detalhes sobre a ação que ocorreu.</span><span class="sxs-lookup"><span data-stu-id="0efef-120">Details about the action that took place.</span></span> <span data-ttu-id="0efef-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0efef-121">Read-only.</span></span>
| <span data-ttu-id="0efef-122">actor</span><span class="sxs-lookup"><span data-stu-id="0efef-122">actor</span></span>    | <span data-ttu-id="0efef-123">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0efef-123">[identitySet][]</span></span>         | <span data-ttu-id="0efef-124">Identidade de quem executou a ação.</span><span class="sxs-lookup"><span data-stu-id="0efef-124">Identity of who performed the action.</span></span> <span data-ttu-id="0efef-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0efef-125">Read-only.</span></span>
| <span data-ttu-id="0efef-126">location</span><span class="sxs-lookup"><span data-stu-id="0efef-126">location</span></span> | <span data-ttu-id="0efef-127">[location][]</span><span class="sxs-lookup"><span data-stu-id="0efef-127">[location][]</span></span>            | <span data-ttu-id="0efef-128">Local físico em que a ação foi executada.</span><span class="sxs-lookup"><span data-stu-id="0efef-128">Physical location where the action was performed.</span></span> <span data-ttu-id="0efef-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0efef-129">Read-only.</span></span>
| <span data-ttu-id="0efef-130">times</span><span class="sxs-lookup"><span data-stu-id="0efef-130">times</span></span>    | <span data-ttu-id="0efef-131">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="0efef-131">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="0efef-132">Detalhes sobre quando ocorreu a atividade.</span><span class="sxs-lookup"><span data-stu-id="0efef-132">Details about when the activity took place.</span></span> <span data-ttu-id="0efef-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0efef-133">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="0efef-137">Relações</span><span class="sxs-lookup"><span data-stu-id="0efef-137">Relationships</span></span>

| <span data-ttu-id="0efef-138">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="0efef-138">Relationship name</span></span> | <span data-ttu-id="0efef-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="0efef-139">Type</span></span>          | <span data-ttu-id="0efef-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="0efef-140">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="0efef-141">driveItem</span><span class="sxs-lookup"><span data-stu-id="0efef-141">driveItem</span></span>         | <span data-ttu-id="0efef-142">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="0efef-142">[driveItem][]</span></span> | <span data-ttu-id="0efef-143">Expõe o **driveItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="0efef-143">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="0efef-144">listItem</span><span class="sxs-lookup"><span data-stu-id="0efef-144">listItem</span></span>          | <span data-ttu-id="0efef-145">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="0efef-145">[listItem][]</span></span>  | <span data-ttu-id="0efef-146">Expõe o **listItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="0efef-146">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="0efef-149">Ações</span><span class="sxs-lookup"><span data-stu-id="0efef-149">Actions</span></span>

<span data-ttu-id="0efef-150">As ações que ocorreram dentro de uma atividade são detalhadas na propriedade **action**.</span><span class="sxs-lookup"><span data-stu-id="0efef-150">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="0efef-151">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="0efef-151">Below are the actions that are available today.</span></span>
<span data-ttu-id="0efef-152">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActivity** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="0efef-152">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="0efef-153">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="0efef-153">Action name</span></span> | <span data-ttu-id="0efef-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="0efef-154">Type</span></span>              | <span data-ttu-id="0efef-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="0efef-155">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="0efef-156">comment</span><span class="sxs-lookup"><span data-stu-id="0efef-156">comment</span></span>     | <span data-ttu-id="0efef-157">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-157">[commentAction][]</span></span> | <span data-ttu-id="0efef-158">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="0efef-158">A comment was added to the item.</span></span>
| <span data-ttu-id="0efef-159">create</span><span class="sxs-lookup"><span data-stu-id="0efef-159">create</span></span>      | <span data-ttu-id="0efef-160">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-160">[createAction][]</span></span>  | <span data-ttu-id="0efef-161">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="0efef-161">An item was created.</span></span>
| <span data-ttu-id="0efef-162">delete</span><span class="sxs-lookup"><span data-stu-id="0efef-162">delete</span></span>      | <span data-ttu-id="0efef-163">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-163">[deleteAction][]</span></span>  | <span data-ttu-id="0efef-164">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="0efef-164">An item was deleted.</span></span>
| <span data-ttu-id="0efef-165">edit</span><span class="sxs-lookup"><span data-stu-id="0efef-165">edit</span></span>        | <span data-ttu-id="0efef-166">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-166">[editAction][]</span></span>    | <span data-ttu-id="0efef-167">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="0efef-167">An item was edited.</span></span>
| <span data-ttu-id="0efef-168">mention</span><span class="sxs-lookup"><span data-stu-id="0efef-168">mention</span></span>     | <span data-ttu-id="0efef-169">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-169">[mentionAction][]</span></span> | <span data-ttu-id="0efef-170">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="0efef-170">A user was mentioned in the item.</span></span>
| <span data-ttu-id="0efef-171">move</span><span class="sxs-lookup"><span data-stu-id="0efef-171">move</span></span>        | <span data-ttu-id="0efef-172">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-172">[moveAction][]</span></span>    | <span data-ttu-id="0efef-173">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="0efef-173">An item was moved.</span></span>
| <span data-ttu-id="0efef-174">rename</span><span class="sxs-lookup"><span data-stu-id="0efef-174">rename</span></span>      | <span data-ttu-id="0efef-175">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-175">[renameAction][]</span></span>  | <span data-ttu-id="0efef-176">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="0efef-176">An item was renamed.</span></span>
| <span data-ttu-id="0efef-177">restore</span><span class="sxs-lookup"><span data-stu-id="0efef-177">restore</span></span>     | <span data-ttu-id="0efef-178">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-178">[restoreAction][]</span></span> | <span data-ttu-id="0efef-179">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="0efef-179">An item was restored.</span></span>
| <span data-ttu-id="0efef-180">share</span><span class="sxs-lookup"><span data-stu-id="0efef-180">share</span></span>       | <span data-ttu-id="0efef-181">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-181">[shareAction][]</span></span>   | <span data-ttu-id="0efef-182">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="0efef-182">An item was shared.</span></span>
| <span data-ttu-id="0efef-183">version</span><span class="sxs-lookup"><span data-stu-id="0efef-183">version</span></span>     | <span data-ttu-id="0efef-184">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="0efef-184">[versionAction][]</span></span> | <span data-ttu-id="0efef-185">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="0efef-185">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="0efef-198">Comentários</span><span class="sxs-lookup"><span data-stu-id="0efef-198">Remarks</span></span>

<span data-ttu-id="0efef-199">**ItemActivity** está disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="0efef-199">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

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
