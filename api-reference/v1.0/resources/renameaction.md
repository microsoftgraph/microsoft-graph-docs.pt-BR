---
author: daspek
ms.author: dspektor
title: tipo de recurso renameaction
description: O objeto renameaction fornece informações sobre uma atividade que renomeia um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2949a3875d657dba3c64b6753855476c1d66bfb3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034717"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="1d5b2-103">tipo de recurso renameaction</span><span class="sxs-lookup"><span data-stu-id="1d5b2-103">renameAction resource type</span></span>

<span data-ttu-id="1d5b2-104">A presença do recurso \*\*\*\* renameaction em uma myactivity indica que a atividade renomeou um item. [\*\*\*\*][activity]</span><span class="sxs-lookup"><span data-stu-id="1d5b2-104">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="1d5b2-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="1d5b2-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="1d5b2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d5b2-106">Properties</span></span>

| <span data-ttu-id="1d5b2-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1d5b2-107">Property name</span></span> | <span data-ttu-id="1d5b2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d5b2-108">Type</span></span>   | <span data-ttu-id="1d5b2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d5b2-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1d5b2-110">oldName</span><span class="sxs-lookup"><span data-stu-id="1d5b2-110">oldName</span></span>       | <span data-ttu-id="1d5b2-111">string</span><span class="sxs-lookup"><span data-stu-id="1d5b2-111">string</span></span> | <span data-ttu-id="1d5b2-112">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="1d5b2-112">The previous name of the item.</span></span>
| <span data-ttu-id="1d5b2-113">newName</span><span class="sxs-lookup"><span data-stu-id="1d5b2-113">newName</span></span>       | <span data-ttu-id="1d5b2-114">string</span><span class="sxs-lookup"><span data-stu-id="1d5b2-114">string</span></span> | <span data-ttu-id="1d5b2-115">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="1d5b2-115">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d5b2-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d5b2-116">JSON representation</span></span>

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
