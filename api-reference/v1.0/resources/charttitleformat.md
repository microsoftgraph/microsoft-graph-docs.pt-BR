---
title: Tipo de recurso ChartTitleFormat
description: Abrange as propriedades de formatação do título do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: da702a7718765af464525c3ae2fafc8376296d25
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533082"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="69cef-103">Tipo de recurso ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="69cef-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="69cef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69cef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69cef-105">Abrange as propriedades de formatação do título do gráfico.</span><span class="sxs-lookup"><span data-stu-id="69cef-105">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="69cef-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="69cef-106">Methods</span></span>
<span data-ttu-id="69cef-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69cef-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="69cef-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69cef-108">Properties</span></span>
<span data-ttu-id="69cef-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="69cef-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="69cef-110">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="69cef-110">Relationships</span></span>
| <span data-ttu-id="69cef-111">Relação</span><span class="sxs-lookup"><span data-stu-id="69cef-111">Relationship</span></span> | <span data-ttu-id="69cef-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="69cef-112">Type</span></span>   |<span data-ttu-id="69cef-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="69cef-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69cef-114">fill</span><span class="sxs-lookup"><span data-stu-id="69cef-114">fill</span></span>|[<span data-ttu-id="69cef-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="69cef-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="69cef-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69cef-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="69cef-118">font</span><span class="sxs-lookup"><span data-stu-id="69cef-118">font</span></span>|[<span data-ttu-id="69cef-119">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="69cef-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="69cef-120">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="69cef-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="69cef-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69cef-121">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="69cef-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69cef-122">JSON representation</span></span>

<span data-ttu-id="69cef-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69cef-123">Here is a JSON representation of the resource.</span></span>

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
