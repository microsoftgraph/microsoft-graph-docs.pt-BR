---
title: tipo de recurso workbookRangeFill
description: Representa a tela de fundo de um objeto Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: cb61352964323b0ded8733aa52ddd19854e028d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007092"
---
# <a name="workbookrangefill-resource-type"></a><span data-ttu-id="7b0ae-103">tipo de recurso workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="7b0ae-103">workbookRangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b0ae-104">Representa a tela de fundo de um objeto Range.</span><span class="sxs-lookup"><span data-stu-id="7b0ae-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="7b0ae-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b0ae-105">Methods</span></span>

| <span data-ttu-id="7b0ae-106">Método</span><span class="sxs-lookup"><span data-stu-id="7b0ae-106">Method</span></span>           | <span data-ttu-id="7b0ae-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b0ae-107">Return Type</span></span>    |<span data-ttu-id="7b0ae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b0ae-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b0ae-109">Obter workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="7b0ae-109">Get workbookRangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="7b0ae-110">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="7b0ae-110">workbookRangeFill</span></span>](workbookrangefill.md) |<span data-ttu-id="7b0ae-111">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="7b0ae-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="7b0ae-112">Update</span><span class="sxs-lookup"><span data-stu-id="7b0ae-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="7b0ae-113">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="7b0ae-113">workbookRangeFill</span></span>](workbookrangefill.md)   |<span data-ttu-id="7b0ae-114">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="7b0ae-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="7b0ae-115">Clear</span><span class="sxs-lookup"><span data-stu-id="7b0ae-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="7b0ae-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b0ae-116">None</span></span>|<span data-ttu-id="7b0ae-117">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="7b0ae-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b0ae-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b0ae-118">Properties</span></span>
| <span data-ttu-id="7b0ae-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b0ae-119">Property</span></span>     | <span data-ttu-id="7b0ae-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b0ae-120">Type</span></span>   |<span data-ttu-id="7b0ae-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b0ae-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b0ae-122">color</span><span class="sxs-lookup"><span data-stu-id="7b0ae-122">color</span></span>|<span data-ttu-id="7b0ae-123">string</span><span class="sxs-lookup"><span data-stu-id="7b0ae-123">string</span></span>|<span data-ttu-id="7b0ae-124">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="7b0ae-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b0ae-125">Relações</span><span class="sxs-lookup"><span data-stu-id="7b0ae-125">Relationships</span></span>
<span data-ttu-id="7b0ae-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b0ae-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7b0ae-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b0ae-127">JSON representation</span></span>

<span data-ttu-id="7b0ae-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b0ae-128">Here is a JSON representation of the resource.</span></span>

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
