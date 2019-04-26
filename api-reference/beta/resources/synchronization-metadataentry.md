---
title: tipo de recurso metadataEntry
description: Metadados para o objeto especificado.
localization_priority: Normal
ms.openlocfilehash: 829dc5fbbf3d73dbabb2e9e69bfff28814cc203a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345568"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="e89ef-103">tipo de recurso metadataEntry</span><span class="sxs-lookup"><span data-stu-id="e89ef-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e89ef-104">Metadados para o objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="e89ef-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="e89ef-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e89ef-105">Properties</span></span>
| <span data-ttu-id="e89ef-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e89ef-106">Property</span></span>     | <span data-ttu-id="e89ef-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e89ef-107">Type</span></span>   |<span data-ttu-id="e89ef-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e89ef-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e89ef-109">key</span><span class="sxs-lookup"><span data-stu-id="e89ef-109">key</span></span>|<span data-ttu-id="e89ef-110">String</span><span class="sxs-lookup"><span data-stu-id="e89ef-110">String</span></span>|<span data-ttu-id="e89ef-111">Nome da propriedade de metadados.</span><span class="sxs-lookup"><span data-stu-id="e89ef-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="e89ef-112">value</span><span class="sxs-lookup"><span data-stu-id="e89ef-112">value</span></span>|<span data-ttu-id="e89ef-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e89ef-113">String</span></span>|<span data-ttu-id="e89ef-114">Valor da propriedade Metadata.</span><span class="sxs-lookup"><span data-stu-id="e89ef-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e89ef-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e89ef-115">JSON representation</span></span>

<span data-ttu-id="e89ef-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e89ef-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
