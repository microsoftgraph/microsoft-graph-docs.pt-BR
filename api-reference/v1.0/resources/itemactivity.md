---
author: daspek
ms.author: dspektor
title: tipo de recurso de multiatividade
description: O objeto myactivity fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ddd478794cc3ad87ce29513c45455a9ba2911a52
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036726"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="d5497-103">tipo de recurso de multiatividade</span><span class="sxs-lookup"><span data-stu-id="d5497-103">itemActivity resource type</span></span>

<span data-ttu-id="d5497-104">O \*\*\*\* recurso doactivity fornece informações sobre as atividades que ocorreram em um item ou em um contêiner.</span><span class="sxs-lookup"><span data-stu-id="d5497-104">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="d5497-105">Disponível atualmente só no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="d5497-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="d5497-106">As ações que ocorreram em um ItemProperty são detalhadas na propriedade itempropertyset. [][]</span><span class="sxs-lookup"><span data-stu-id="d5497-106">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="d5497-107">**Observação:** \*\*\*\* o myactivity atualmente só está disponível no SharePoint e no onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="d5497-107">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="d5497-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5497-109">Properties</span></span>

| <span data-ttu-id="d5497-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5497-110">Property</span></span> | <span data-ttu-id="d5497-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5497-111">Type</span></span>                    | <span data-ttu-id="d5497-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5497-112">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="d5497-113">id</span><span class="sxs-lookup"><span data-stu-id="d5497-113">id</span></span>       | <span data-ttu-id="d5497-114">string</span><span class="sxs-lookup"><span data-stu-id="d5497-114">string</span></span>                  | <span data-ttu-id="d5497-115">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="d5497-115">The unique identifier of the activity.</span></span> <span data-ttu-id="d5497-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5497-116">Read-only.</span></span>
| <span data-ttu-id="d5497-117">Access</span><span class="sxs-lookup"><span data-stu-id="d5497-117">access</span></span>   | <span data-ttu-id="d5497-118">[accessaction][]</span><span class="sxs-lookup"><span data-stu-id="d5497-118">[accessAction][]</span></span>        | <span data-ttu-id="d5497-119">Um item foi acessado.</span><span class="sxs-lookup"><span data-stu-id="d5497-119">An item was accessed.</span></span>
| <span data-ttu-id="d5497-120">actor</span><span class="sxs-lookup"><span data-stu-id="d5497-120">actor</span></span>    | <span data-ttu-id="d5497-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d5497-121">[identitySet][]</span></span>         | <span data-ttu-id="d5497-122">Identidade de quem executou a ação.</span><span class="sxs-lookup"><span data-stu-id="d5497-122">Identity of who performed the action.</span></span> <span data-ttu-id="d5497-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5497-123">Read-only.</span></span>
| <span data-ttu-id="d5497-124">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="d5497-124">activityDateTime</span></span>    | <span data-ttu-id="d5497-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5497-125">DateTimeOffset</span></span> | <span data-ttu-id="d5497-126">Detalhes sobre quando ocorreu a atividade.</span><span class="sxs-lookup"><span data-stu-id="d5497-126">Details about when the activity took place.</span></span> <span data-ttu-id="d5497-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5497-127">Read-only.</span></span>

[accessaction]: accessaction.md
[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="d5497-130">Relações</span><span class="sxs-lookup"><span data-stu-id="d5497-130">Relationships</span></span>

| <span data-ttu-id="d5497-131">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="d5497-131">Relationship name</span></span> | <span data-ttu-id="d5497-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5497-132">Type</span></span>          | <span data-ttu-id="d5497-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5497-133">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="d5497-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="d5497-134">driveItem</span></span>         | <span data-ttu-id="d5497-135">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="d5497-135">[driveItem][]</span></span> | <span data-ttu-id="d5497-136">Expõe o **driveItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="d5497-136">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="d5497-137">listItem</span><span class="sxs-lookup"><span data-stu-id="d5497-137">listItem</span></span>          | <span data-ttu-id="d5497-138">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="d5497-138">[listItem][]</span></span>  | <span data-ttu-id="d5497-139">Expõe o **listItem** ao qual essa atividade direcionou.</span><span class="sxs-lookup"><span data-stu-id="d5497-139">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="d5497-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5497-142">JSON representation</span></span>

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
