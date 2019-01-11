---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
ms.openlocfilehash: a29bdad0ae5e06d3d1b55f1fb7ceb630bec1b564
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819667"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="eafce-102">Tipo de recurso ItemActivity</span><span class="sxs-lookup"><span data-stu-id="eafce-102">ItemActivity resource type</span></span>

> <span data-ttu-id="eafce-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eafce-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eafce-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eafce-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eafce-105">O recurso **ItemActivity** fornece informações sobre atividades que ocorreram em um item ou dentro de um repositório.</span><span class="sxs-lookup"><span data-stu-id="eafce-105">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="eafce-106">Disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="eafce-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eafce-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eafce-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="eafce-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eafce-108">Properties</span></span>

| <span data-ttu-id="eafce-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eafce-109">Property</span></span> | <span data-ttu-id="eafce-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eafce-110">Type</span></span>                    | <span data-ttu-id="eafce-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eafce-111">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="eafce-112">id</span><span class="sxs-lookup"><span data-stu-id="eafce-112">id</span></span>       | <span data-ttu-id="eafce-113">string</span><span class="sxs-lookup"><span data-stu-id="eafce-113">string</span></span>                  | <span data-ttu-id="eafce-114">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="eafce-114">The unique identifier of the activity.</span></span> <span data-ttu-id="eafce-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eafce-115">Read-only.</span></span>
| <span data-ttu-id="eafce-116">acesso</span><span class="sxs-lookup"><span data-stu-id="eafce-116">access</span></span>   | <span data-ttu-id="eafce-117">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-117">[accessAction][]</span></span>        | <span data-ttu-id="eafce-118">Um item foi acessado.</span><span class="sxs-lookup"><span data-stu-id="eafce-118">An item was accessed.</span></span>
| <span data-ttu-id="eafce-119">action</span><span class="sxs-lookup"><span data-stu-id="eafce-119">action</span></span>   | <span data-ttu-id="eafce-120">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="eafce-120">[itemActionSet][]</span></span>       | <span data-ttu-id="eafce-121">Detalhes sobre a ação que ocorreu.</span><span class="sxs-lookup"><span data-stu-id="eafce-121">Details about the action that took place.</span></span> <span data-ttu-id="eafce-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eafce-122">Read-only.</span></span>
| <span data-ttu-id="eafce-123">actor</span><span class="sxs-lookup"><span data-stu-id="eafce-123">actor</span></span>    | <span data-ttu-id="eafce-124">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="eafce-124">[identitySet][]</span></span>         | <span data-ttu-id="eafce-125">Identidade de quem executou a ação.</span><span class="sxs-lookup"><span data-stu-id="eafce-125">Identity of who performed the action.</span></span> <span data-ttu-id="eafce-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eafce-126">Read-only.</span></span>
| <span data-ttu-id="eafce-127">location</span><span class="sxs-lookup"><span data-stu-id="eafce-127">location</span></span> | <span data-ttu-id="eafce-128">[location][]</span><span class="sxs-lookup"><span data-stu-id="eafce-128">[location][]</span></span>            | <span data-ttu-id="eafce-129">Local físico onde a ação foi realizada.</span><span class="sxs-lookup"><span data-stu-id="eafce-129">Physical location where the action was performed.</span></span> <span data-ttu-id="eafce-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eafce-130">Read-only.</span></span>
| <span data-ttu-id="eafce-131">times</span><span class="sxs-lookup"><span data-stu-id="eafce-131">times</span></span>    | <span data-ttu-id="eafce-132">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="eafce-132">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="eafce-133">Detalhes sobre quando ocorreu a atividade.</span><span class="sxs-lookup"><span data-stu-id="eafce-133">Details about when the activity took place.</span></span> <span data-ttu-id="eafce-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eafce-134">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="eafce-138">Relações</span><span class="sxs-lookup"><span data-stu-id="eafce-138">Relationships</span></span>

| <span data-ttu-id="eafce-139">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="eafce-139">Relationship name</span></span> | <span data-ttu-id="eafce-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="eafce-140">Type</span></span>          | <span data-ttu-id="eafce-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="eafce-141">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="eafce-142">driveItem</span><span class="sxs-lookup"><span data-stu-id="eafce-142">driveItem</span></span>         | <span data-ttu-id="eafce-143">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="eafce-143">[driveItem][]</span></span> | <span data-ttu-id="eafce-144">Expõe o **driveItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="eafce-144">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="eafce-145">listItem</span><span class="sxs-lookup"><span data-stu-id="eafce-145">listItem</span></span>          | <span data-ttu-id="eafce-146">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="eafce-146">[listItem][]</span></span>  | <span data-ttu-id="eafce-147">Expõe o **listItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="eafce-147">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="eafce-150">Ações</span><span class="sxs-lookup"><span data-stu-id="eafce-150">Actions</span></span>

<span data-ttu-id="eafce-151">As ações que ocorreram dentro de uma atividade são detalhadas na propriedade **action**.</span><span class="sxs-lookup"><span data-stu-id="eafce-151">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="eafce-152">Abaixo estão as ações disponíveis atualmente.</span><span class="sxs-lookup"><span data-stu-id="eafce-152">Below are the actions that are available today.</span></span>
<span data-ttu-id="eafce-153">Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActivity** sem quaisquer ações que seu aplicativo entenda.</span><span class="sxs-lookup"><span data-stu-id="eafce-153">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="eafce-154">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="eafce-154">Action name</span></span> | <span data-ttu-id="eafce-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="eafce-155">Type</span></span>              | <span data-ttu-id="eafce-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="eafce-156">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="eafce-157">comment</span><span class="sxs-lookup"><span data-stu-id="eafce-157">comment</span></span>     | <span data-ttu-id="eafce-158">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-158">[commentAction][]</span></span> | <span data-ttu-id="eafce-159">Um comentário foi adicionado ao item.</span><span class="sxs-lookup"><span data-stu-id="eafce-159">A comment was added to the item.</span></span>
| <span data-ttu-id="eafce-160">create</span><span class="sxs-lookup"><span data-stu-id="eafce-160">create</span></span>      | <span data-ttu-id="eafce-161">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-161">[createAction][]</span></span>  | <span data-ttu-id="eafce-162">Um item foi criado.</span><span class="sxs-lookup"><span data-stu-id="eafce-162">An item was created.</span></span>
| <span data-ttu-id="eafce-163">delete</span><span class="sxs-lookup"><span data-stu-id="eafce-163">delete</span></span>      | <span data-ttu-id="eafce-164">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-164">[deleteAction][]</span></span>  | <span data-ttu-id="eafce-165">Um item foi excluído.</span><span class="sxs-lookup"><span data-stu-id="eafce-165">An item was deleted.</span></span>
| <span data-ttu-id="eafce-166">edit</span><span class="sxs-lookup"><span data-stu-id="eafce-166">edit</span></span>        | <span data-ttu-id="eafce-167">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-167">[editAction][]</span></span>    | <span data-ttu-id="eafce-168">Um item foi editado.</span><span class="sxs-lookup"><span data-stu-id="eafce-168">An item was edited.</span></span>
| <span data-ttu-id="eafce-169">mention</span><span class="sxs-lookup"><span data-stu-id="eafce-169">mention</span></span>     | <span data-ttu-id="eafce-170">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-170">[mentionAction][]</span></span> | <span data-ttu-id="eafce-171">Um usuário foi mencionado no item.</span><span class="sxs-lookup"><span data-stu-id="eafce-171">A user was mentioned in the item.</span></span>
| <span data-ttu-id="eafce-172">move</span><span class="sxs-lookup"><span data-stu-id="eafce-172">move</span></span>        | <span data-ttu-id="eafce-173">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-173">[moveAction][]</span></span>    | <span data-ttu-id="eafce-174">Um item foi movido.</span><span class="sxs-lookup"><span data-stu-id="eafce-174">An item was moved.</span></span>
| <span data-ttu-id="eafce-175">rename</span><span class="sxs-lookup"><span data-stu-id="eafce-175">rename</span></span>      | <span data-ttu-id="eafce-176">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-176">[renameAction][]</span></span>  | <span data-ttu-id="eafce-177">Um item foi renomeado.</span><span class="sxs-lookup"><span data-stu-id="eafce-177">An item was renamed.</span></span>
| <span data-ttu-id="eafce-178">restore</span><span class="sxs-lookup"><span data-stu-id="eafce-178">restore</span></span>     | <span data-ttu-id="eafce-179">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-179">[restoreAction][]</span></span> | <span data-ttu-id="eafce-180">Um item foi restaurado.</span><span class="sxs-lookup"><span data-stu-id="eafce-180">An item was restored.</span></span>
| <span data-ttu-id="eafce-181">share</span><span class="sxs-lookup"><span data-stu-id="eafce-181">share</span></span>       | <span data-ttu-id="eafce-182">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-182">[shareAction][]</span></span>   | <span data-ttu-id="eafce-183">Um item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="eafce-183">An item was shared.</span></span>
| <span data-ttu-id="eafce-184">version</span><span class="sxs-lookup"><span data-stu-id="eafce-184">version</span></span>     | <span data-ttu-id="eafce-185">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="eafce-185">[versionAction][]</span></span> | <span data-ttu-id="eafce-186">Foi feito o controle de versão de um item.</span><span class="sxs-lookup"><span data-stu-id="eafce-186">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="eafce-199">Comentários</span><span class="sxs-lookup"><span data-stu-id="eafce-199">Remarks</span></span>

<span data-ttu-id="eafce-200">**ItemActivity** está disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="eafce-200">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity"
} -->
