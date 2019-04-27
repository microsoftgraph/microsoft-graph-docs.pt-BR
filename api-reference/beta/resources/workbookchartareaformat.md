---
title: tipo de recurso workbookChartAreaFormat
description: Encapsula as propriedades de formato da área de gráfico geral.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6554604e2bb4c49d7e14546f1c5079690f99637f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348459"
---
# <a name="workbookchartareaformat-resource-type"></a><span data-ttu-id="28df4-103">tipo de recurso workbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="28df4-103">workbookChartAreaFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28df4-104">Encapsula as propriedades de formato da área de gráfico geral.</span><span class="sxs-lookup"><span data-stu-id="28df4-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="28df4-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="28df4-105">Methods</span></span>
<span data-ttu-id="28df4-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28df4-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="28df4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28df4-107">Properties</span></span>
<span data-ttu-id="28df4-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="28df4-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="28df4-109">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="28df4-109">Relationships</span></span>
| <span data-ttu-id="28df4-110">Relação</span><span class="sxs-lookup"><span data-stu-id="28df4-110">Relationship</span></span> | <span data-ttu-id="28df4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="28df4-111">Type</span></span>   |<span data-ttu-id="28df4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="28df4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28df4-113">fill</span><span class="sxs-lookup"><span data-stu-id="28df4-113">fill</span></span>|[<span data-ttu-id="28df4-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="28df4-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="28df4-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="28df4-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="28df4-117">font</span><span class="sxs-lookup"><span data-stu-id="28df4-117">font</span></span>|[<span data-ttu-id="28df4-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="28df4-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="28df4-119">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="28df4-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="28df4-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="28df4-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28df4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28df4-121">JSON representation</span></span>

<span data-ttu-id="28df4-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28df4-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
