---
title: Tipo de recurso ChartTitleFormat
description: Abrange as propriedades de formatação do título do gráfico.
author: lumine2008
ms.openlocfilehash: 16169af251a0764c99ae04c5516ad9d552d1654c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362136"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="d1a4d-103">Tipo de recurso ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="d1a4d-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="d1a4d-104">Abrange as propriedades de formatação do título do gráfico.</span><span class="sxs-lookup"><span data-stu-id="d1a4d-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="d1a4d-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d1a4d-105">Methods</span></span>
<span data-ttu-id="d1a4d-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1a4d-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="d1a4d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1a4d-107">Properties</span></span>
<span data-ttu-id="d1a4d-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1a4d-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d1a4d-109">Relações</span><span class="sxs-lookup"><span data-stu-id="d1a4d-109">Relationships</span></span>
| <span data-ttu-id="d1a4d-110">Relação</span><span class="sxs-lookup"><span data-stu-id="d1a4d-110">Relationship</span></span> | <span data-ttu-id="d1a4d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1a4d-111">Type</span></span>   |<span data-ttu-id="d1a4d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1a4d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1a4d-113">fill</span><span class="sxs-lookup"><span data-stu-id="d1a4d-113">fill</span></span>|[<span data-ttu-id="d1a4d-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="d1a4d-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="d1a4d-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1a4d-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="d1a4d-117">font</span><span class="sxs-lookup"><span data-stu-id="d1a4d-117">font</span></span>|[<span data-ttu-id="d1a4d-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d1a4d-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="d1a4d-p102">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1a4d-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="d1a4d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1a4d-121">JSON representation</span></span>

<span data-ttu-id="d1a4d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1a4d-122">Here is a JSON representation of the resource.</span></span>

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
