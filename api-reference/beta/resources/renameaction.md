---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: c204efb50802fb35ea059a923bf1ce0bc08ed519
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343840"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="a703d-102">Tipo de recurso RenameAction</span><span class="sxs-lookup"><span data-stu-id="a703d-102">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a703d-103">A presença do recurso **RenameAction** em uma [**itemActivity**][activity] indica que a atividade renomeou um item.</span><span class="sxs-lookup"><span data-stu-id="a703d-103">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="a703d-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a703d-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a703d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a703d-105">Properties</span></span>

| <span data-ttu-id="a703d-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a703d-106">Property name</span></span> | <span data-ttu-id="a703d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a703d-107">Type</span></span>   | <span data-ttu-id="a703d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a703d-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a703d-109">oldName</span><span class="sxs-lookup"><span data-stu-id="a703d-109">oldName</span></span>       | <span data-ttu-id="a703d-110">string</span><span class="sxs-lookup"><span data-stu-id="a703d-110">string</span></span> | <span data-ttu-id="a703d-111">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="a703d-111">The previous name of the item.</span></span>
| <span data-ttu-id="a703d-112">newName</span><span class="sxs-lookup"><span data-stu-id="a703d-112">newName</span></span>       | <span data-ttu-id="a703d-113">string</span><span class="sxs-lookup"><span data-stu-id="a703d-113">string</span></span> | <span data-ttu-id="a703d-114">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="a703d-114">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="a703d-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="a703d-115">Remarks</span></span>

<span data-ttu-id="a703d-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a703d-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": []
}
-->
