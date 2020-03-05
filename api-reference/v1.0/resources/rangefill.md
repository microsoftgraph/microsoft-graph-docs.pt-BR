---
title: Tipo de recurso RangeFill
description: Representa a tela de fundo de um objeto Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 37bc96fdd0dad65a1f6b5b6bcec244ef96b915ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447021"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="07509-103">Tipo de recurso RangeFill</span><span class="sxs-lookup"><span data-stu-id="07509-103">RangeFill resource type</span></span>

<span data-ttu-id="07509-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="07509-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07509-105">Representa a tela de fundo de um objeto Range.</span><span class="sxs-lookup"><span data-stu-id="07509-105">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="07509-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="07509-106">Methods</span></span>

| <span data-ttu-id="07509-107">Método</span><span class="sxs-lookup"><span data-stu-id="07509-107">Method</span></span>           | <span data-ttu-id="07509-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="07509-108">Return Type</span></span>    |<span data-ttu-id="07509-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="07509-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07509-110">Get RangeFill</span><span class="sxs-lookup"><span data-stu-id="07509-110">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="07509-111">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="07509-111">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="07509-112">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="07509-112">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="07509-113">Update</span><span class="sxs-lookup"><span data-stu-id="07509-113">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="07509-114">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="07509-114">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="07509-115">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="07509-115">Update RangeFill object.</span></span> |
|[<span data-ttu-id="07509-116">Clear</span><span class="sxs-lookup"><span data-stu-id="07509-116">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="07509-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07509-117">None</span></span>|<span data-ttu-id="07509-118">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="07509-118">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="07509-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07509-119">Properties</span></span>
| <span data-ttu-id="07509-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07509-120">Property</span></span>     | <span data-ttu-id="07509-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="07509-121">Type</span></span>   |<span data-ttu-id="07509-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="07509-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07509-123">color</span><span class="sxs-lookup"><span data-stu-id="07509-123">color</span></span>|<span data-ttu-id="07509-124">string</span><span class="sxs-lookup"><span data-stu-id="07509-124">string</span></span>|<span data-ttu-id="07509-125">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="07509-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="07509-126">Relações</span><span class="sxs-lookup"><span data-stu-id="07509-126">Relationships</span></span>
<span data-ttu-id="07509-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07509-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="07509-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07509-128">JSON representation</span></span>

<span data-ttu-id="07509-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07509-129">Here is a JSON representation of the resource.</span></span>

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
