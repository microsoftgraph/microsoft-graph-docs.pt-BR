---
title: Tipo de recurso RangeFill
description: Representa o plano de fundo de um objeto de intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d1ae60c0b362ba8593f374c5edd505121cd18587
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509669"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="2ba92-103">Tipo de recurso RangeFill</span><span class="sxs-lookup"><span data-stu-id="2ba92-103">RangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba92-104">Representa o plano de fundo de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="2ba92-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="2ba92-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ba92-105">Methods</span></span>

| <span data-ttu-id="2ba92-106">Método</span><span class="sxs-lookup"><span data-stu-id="2ba92-106">Method</span></span>           | <span data-ttu-id="2ba92-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ba92-107">Return Type</span></span>    |<span data-ttu-id="2ba92-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ba92-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ba92-109">Get RangeFill</span><span class="sxs-lookup"><span data-stu-id="2ba92-109">[Get RangeFill](../api/rangefill-get.md)</span></span> | <span data-ttu-id="2ba92-110">RangeFill</span><span class="sxs-lookup"><span data-stu-id="2ba92-110">[RangeFill](rangefill.md)</span></span> |<span data-ttu-id="2ba92-111">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="2ba92-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="2ba92-112">Update</span><span class="sxs-lookup"><span data-stu-id="2ba92-112">Update</span></span>](../api/rangefill-update.md) | <span data-ttu-id="2ba92-113">RangeFill</span><span class="sxs-lookup"><span data-stu-id="2ba92-113">[RangeFill](rangefill.md)</span></span>   |<span data-ttu-id="2ba92-114">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="2ba92-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="2ba92-115">Clear</span><span class="sxs-lookup"><span data-stu-id="2ba92-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="2ba92-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ba92-116">None</span></span>|<span data-ttu-id="2ba92-117">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="2ba92-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ba92-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ba92-118">Properties</span></span>
| <span data-ttu-id="2ba92-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ba92-119">Property</span></span>     | <span data-ttu-id="2ba92-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ba92-120">Type</span></span>   |<span data-ttu-id="2ba92-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ba92-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ba92-122">color</span><span class="sxs-lookup"><span data-stu-id="2ba92-122">color</span></span>|<span data-ttu-id="2ba92-123">string</span><span class="sxs-lookup"><span data-stu-id="2ba92-123">string</span></span>|<span data-ttu-id="2ba92-124">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="2ba92-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ba92-125">Relações</span><span class="sxs-lookup"><span data-stu-id="2ba92-125">Relationships</span></span>
<span data-ttu-id="2ba92-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2ba92-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2ba92-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ba92-127">JSON representation</span></span>

<span data-ttu-id="2ba92-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ba92-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefill.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
