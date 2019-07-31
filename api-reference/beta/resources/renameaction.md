---
author: daspek
description: A presença do recurso RenameAction em uma itemActivity indica que a atividade renomeou um item.
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d62d3f7f836ece716bdc3e616e1943de8c040652
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965412"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="83722-103">Tipo de recurso RenameAction</span><span class="sxs-lookup"><span data-stu-id="83722-103">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83722-104">A presença do recurso **RenameAction** em uma [**itemActivity**][activity] indica que a atividade renomeou um item.</span><span class="sxs-lookup"><span data-stu-id="83722-104">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="83722-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83722-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="83722-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83722-106">Properties</span></span>

| <span data-ttu-id="83722-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="83722-107">Property name</span></span> | <span data-ttu-id="83722-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="83722-108">Type</span></span>   | <span data-ttu-id="83722-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="83722-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="83722-110">oldName</span><span class="sxs-lookup"><span data-stu-id="83722-110">oldName</span></span>       | <span data-ttu-id="83722-111">string</span><span class="sxs-lookup"><span data-stu-id="83722-111">string</span></span> | <span data-ttu-id="83722-112">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="83722-112">The previous name of the item.</span></span>
| <span data-ttu-id="83722-113">newName</span><span class="sxs-lookup"><span data-stu-id="83722-113">newName</span></span>       | <span data-ttu-id="83722-114">string</span><span class="sxs-lookup"><span data-stu-id="83722-114">string</span></span> | <span data-ttu-id="83722-115">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="83722-115">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="83722-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="83722-116">Remarks</span></span>

<span data-ttu-id="83722-117">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="83722-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
