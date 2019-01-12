---
title: Tipo de recurso ChartTitleFormat
description: Abrange as propriedades de formatação do título do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3a2c16d37d2ca86d7cafbb4047ee0bcea1ee4bde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977112"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="1d819-103">Tipo de recurso ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="1d819-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="1d819-104">Abrange as propriedades de formatação do título do gráfico.</span><span class="sxs-lookup"><span data-stu-id="1d819-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="1d819-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d819-105">Methods</span></span>
<span data-ttu-id="1d819-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d819-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="1d819-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d819-107">Properties</span></span>
<span data-ttu-id="1d819-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d819-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1d819-109">Relações</span><span class="sxs-lookup"><span data-stu-id="1d819-109">Relationships</span></span>
| <span data-ttu-id="1d819-110">Relação</span><span class="sxs-lookup"><span data-stu-id="1d819-110">Relationship</span></span> | <span data-ttu-id="1d819-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d819-111">Type</span></span>   |<span data-ttu-id="1d819-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d819-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d819-113">fill</span><span class="sxs-lookup"><span data-stu-id="1d819-113">fill</span></span>|[<span data-ttu-id="1d819-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="1d819-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="1d819-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1d819-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="1d819-117">font</span><span class="sxs-lookup"><span data-stu-id="1d819-117">font</span></span>|[<span data-ttu-id="1d819-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="1d819-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="1d819-p102">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1d819-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="1d819-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d819-121">JSON representation</span></span>

<span data-ttu-id="1d819-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d819-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
