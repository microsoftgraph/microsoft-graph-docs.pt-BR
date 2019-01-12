---
title: Tipo de recurso RangeFill
description: Representa o plano de fundo de um objeto de intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 75aa4bd91ad6f1038fdc42460c6a3c9ab928a09d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911816"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="776ae-103">Tipo de recurso RangeFill</span><span class="sxs-lookup"><span data-stu-id="776ae-103">RangeFill resource type</span></span>

<span data-ttu-id="776ae-104">Representa o plano de fundo de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="776ae-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="776ae-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="776ae-105">Methods</span></span>

| <span data-ttu-id="776ae-106">Método</span><span class="sxs-lookup"><span data-stu-id="776ae-106">Method</span></span>           | <span data-ttu-id="776ae-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="776ae-107">Return Type</span></span>    |<span data-ttu-id="776ae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="776ae-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="776ae-109">Get RangeFill</span><span class="sxs-lookup"><span data-stu-id="776ae-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="776ae-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="776ae-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="776ae-111">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="776ae-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="776ae-112">Update</span><span class="sxs-lookup"><span data-stu-id="776ae-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="776ae-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="776ae-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="776ae-114">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="776ae-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="776ae-115">Clear</span><span class="sxs-lookup"><span data-stu-id="776ae-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="776ae-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="776ae-116">None</span></span>|<span data-ttu-id="776ae-117">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="776ae-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="776ae-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="776ae-118">Properties</span></span>
| <span data-ttu-id="776ae-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="776ae-119">Property</span></span>     | <span data-ttu-id="776ae-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="776ae-120">Type</span></span>   |<span data-ttu-id="776ae-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="776ae-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="776ae-122">color</span><span class="sxs-lookup"><span data-stu-id="776ae-122">color</span></span>|<span data-ttu-id="776ae-123">string</span><span class="sxs-lookup"><span data-stu-id="776ae-123">string</span></span>|<span data-ttu-id="776ae-124">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="776ae-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="776ae-125">Relações</span><span class="sxs-lookup"><span data-stu-id="776ae-125">Relationships</span></span>
<span data-ttu-id="776ae-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="776ae-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="776ae-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="776ae-127">JSON representation</span></span>

<span data-ttu-id="776ae-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="776ae-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
