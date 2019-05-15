---
author: daspek
ms.author: dspektor
title: tipo de recurso de multiatividade
description: O objeto myactivity fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c05493ddeb8e007da6ba8b7508369b4d013e672
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970597"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="eb4ab-103">tipo de recurso de multiatividade</span><span class="sxs-lookup"><span data-stu-id="eb4ab-103">itemActivity resource type</span></span>

<span data-ttu-id="eb4ab-104">O \*\*\*\* recurso doactivity fornece informações sobre as atividades que ocorreram em um item ou em um contêiner.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-104">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="eb4ab-105">Disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="eb4ab-106">As ações que ocorreram em um ItemProperty são detalhadas na propriedade itempropertyset. [][]</span><span class="sxs-lookup"><span data-stu-id="eb4ab-106">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="eb4ab-107">**Observação:** \*\*\*\* o myactivity atualmente só está disponível no SharePoint e no onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-107">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="eb4ab-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb4ab-109">Properties</span></span>

| <span data-ttu-id="eb4ab-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb4ab-110">Property</span></span> | <span data-ttu-id="eb4ab-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb4ab-111">Type</span></span>                    | <span data-ttu-id="eb4ab-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb4ab-112">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="eb4ab-113">id</span><span class="sxs-lookup"><span data-stu-id="eb4ab-113">id</span></span>       | <span data-ttu-id="eb4ab-114">string</span><span class="sxs-lookup"><span data-stu-id="eb4ab-114">string</span></span>                  | <span data-ttu-id="eb4ab-115">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-115">The unique identifier of the activity.</span></span> <span data-ttu-id="eb4ab-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-116">Read-only.</span></span>
| <span data-ttu-id="eb4ab-117">Access</span><span class="sxs-lookup"><span data-stu-id="eb4ab-117">access</span></span>   | <span data-ttu-id="eb4ab-118">[accessaction][]</span><span class="sxs-lookup"><span data-stu-id="eb4ab-118">[accessAction][]</span></span>        | <span data-ttu-id="eb4ab-119">Um item foi acessado.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-119">An item was accessed.</span></span>
| <span data-ttu-id="eb4ab-120">actor</span><span class="sxs-lookup"><span data-stu-id="eb4ab-120">actor</span></span>    | <span data-ttu-id="eb4ab-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="eb4ab-121">[identitySet][]</span></span>         | <span data-ttu-id="eb4ab-122">Identidade de quem executou a ação.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-122">Identity of who performed the action.</span></span> <span data-ttu-id="eb4ab-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-123">Read-only.</span></span>
| <span data-ttu-id="eb4ab-124">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="eb4ab-124">activityDateTime</span></span>    | <span data-ttu-id="eb4ab-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb4ab-125">DateTimeOffset</span></span> | <span data-ttu-id="eb4ab-126">Detalhes sobre quando ocorreu a atividade.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-126">Details about when the activity took place.</span></span> <span data-ttu-id="eb4ab-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-127">Read-only.</span></span>

[accessaction]: accessAction.md
[accessAction]: accessAction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="eb4ab-130">Relações</span><span class="sxs-lookup"><span data-stu-id="eb4ab-130">Relationships</span></span>

| <span data-ttu-id="eb4ab-131">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="eb4ab-131">Relationship name</span></span> | <span data-ttu-id="eb4ab-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb4ab-132">Type</span></span>          | <span data-ttu-id="eb4ab-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb4ab-133">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="eb4ab-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="eb4ab-134">driveItem</span></span>         | <span data-ttu-id="eb4ab-135">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="eb4ab-135">[driveItem][]</span></span> | <span data-ttu-id="eb4ab-136">Expõe o **driveItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-136">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="eb4ab-137">listItem</span><span class="sxs-lookup"><span data-stu-id="eb4ab-137">listItem</span></span>          | <span data-ttu-id="eb4ab-138">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="eb4ab-138">[listItem][]</span></span>  | <span data-ttu-id="eb4ab-139">Expõe o **listItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="eb4ab-139">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="eb4ab-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb4ab-142">JSON representation</span></span>

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
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "activityDateTime": {"@odata.type": "String (timestamp)"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActivity",
  "suppressions": []
}
-->
