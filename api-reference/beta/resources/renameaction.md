---
author: daspek
description: A presença do recurso RenameAction em uma itemActivity indica que a atividade renomeou um item.
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6745f932c0a2d9b92273f45e147439cfbd2ed911
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521128"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="c8822-103">Tipo de recurso RenameAction</span><span class="sxs-lookup"><span data-stu-id="c8822-103">RenameAction resource type</span></span>

<span data-ttu-id="c8822-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c8822-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8822-105">A presença do recurso **RenameAction** em uma [**itemActivity**][activity] indica que a atividade renomeou um item.</span><span class="sxs-lookup"><span data-stu-id="c8822-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c8822-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8822-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c8822-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8822-107">Properties</span></span>

| <span data-ttu-id="c8822-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c8822-108">Property name</span></span> | <span data-ttu-id="c8822-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8822-109">Type</span></span>   | <span data-ttu-id="c8822-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8822-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c8822-111">oldName</span><span class="sxs-lookup"><span data-stu-id="c8822-111">oldName</span></span>       | <span data-ttu-id="c8822-112">string</span><span class="sxs-lookup"><span data-stu-id="c8822-112">string</span></span> | <span data-ttu-id="c8822-113">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="c8822-113">The previous name of the item.</span></span>
| <span data-ttu-id="c8822-114">newName</span><span class="sxs-lookup"><span data-stu-id="c8822-114">newName</span></span>       | <span data-ttu-id="c8822-115">string</span><span class="sxs-lookup"><span data-stu-id="c8822-115">string</span></span> | <span data-ttu-id="c8822-116">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="c8822-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="c8822-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="c8822-117">Remarks</span></span>

<span data-ttu-id="c8822-118">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="c8822-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
