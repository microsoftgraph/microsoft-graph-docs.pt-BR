---
title: tipo de recurso workbookRangeFill
description: Representa a tela de fundo de um objeto Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d9a174d8d1cb6db278354522fc8c81933551fa84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519180"
---
# <a name="workbookrangefill-resource-type"></a><span data-ttu-id="aa70c-103">tipo de recurso workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="aa70c-103">workbookRangeFill resource type</span></span>

<span data-ttu-id="aa70c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aa70c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa70c-105">Representa a tela de fundo de um objeto Range.</span><span class="sxs-lookup"><span data-stu-id="aa70c-105">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="aa70c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="aa70c-106">Methods</span></span>

| <span data-ttu-id="aa70c-107">Método</span><span class="sxs-lookup"><span data-stu-id="aa70c-107">Method</span></span>           | <span data-ttu-id="aa70c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aa70c-108">Return Type</span></span>    |<span data-ttu-id="aa70c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa70c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa70c-110">Obter workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="aa70c-110">Get workbookRangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="aa70c-111">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="aa70c-111">workbookRangeFill</span></span>](workbookrangefill.md) |<span data-ttu-id="aa70c-112">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="aa70c-112">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="aa70c-113">Update</span><span class="sxs-lookup"><span data-stu-id="aa70c-113">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="aa70c-114">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="aa70c-114">workbookRangeFill</span></span>](workbookrangefill.md)   |<span data-ttu-id="aa70c-115">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="aa70c-115">Update RangeFill object.</span></span> |
|[<span data-ttu-id="aa70c-116">Clear</span><span class="sxs-lookup"><span data-stu-id="aa70c-116">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="aa70c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aa70c-117">None</span></span>|<span data-ttu-id="aa70c-118">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="aa70c-118">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa70c-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa70c-119">Properties</span></span>
| <span data-ttu-id="aa70c-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa70c-120">Property</span></span>     | <span data-ttu-id="aa70c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa70c-121">Type</span></span>   |<span data-ttu-id="aa70c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa70c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa70c-123">color</span><span class="sxs-lookup"><span data-stu-id="aa70c-123">color</span></span>|<span data-ttu-id="aa70c-124">string</span><span class="sxs-lookup"><span data-stu-id="aa70c-124">string</span></span>|<span data-ttu-id="aa70c-125">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="aa70c-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa70c-126">Relações</span><span class="sxs-lookup"><span data-stu-id="aa70c-126">Relationships</span></span>
<span data-ttu-id="aa70c-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aa70c-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="aa70c-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa70c-128">JSON representation</span></span>

<span data-ttu-id="aa70c-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa70c-129">Here is a JSON representation of the resource.</span></span>

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
