---
title: Tipo de recurso ChartAreaFormat
description: Abrange as propriedades de formatação da área geral do gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 79867ff3519467279abcb4b9684b713964eb8f98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838168"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="34c02-103">Tipo de recurso ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="34c02-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="34c02-104">Abrange as propriedades de formatação da área geral do gráfico.</span><span class="sxs-lookup"><span data-stu-id="34c02-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="34c02-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="34c02-105">Methods</span></span>
<span data-ttu-id="34c02-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34c02-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="34c02-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34c02-107">Properties</span></span>
<span data-ttu-id="34c02-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34c02-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="34c02-109">Relações</span><span class="sxs-lookup"><span data-stu-id="34c02-109">Relationships</span></span>
| <span data-ttu-id="34c02-110">Relação</span><span class="sxs-lookup"><span data-stu-id="34c02-110">Relationship</span></span> | <span data-ttu-id="34c02-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="34c02-111">Type</span></span>   |<span data-ttu-id="34c02-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="34c02-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34c02-113">fill</span><span class="sxs-lookup"><span data-stu-id="34c02-113">fill</span></span>|[<span data-ttu-id="34c02-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="34c02-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="34c02-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34c02-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="34c02-117">font</span><span class="sxs-lookup"><span data-stu-id="34c02-117">font</span></span>|[<span data-ttu-id="34c02-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="34c02-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="34c02-p102">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34c02-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34c02-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34c02-121">JSON representation</span></span>

<span data-ttu-id="34c02-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34c02-122">Here is a JSON representation of the resource.</span></span>

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
