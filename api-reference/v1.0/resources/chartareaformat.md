---
title: Tipo de recurso ChartAreaFormat
description: Abrange as propriedades de formatação da área geral do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a447b604807f3ae223445db953d45928eda9f36b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939991"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="69fc7-103">Tipo de recurso ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="69fc7-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="69fc7-104">Abrange as propriedades de formatação da área geral do gráfico.</span><span class="sxs-lookup"><span data-stu-id="69fc7-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="69fc7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="69fc7-105">Methods</span></span>
<span data-ttu-id="69fc7-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69fc7-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="69fc7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69fc7-107">Properties</span></span>
<span data-ttu-id="69fc7-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69fc7-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="69fc7-109">Relações</span><span class="sxs-lookup"><span data-stu-id="69fc7-109">Relationships</span></span>
| <span data-ttu-id="69fc7-110">Relação</span><span class="sxs-lookup"><span data-stu-id="69fc7-110">Relationship</span></span> | <span data-ttu-id="69fc7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="69fc7-111">Type</span></span>   |<span data-ttu-id="69fc7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="69fc7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69fc7-113">fill</span><span class="sxs-lookup"><span data-stu-id="69fc7-113">fill</span></span>|[<span data-ttu-id="69fc7-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="69fc7-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="69fc7-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69fc7-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="69fc7-117">font</span><span class="sxs-lookup"><span data-stu-id="69fc7-117">font</span></span>|[<span data-ttu-id="69fc7-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="69fc7-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="69fc7-p102">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69fc7-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69fc7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69fc7-121">JSON representation</span></span>

<span data-ttu-id="69fc7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69fc7-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
