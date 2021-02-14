---
author: daspek
title: Tipo de recurso itemActivity
description: O objeto itemActivity fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ef213dd50e5a6be8a96880ccd1a64f15f183f54b
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238684"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="05c29-103">Tipo de recurso itemActivity</span><span class="sxs-lookup"><span data-stu-id="05c29-103">itemActivity resource type</span></span>

<span data-ttu-id="05c29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05c29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05c29-105">O **recurso itemActivity** fornece informações sobre atividades que ocorreram em um item ou em um contêiner.</span><span class="sxs-lookup"><span data-stu-id="05c29-105">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="05c29-106">Disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="05c29-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="05c29-107">As ações que ocorreram em um itemActivity são detalhadas na [propriedade itemActionSet.][]</span><span class="sxs-lookup"><span data-stu-id="05c29-107">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="05c29-108">**Observação:** **itemActivity** só está disponível atualmente no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="05c29-108">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="05c29-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05c29-110">Properties</span></span>

| <span data-ttu-id="05c29-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05c29-111">Property</span></span> | <span data-ttu-id="05c29-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="05c29-112">Type</span></span>                    | <span data-ttu-id="05c29-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c29-113">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="05c29-114">id</span><span class="sxs-lookup"><span data-stu-id="05c29-114">id</span></span>       | <span data-ttu-id="05c29-115">string</span><span class="sxs-lookup"><span data-stu-id="05c29-115">string</span></span>                  | <span data-ttu-id="05c29-116">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="05c29-116">The unique identifier of the activity.</span></span> <span data-ttu-id="05c29-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05c29-117">Read-only.</span></span>
| <span data-ttu-id="05c29-118">access</span><span class="sxs-lookup"><span data-stu-id="05c29-118">access</span></span>   | <span data-ttu-id="05c29-119">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="05c29-119">[accessAction][]</span></span>        | <span data-ttu-id="05c29-120">Um item foi acessado.</span><span class="sxs-lookup"><span data-stu-id="05c29-120">An item was accessed.</span></span>
| <span data-ttu-id="05c29-121">actor</span><span class="sxs-lookup"><span data-stu-id="05c29-121">actor</span></span>    | <span data-ttu-id="05c29-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="05c29-122">[identitySet][]</span></span>         | <span data-ttu-id="05c29-123">Identidade de quem executou a ação.</span><span class="sxs-lookup"><span data-stu-id="05c29-123">Identity of who performed the action.</span></span> <span data-ttu-id="05c29-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05c29-124">Read-only.</span></span>
| <span data-ttu-id="05c29-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="05c29-125">activityDateTime</span></span>    | <span data-ttu-id="05c29-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05c29-126">DateTimeOffset</span></span> | <span data-ttu-id="05c29-127">Detalhes sobre quando ocorreu a atividade.</span><span class="sxs-lookup"><span data-stu-id="05c29-127">Details about when the activity took place.</span></span> <span data-ttu-id="05c29-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05c29-128">Read-only.</span></span>

[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="05c29-131">Relações</span><span class="sxs-lookup"><span data-stu-id="05c29-131">Relationships</span></span>

| <span data-ttu-id="05c29-132">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="05c29-132">Relationship name</span></span> | <span data-ttu-id="05c29-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="05c29-133">Type</span></span>          | <span data-ttu-id="05c29-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c29-134">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="05c29-135">driveItem</span><span class="sxs-lookup"><span data-stu-id="05c29-135">driveItem</span></span>         | <span data-ttu-id="05c29-136">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="05c29-136">[driveItem][]</span></span> | <span data-ttu-id="05c29-137">Expõe o **driveItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="05c29-137">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="05c29-138">listItem</span><span class="sxs-lookup"><span data-stu-id="05c29-138">listItem</span></span>          | <span data-ttu-id="05c29-139">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="05c29-139">[listItem][]</span></span>  | <span data-ttu-id="05c29-140">Expõe o **listItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="05c29-140">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="05c29-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05c29-143">JSON representation</span></span>

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

