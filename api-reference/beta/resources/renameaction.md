---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: bc731a94167e16518c8dd9eaea7deabd5f519f7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515465"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="1c5a7-102">Tipo de recurso RenameAction</span><span class="sxs-lookup"><span data-stu-id="1c5a7-102">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c5a7-103">A presença do recurso **RenameAction** em uma [**itemActivity**][activity] indica que a atividade renomeou um item.</span><span class="sxs-lookup"><span data-stu-id="1c5a7-103">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="1c5a7-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c5a7-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1c5a7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c5a7-105">Properties</span></span>

| <span data-ttu-id="1c5a7-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1c5a7-106">Property name</span></span> | <span data-ttu-id="1c5a7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c5a7-107">Type</span></span>   | <span data-ttu-id="1c5a7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c5a7-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1c5a7-109">oldName</span><span class="sxs-lookup"><span data-stu-id="1c5a7-109">oldName</span></span>       | <span data-ttu-id="1c5a7-110">string</span><span class="sxs-lookup"><span data-stu-id="1c5a7-110">string</span></span> | <span data-ttu-id="1c5a7-111">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="1c5a7-111">The previous name of the item.</span></span>
| <span data-ttu-id="1c5a7-112">newName</span><span class="sxs-lookup"><span data-stu-id="1c5a7-112">newName</span></span>       | <span data-ttu-id="1c5a7-113">string</span><span class="sxs-lookup"><span data-stu-id="1c5a7-113">string</span></span> | <span data-ttu-id="1c5a7-114">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="1c5a7-114">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="1c5a7-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="1c5a7-115">Remarks</span></span>

<span data-ttu-id="1c5a7-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="1c5a7-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/renameaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
