---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: bc731a94167e16518c8dd9eaea7deabd5f519f7b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563073"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="7b52a-102">Tipo de recurso RenameAction</span><span class="sxs-lookup"><span data-stu-id="7b52a-102">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b52a-103">A presença do recurso **RenameAction** em uma [**itemActivity**][activity] indica que a atividade renomeou um item.</span><span class="sxs-lookup"><span data-stu-id="7b52a-103">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="7b52a-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b52a-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7b52a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b52a-105">Properties</span></span>

| <span data-ttu-id="7b52a-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7b52a-106">Property name</span></span> | <span data-ttu-id="7b52a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b52a-107">Type</span></span>   | <span data-ttu-id="7b52a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b52a-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="7b52a-109">oldName</span><span class="sxs-lookup"><span data-stu-id="7b52a-109">oldName</span></span>       | <span data-ttu-id="7b52a-110">string</span><span class="sxs-lookup"><span data-stu-id="7b52a-110">string</span></span> | <span data-ttu-id="7b52a-111">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="7b52a-111">The previous name of the item.</span></span>
| <span data-ttu-id="7b52a-112">newName</span><span class="sxs-lookup"><span data-stu-id="7b52a-112">newName</span></span>       | <span data-ttu-id="7b52a-113">string</span><span class="sxs-lookup"><span data-stu-id="7b52a-113">string</span></span> | <span data-ttu-id="7b52a-114">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="7b52a-114">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="7b52a-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="7b52a-115">Remarks</span></span>

<span data-ttu-id="7b52a-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="7b52a-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
