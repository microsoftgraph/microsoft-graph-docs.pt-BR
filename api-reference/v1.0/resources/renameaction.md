---
author: daspek
ms.author: dspektor
title: tipo de recurso renameaction
description: O objeto renameaction fornece informações sobre uma atividade que renomeia um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bce040130d74b7977fc1f988a34edde674f9e0d4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970603"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="641ae-103">tipo de recurso renameaction</span><span class="sxs-lookup"><span data-stu-id="641ae-103">renameAction resource type</span></span>

<span data-ttu-id="641ae-104">A presença do recurso \*\*\*\* renameaction em uma myactivity [\*\*\*\*] [ activity] indica que a atividade renomeou um item.</span><span class="sxs-lookup"><span data-stu-id="641ae-104">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="641ae-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="641ae-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="641ae-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="641ae-106">Properties</span></span>

| <span data-ttu-id="641ae-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="641ae-107">Property name</span></span> | <span data-ttu-id="641ae-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="641ae-108">Type</span></span>   | <span data-ttu-id="641ae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="641ae-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="641ae-110">oldName</span><span class="sxs-lookup"><span data-stu-id="641ae-110">oldName</span></span>       | <span data-ttu-id="641ae-111">string</span><span class="sxs-lookup"><span data-stu-id="641ae-111">string</span></span> | <span data-ttu-id="641ae-112">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="641ae-112">The previous name of the item.</span></span>
| <span data-ttu-id="641ae-113">newName</span><span class="sxs-lookup"><span data-stu-id="641ae-113">newName</span></span>       | <span data-ttu-id="641ae-114">string</span><span class="sxs-lookup"><span data-stu-id="641ae-114">string</span></span> | <span data-ttu-id="641ae-115">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="641ae-115">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="641ae-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="641ae-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->
