---
title: tipo de recurso workbookRangeFill
description: Representa a tela de fundo de um objeto Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 60f2af8ce43dcba1866949864e581b4c933ee760
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046214"
---
# <a name="workbookrangefill-resource-type"></a><span data-ttu-id="a86cc-103">tipo de recurso workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="a86cc-103">workbookRangeFill resource type</span></span>

<span data-ttu-id="a86cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a86cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a86cc-105">Representa a tela de fundo de um objeto Range.</span><span class="sxs-lookup"><span data-stu-id="a86cc-105">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="a86cc-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a86cc-106">Methods</span></span>

| <span data-ttu-id="a86cc-107">Método</span><span class="sxs-lookup"><span data-stu-id="a86cc-107">Method</span></span>           | <span data-ttu-id="a86cc-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a86cc-108">Return Type</span></span>    |<span data-ttu-id="a86cc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a86cc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a86cc-110">Obter workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="a86cc-110">Get workbookRangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="a86cc-111">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="a86cc-111">workbookRangeFill</span></span>](workbookrangefill.md) |<span data-ttu-id="a86cc-112">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="a86cc-112">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="a86cc-113">Update</span><span class="sxs-lookup"><span data-stu-id="a86cc-113">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="a86cc-114">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="a86cc-114">workbookRangeFill</span></span>](workbookrangefill.md)   |<span data-ttu-id="a86cc-115">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="a86cc-115">Update RangeFill object.</span></span> |
|[<span data-ttu-id="a86cc-116">Clear</span><span class="sxs-lookup"><span data-stu-id="a86cc-116">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="a86cc-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a86cc-117">None</span></span>|<span data-ttu-id="a86cc-118">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="a86cc-118">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="a86cc-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a86cc-119">Properties</span></span>
| <span data-ttu-id="a86cc-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a86cc-120">Property</span></span>     | <span data-ttu-id="a86cc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a86cc-121">Type</span></span>   |<span data-ttu-id="a86cc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a86cc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a86cc-123">color</span><span class="sxs-lookup"><span data-stu-id="a86cc-123">color</span></span>|<span data-ttu-id="a86cc-124">string</span><span class="sxs-lookup"><span data-stu-id="a86cc-124">string</span></span>|<span data-ttu-id="a86cc-125">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="a86cc-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="a86cc-126">Relações</span><span class="sxs-lookup"><span data-stu-id="a86cc-126">Relationships</span></span>
<span data-ttu-id="a86cc-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a86cc-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a86cc-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a86cc-128">JSON representation</span></span>

<span data-ttu-id="a86cc-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a86cc-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFill"
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
  "suppressions": []
}
-->


