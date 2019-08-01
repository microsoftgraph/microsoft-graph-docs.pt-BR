---
title: Tipo de recurso RangeFill
description: Representa a tela de fundo de um objeto Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b884312f8c3a9e8e02242023556713be62f8529f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034906"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="a73a9-103">Tipo de recurso RangeFill</span><span class="sxs-lookup"><span data-stu-id="a73a9-103">RangeFill resource type</span></span>

<span data-ttu-id="a73a9-104">Representa a tela de fundo de um objeto Range.</span><span class="sxs-lookup"><span data-stu-id="a73a9-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="a73a9-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a73a9-105">Methods</span></span>

| <span data-ttu-id="a73a9-106">Método</span><span class="sxs-lookup"><span data-stu-id="a73a9-106">Method</span></span>           | <span data-ttu-id="a73a9-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a73a9-107">Return Type</span></span>    |<span data-ttu-id="a73a9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a73a9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a73a9-109">Get RangeFill</span><span class="sxs-lookup"><span data-stu-id="a73a9-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="a73a9-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="a73a9-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="a73a9-111">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="a73a9-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="a73a9-112">Update</span><span class="sxs-lookup"><span data-stu-id="a73a9-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="a73a9-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="a73a9-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="a73a9-114">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="a73a9-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="a73a9-115">Clear</span><span class="sxs-lookup"><span data-stu-id="a73a9-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="a73a9-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a73a9-116">None</span></span>|<span data-ttu-id="a73a9-117">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="a73a9-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="a73a9-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a73a9-118">Properties</span></span>
| <span data-ttu-id="a73a9-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a73a9-119">Property</span></span>     | <span data-ttu-id="a73a9-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a73a9-120">Type</span></span>   |<span data-ttu-id="a73a9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a73a9-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a73a9-122">color</span><span class="sxs-lookup"><span data-stu-id="a73a9-122">color</span></span>|<span data-ttu-id="a73a9-123">string</span><span class="sxs-lookup"><span data-stu-id="a73a9-123">string</span></span>|<span data-ttu-id="a73a9-124">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="a73a9-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="a73a9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="a73a9-125">Relationships</span></span>
<span data-ttu-id="a73a9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a73a9-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a73a9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a73a9-127">JSON representation</span></span>

<span data-ttu-id="a73a9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a73a9-128">Here is a JSON representation of the resource.</span></span>

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
