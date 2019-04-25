---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
ms.openlocfilehash: 5e2be549c3e3e9e799449679b605577ecd782a94
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561884"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="20074-102">Tipo de recurso ItemActivity</span><span class="sxs-lookup"><span data-stu-id="20074-102">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20074-103">O recurso **ItemActivity** fornece informações sobre atividades que ocorreram em um item ou dentro de um repositório.</span><span class="sxs-lookup"><span data-stu-id="20074-103">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="20074-104">Disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="20074-104">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="20074-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20074-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="20074-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20074-106">Properties</span></span>

| <span data-ttu-id="20074-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20074-107">Property</span></span> | <span data-ttu-id="20074-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="20074-108">Type</span></span>                    | <span data-ttu-id="20074-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="20074-109">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="20074-110">id</span><span class="sxs-lookup"><span data-stu-id="20074-110">id</span></span>       | <span data-ttu-id="20074-111">string</span><span class="sxs-lookup"><span data-stu-id="20074-111">string</span></span>                  | <span data-ttu-id="20074-112">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="20074-112">The unique identifier of the activity.</span></span> <span data-ttu-id="20074-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20074-113">Read-only.</span></span>
| <span data-ttu-id="20074-114">Access</span><span class="sxs-lookup"><span data-stu-id="20074-114">access</span></span>   | <span data-ttu-id="20074-115">[accessaction][]</span><span class="sxs-lookup"><span data-stu-id="20074-115">[accessAction][]</span></span>        | <span data-ttu-id="20074-116">Um item foi acessado.</span><span class="sxs-lookup"><span data-stu-id="20074-116">An item was accessed.</span></span>
| <span data-ttu-id="20074-117">action</span><span class="sxs-lookup"><span data-stu-id="20074-117">action</span></span>   | <span data-ttu-id="20074-118">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="20074-118">[itemActionSet][]</span></span>       | <span data-ttu-id="20074-119">Detalhes sobre a ação que ocorreu.</span><span class="sxs-lookup"><span data-stu-id="20074-119">Details about the action that took place.</span></span> <span data-ttu-id="20074-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20074-120">Read-only.</span></span>
| <span data-ttu-id="20074-121">actor</span><span class="sxs-lookup"><span data-stu-id="20074-121">actor</span></span>    | <span data-ttu-id="20074-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="20074-122">[identitySet][]</span></span>         | <span data-ttu-id="20074-123">Identidade de quem executou a ação.</span><span class="sxs-lookup"><span data-stu-id="20074-123">Identity of who performed the action.</span></span> <span data-ttu-id="20074-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20074-124">Read-only.</span></span>
| <span data-ttu-id="20074-125">location</span><span class="sxs-lookup"><span data-stu-id="20074-125">location</span></span> | <span data-ttu-id="20074-126">[location][]</span><span class="sxs-lookup"><span data-stu-id="20074-126">[location][]</span></span>            | <span data-ttu-id="20074-127">Local físico em que a ação foi executada.</span><span class="sxs-lookup"><span data-stu-id="20074-127">Physical location where the action was performed.</span></span> <span data-ttu-id="20074-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20074-128">Read-only.</span></span>
| <span data-ttu-id="20074-129">times</span><span class="sxs-lookup"><span data-stu-id="20074-129">times</span></span>    | <span data-ttu-id="20074-130">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="20074-130">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="20074-131">Detalhes sobre quando ocorreu a atividade.</span><span class="sxs-lookup"><span data-stu-id="20074-131">Details about when the activity took place.</span></span> <span data-ttu-id="20074-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20074-132">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="20074-136">Relações</span><span class="sxs-lookup"><span data-stu-id="20074-136">Relationships</span></span>

| <span data-ttu-id="20074-137">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="20074-137">Relationship name</span></span> | <span data-ttu-id="20074-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="20074-138">Type</span></span>          | <span data-ttu-id="20074-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="20074-139">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="20074-140">driveItem</span><span class="sxs-lookup"><span data-stu-id="20074-140">driveItem</span></span>         | <span data-ttu-id="20074-141">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="20074-141">[driveItem][]</span></span> | <span data-ttu-id="20074-142">Expõe o **driveItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="20074-142">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="20074-143">listItem</span><span class="sxs-lookup"><span data-stu-id="20074-143">listItem</span></span>          | <span data-ttu-id="20074-144">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="20074-144">[listItem][]</span></span>  | <span data-ttu-id="20074-145">Expõe o **listItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="20074-145">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="20074-148">Ações</span><span class="sxs-lookup"><span data-stu-id="20074-148">Actions</span></span>

<span data-ttu-id="20074-149">As ações que ocorreram dentro de uma atividade são detalhadas na propriedade **action**.</span><span class="sxs-lookup"><span data-stu-id="20074-149">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="20074-150">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="20074-150">Below are the actions that are available today.</span></span>
<span data-ttu-id="20074-151">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActivity** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="20074-151">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="20074-152">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="20074-152">Action name</span></span> | <span data-ttu-id="20074-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="20074-153">Type</span></span>              | <span data-ttu-id="20074-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="20074-154">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="20074-155">comment</span><span class="sxs-lookup"><span data-stu-id="20074-155">comment</span></span>     | <span data-ttu-id="20074-156">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-156">[commentAction][]</span></span> | <span data-ttu-id="20074-157">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="20074-157">A comment was added to the item.</span></span>
| <span data-ttu-id="20074-158">create</span><span class="sxs-lookup"><span data-stu-id="20074-158">create</span></span>      | <span data-ttu-id="20074-159">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-159">[createAction][]</span></span>  | <span data-ttu-id="20074-160">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="20074-160">An item was created.</span></span>
| <span data-ttu-id="20074-161">delete</span><span class="sxs-lookup"><span data-stu-id="20074-161">delete</span></span>      | <span data-ttu-id="20074-162">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-162">[deleteAction][]</span></span>  | <span data-ttu-id="20074-163">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="20074-163">An item was deleted.</span></span>
| <span data-ttu-id="20074-164">edit</span><span class="sxs-lookup"><span data-stu-id="20074-164">edit</span></span>        | <span data-ttu-id="20074-165">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-165">[editAction][]</span></span>    | <span data-ttu-id="20074-166">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="20074-166">An item was edited.</span></span>
| <span data-ttu-id="20074-167">mention</span><span class="sxs-lookup"><span data-stu-id="20074-167">mention</span></span>     | <span data-ttu-id="20074-168">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-168">[mentionAction][]</span></span> | <span data-ttu-id="20074-169">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="20074-169">A user was mentioned in the item.</span></span>
| <span data-ttu-id="20074-170">move</span><span class="sxs-lookup"><span data-stu-id="20074-170">move</span></span>        | <span data-ttu-id="20074-171">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-171">[moveAction][]</span></span>    | <span data-ttu-id="20074-172">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="20074-172">An item was moved.</span></span>
| <span data-ttu-id="20074-173">rename</span><span class="sxs-lookup"><span data-stu-id="20074-173">rename</span></span>      | <span data-ttu-id="20074-174">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-174">[renameAction][]</span></span>  | <span data-ttu-id="20074-175">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="20074-175">An item was renamed.</span></span>
| <span data-ttu-id="20074-176">restore</span><span class="sxs-lookup"><span data-stu-id="20074-176">restore</span></span>     | <span data-ttu-id="20074-177">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-177">[restoreAction][]</span></span> | <span data-ttu-id="20074-178">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="20074-178">An item was restored.</span></span>
| <span data-ttu-id="20074-179">share</span><span class="sxs-lookup"><span data-stu-id="20074-179">share</span></span>       | <span data-ttu-id="20074-180">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-180">[shareAction][]</span></span>   | <span data-ttu-id="20074-181">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="20074-181">An item was shared.</span></span>
| <span data-ttu-id="20074-182">version</span><span class="sxs-lookup"><span data-stu-id="20074-182">version</span></span>     | <span data-ttu-id="20074-183">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="20074-183">[versionAction][]</span></span> | <span data-ttu-id="20074-184">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="20074-184">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="20074-197">Comentários</span><span class="sxs-lookup"><span data-stu-id="20074-197">Remarks</span></span>

<span data-ttu-id="20074-198">**ItemActivity** está disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="20074-198">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
