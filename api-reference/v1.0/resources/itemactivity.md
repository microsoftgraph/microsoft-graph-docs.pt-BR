---
author: daspek
ms.author: dspektor
title: tipo de recurso de multiatividade
description: O objeto myactivity fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4ae71056fccebcb372891124b01999004b1957c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009328"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="b2d1a-103">tipo de recurso de multiatividade</span><span class="sxs-lookup"><span data-stu-id="b2d1a-103">itemActivity resource type</span></span>

<span data-ttu-id="b2d1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2d1a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2d1a-105">O recurso **doactivity** fornece informações sobre as atividades que ocorreram em um item ou em um contêiner.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-105">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="b2d1a-106">Disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="b2d1a-107">As ações que ocorreram em um ItemProperty são detalhadas [na propriedade][] itempropertyset.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-107">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="b2d1a-108">**Observação:** o **myactivity** atualmente só está disponível no SharePoint e no onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-108">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="b2d1a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2d1a-110">Properties</span></span>

| <span data-ttu-id="b2d1a-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2d1a-111">Property</span></span> | <span data-ttu-id="b2d1a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2d1a-112">Type</span></span>                    | <span data-ttu-id="b2d1a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2d1a-113">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="b2d1a-114">id</span><span class="sxs-lookup"><span data-stu-id="b2d1a-114">id</span></span>       | <span data-ttu-id="b2d1a-115">string</span><span class="sxs-lookup"><span data-stu-id="b2d1a-115">string</span></span>                  | <span data-ttu-id="b2d1a-116">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-116">The unique identifier of the activity.</span></span> <span data-ttu-id="b2d1a-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-117">Read-only.</span></span>
| <span data-ttu-id="b2d1a-118">Access</span><span class="sxs-lookup"><span data-stu-id="b2d1a-118">access</span></span>   | <span data-ttu-id="b2d1a-119">[accessaction][]</span><span class="sxs-lookup"><span data-stu-id="b2d1a-119">[accessAction][]</span></span>        | <span data-ttu-id="b2d1a-120">Um item foi acessado.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-120">An item was accessed.</span></span>
| <span data-ttu-id="b2d1a-121">actor</span><span class="sxs-lookup"><span data-stu-id="b2d1a-121">actor</span></span>    | <span data-ttu-id="b2d1a-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b2d1a-122">[identitySet][]</span></span>         | <span data-ttu-id="b2d1a-123">Identidade de quem executou a ação.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-123">Identity of who performed the action.</span></span> <span data-ttu-id="b2d1a-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-124">Read-only.</span></span>
| <span data-ttu-id="b2d1a-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="b2d1a-125">activityDateTime</span></span>    | <span data-ttu-id="b2d1a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2d1a-126">DateTimeOffset</span></span> | <span data-ttu-id="b2d1a-127">Detalhes sobre quando ocorreu a atividade.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-127">Details about when the activity took place.</span></span> <span data-ttu-id="b2d1a-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-128">Read-only.</span></span>

[accessaction]: accessaction.md
[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="b2d1a-131">Relações</span><span class="sxs-lookup"><span data-stu-id="b2d1a-131">Relationships</span></span>

| <span data-ttu-id="b2d1a-132">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="b2d1a-132">Relationship name</span></span> | <span data-ttu-id="b2d1a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2d1a-133">Type</span></span>          | <span data-ttu-id="b2d1a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2d1a-134">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="b2d1a-135">driveItem</span><span class="sxs-lookup"><span data-stu-id="b2d1a-135">driveItem</span></span>         | <span data-ttu-id="b2d1a-136">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="b2d1a-136">[driveItem][]</span></span> | <span data-ttu-id="b2d1a-137">Expõe o **driveItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-137">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="b2d1a-138">listItem</span><span class="sxs-lookup"><span data-stu-id="b2d1a-138">listItem</span></span>          | <span data-ttu-id="b2d1a-139">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="b2d1a-139">[listItem][]</span></span>  | <span data-ttu-id="b2d1a-140">Expõe o **listItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="b2d1a-140">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="b2d1a-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2d1a-143">JSON representation</span></span>

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

