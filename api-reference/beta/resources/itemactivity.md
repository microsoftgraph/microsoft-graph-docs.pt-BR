---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
ms.openlocfilehash: 7c8cdab7adc705333d1aeaad526aeeb813de10a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039497"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="3727f-102">Tipo de recurso ItemActivity</span><span class="sxs-lookup"><span data-stu-id="3727f-102">ItemActivity resource type</span></span>

> <span data-ttu-id="3727f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3727f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3727f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3727f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3727f-105">O recurso **ItemActivity** fornece informações sobre atividades que ocorreram em um item ou dentro de um repositório.</span><span class="sxs-lookup"><span data-stu-id="3727f-105">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="3727f-106">Disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="3727f-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3727f-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3727f-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3727f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3727f-108">Properties</span></span>

| <span data-ttu-id="3727f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3727f-109">Property</span></span> | <span data-ttu-id="3727f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3727f-110">Type</span></span>                    | <span data-ttu-id="3727f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3727f-111">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="3727f-112">id</span><span class="sxs-lookup"><span data-stu-id="3727f-112">id</span></span>       | <span data-ttu-id="3727f-113">string</span><span class="sxs-lookup"><span data-stu-id="3727f-113">string</span></span>                  | <span data-ttu-id="3727f-114">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="3727f-114">The unique identifier of the activity.</span></span> <span data-ttu-id="3727f-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3727f-115">Read-only.</span></span>
| <span data-ttu-id="3727f-116">acesso</span><span class="sxs-lookup"><span data-stu-id="3727f-116">access</span></span>   | <span data-ttu-id="3727f-117">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-117">[accessAction][]</span></span>        | <span data-ttu-id="3727f-118">Um item foi acessado.</span><span class="sxs-lookup"><span data-stu-id="3727f-118">An item was accessed.</span></span>
| <span data-ttu-id="3727f-119">action</span><span class="sxs-lookup"><span data-stu-id="3727f-119">action</span></span>   | <span data-ttu-id="3727f-120">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="3727f-120">[itemActionSet][]</span></span>       | <span data-ttu-id="3727f-121">Detalhes sobre a ação que ocorreu.</span><span class="sxs-lookup"><span data-stu-id="3727f-121">Details about the action that took place.</span></span> <span data-ttu-id="3727f-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3727f-122">Read-only.</span></span>
| <span data-ttu-id="3727f-123">actor</span><span class="sxs-lookup"><span data-stu-id="3727f-123">actor</span></span>    | <span data-ttu-id="3727f-124">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3727f-124">[identitySet][]</span></span>         | <span data-ttu-id="3727f-125">Identidade de quem executou a ação.</span><span class="sxs-lookup"><span data-stu-id="3727f-125">Identity of who performed the action.</span></span> <span data-ttu-id="3727f-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3727f-126">Read-only.</span></span>
| <span data-ttu-id="3727f-127">location</span><span class="sxs-lookup"><span data-stu-id="3727f-127">location</span></span> | <span data-ttu-id="3727f-128">[location][]</span><span class="sxs-lookup"><span data-stu-id="3727f-128">[location][]</span></span>            | <span data-ttu-id="3727f-129">Local físico onde a ação foi realizada.</span><span class="sxs-lookup"><span data-stu-id="3727f-129">Physical location where the action was performed.</span></span> <span data-ttu-id="3727f-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3727f-130">Read-only.</span></span>
| <span data-ttu-id="3727f-131">times</span><span class="sxs-lookup"><span data-stu-id="3727f-131">times</span></span>    | <span data-ttu-id="3727f-132">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="3727f-132">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="3727f-133">Detalhes sobre quando ocorreu a atividade.</span><span class="sxs-lookup"><span data-stu-id="3727f-133">Details about when the activity took place.</span></span> <span data-ttu-id="3727f-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3727f-134">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="3727f-138">Relações</span><span class="sxs-lookup"><span data-stu-id="3727f-138">Relationships</span></span>

| <span data-ttu-id="3727f-139">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="3727f-139">Relationship name</span></span> | <span data-ttu-id="3727f-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="3727f-140">Type</span></span>          | <span data-ttu-id="3727f-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="3727f-141">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="3727f-142">driveItem</span><span class="sxs-lookup"><span data-stu-id="3727f-142">driveItem</span></span>         | <span data-ttu-id="3727f-143">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="3727f-143">[driveItem][]</span></span> | <span data-ttu-id="3727f-144">Expõe o **driveItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="3727f-144">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="3727f-145">listItem</span><span class="sxs-lookup"><span data-stu-id="3727f-145">listItem</span></span>          | <span data-ttu-id="3727f-146">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="3727f-146">[listItem][]</span></span>  | <span data-ttu-id="3727f-147">Expõe o **listItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="3727f-147">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="3727f-150">Ações</span><span class="sxs-lookup"><span data-stu-id="3727f-150">Actions</span></span>

<span data-ttu-id="3727f-151">As ações que ocorreram dentro de uma atividade são detalhadas na propriedade **action**.</span><span class="sxs-lookup"><span data-stu-id="3727f-151">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="3727f-152">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="3727f-152">Below are the actions that are available today.</span></span>
<span data-ttu-id="3727f-153">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActivity** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="3727f-153">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="3727f-154">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="3727f-154">Action name</span></span> | <span data-ttu-id="3727f-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="3727f-155">Type</span></span>              | <span data-ttu-id="3727f-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="3727f-156">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="3727f-157">comment</span><span class="sxs-lookup"><span data-stu-id="3727f-157">comment</span></span>     | <span data-ttu-id="3727f-158">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-158">[commentAction][]</span></span> | <span data-ttu-id="3727f-159">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="3727f-159">A comment was added to the item.</span></span>
| <span data-ttu-id="3727f-160">create</span><span class="sxs-lookup"><span data-stu-id="3727f-160">create</span></span>      | <span data-ttu-id="3727f-161">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-161">[createAction][]</span></span>  | <span data-ttu-id="3727f-162">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="3727f-162">An item was created.</span></span>
| <span data-ttu-id="3727f-163">delete</span><span class="sxs-lookup"><span data-stu-id="3727f-163">delete</span></span>      | <span data-ttu-id="3727f-164">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-164">[deleteAction][]</span></span>  | <span data-ttu-id="3727f-165">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="3727f-165">An item was deleted.</span></span>
| <span data-ttu-id="3727f-166">edit</span><span class="sxs-lookup"><span data-stu-id="3727f-166">edit</span></span>        | <span data-ttu-id="3727f-167">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-167">[editAction][]</span></span>    | <span data-ttu-id="3727f-168">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="3727f-168">An item was edited.</span></span>
| <span data-ttu-id="3727f-169">mention</span><span class="sxs-lookup"><span data-stu-id="3727f-169">mention</span></span>     | <span data-ttu-id="3727f-170">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-170">[mentionAction][]</span></span> | <span data-ttu-id="3727f-171">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="3727f-171">A user was mentioned in the item.</span></span>
| <span data-ttu-id="3727f-172">move</span><span class="sxs-lookup"><span data-stu-id="3727f-172">move</span></span>        | <span data-ttu-id="3727f-173">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-173">[moveAction][]</span></span>    | <span data-ttu-id="3727f-174">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="3727f-174">An item was moved.</span></span>
| <span data-ttu-id="3727f-175">rename</span><span class="sxs-lookup"><span data-stu-id="3727f-175">rename</span></span>      | <span data-ttu-id="3727f-176">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-176">[renameAction][]</span></span>  | <span data-ttu-id="3727f-177">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="3727f-177">An item was renamed.</span></span>
| <span data-ttu-id="3727f-178">restore</span><span class="sxs-lookup"><span data-stu-id="3727f-178">restore</span></span>     | <span data-ttu-id="3727f-179">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-179">[restoreAction][]</span></span> | <span data-ttu-id="3727f-180">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="3727f-180">An item was restored.</span></span>
| <span data-ttu-id="3727f-181">share</span><span class="sxs-lookup"><span data-stu-id="3727f-181">share</span></span>       | <span data-ttu-id="3727f-182">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-182">[shareAction][]</span></span>   | <span data-ttu-id="3727f-183">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="3727f-183">An item was shared.</span></span>
| <span data-ttu-id="3727f-184">version</span><span class="sxs-lookup"><span data-stu-id="3727f-184">version</span></span>     | <span data-ttu-id="3727f-185">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="3727f-185">[versionAction][]</span></span> | <span data-ttu-id="3727f-186">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="3727f-186">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="3727f-199">Comentários</span><span class="sxs-lookup"><span data-stu-id="3727f-199">Remarks</span></span>

<span data-ttu-id="3727f-200">**ItemActivity** está disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="3727f-200">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity"
} -->
