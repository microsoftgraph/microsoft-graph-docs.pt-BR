---
author: daspek
ms.author: dspektor
title: tipo de recurso renameaction
description: O objeto renameaction fornece informações sobre uma atividade que renomeia um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b21d4630ca29aff9322d5114a5048b42f19fa4a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533845"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="fe8e4-103">tipo de recurso renameaction</span><span class="sxs-lookup"><span data-stu-id="fe8e4-103">renameAction resource type</span></span>

<span data-ttu-id="fe8e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe8e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe8e4-105">A presença do recurso **renameaction** em uma [**myactivity**][activity] indica que a atividade renomeou um item.</span><span class="sxs-lookup"><span data-stu-id="fe8e4-105">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="fe8e4-106">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="fe8e4-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="fe8e4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe8e4-107">Properties</span></span>

| <span data-ttu-id="fe8e4-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="fe8e4-108">Property name</span></span> | <span data-ttu-id="fe8e4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe8e4-109">Type</span></span>   | <span data-ttu-id="fe8e4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe8e4-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="fe8e4-111">oldName</span><span class="sxs-lookup"><span data-stu-id="fe8e4-111">oldName</span></span>       | <span data-ttu-id="fe8e4-112">string</span><span class="sxs-lookup"><span data-stu-id="fe8e4-112">string</span></span> | <span data-ttu-id="fe8e4-113">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="fe8e4-113">The previous name of the item.</span></span>
| <span data-ttu-id="fe8e4-114">newName</span><span class="sxs-lookup"><span data-stu-id="fe8e4-114">newName</span></span>       | <span data-ttu-id="fe8e4-115">string</span><span class="sxs-lookup"><span data-stu-id="fe8e4-115">string</span></span> | <span data-ttu-id="fe8e4-116">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="fe8e4-116">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe8e4-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe8e4-117">JSON representation</span></span>

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
