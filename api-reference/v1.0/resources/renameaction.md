---
author: daspek
title: Tipo de recurso renameAction
description: O objeto renameAction fornece informações sobre uma atividade que renomeou um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 35e0aa9929b8e152265a5540625f5981a587edb7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238649"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="c5336-103">Tipo de recurso renameAction</span><span class="sxs-lookup"><span data-stu-id="c5336-103">renameAction resource type</span></span>

<span data-ttu-id="c5336-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5336-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5336-105">A presença do recurso **renameAction** em um [**itemActivity**][activity] indica que a atividade renomeou um item.</span><span class="sxs-lookup"><span data-stu-id="c5336-105">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="c5336-106">**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="c5336-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="c5336-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5336-107">Properties</span></span>

| <span data-ttu-id="c5336-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c5336-108">Property name</span></span> | <span data-ttu-id="c5336-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5336-109">Type</span></span>   | <span data-ttu-id="c5336-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5336-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c5336-111">oldName</span><span class="sxs-lookup"><span data-stu-id="c5336-111">oldName</span></span>       | <span data-ttu-id="c5336-112">string</span><span class="sxs-lookup"><span data-stu-id="c5336-112">string</span></span> | <span data-ttu-id="c5336-113">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="c5336-113">The previous name of the item.</span></span>
| <span data-ttu-id="c5336-114">newName</span><span class="sxs-lookup"><span data-stu-id="c5336-114">newName</span></span>       | <span data-ttu-id="c5336-115">string</span><span class="sxs-lookup"><span data-stu-id="c5336-115">string</span></span> | <span data-ttu-id="c5336-116">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="c5336-116">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5336-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5336-117">JSON representation</span></span>

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

