---
title: Tipo de recurso ChartAreaFormat
description: Abrange as propriedades de formatação da área geral do gráfico.
ms.openlocfilehash: 19f09ab735f6df4fe4cdc0ccbf13bc75a5ca834e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003765"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="74a2d-103">Tipo de recurso ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="74a2d-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="74a2d-104">Abrange as propriedades de formatação da área geral do gráfico.</span><span class="sxs-lookup"><span data-stu-id="74a2d-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="74a2d-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="74a2d-105">Methods</span></span>
<span data-ttu-id="74a2d-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74a2d-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="74a2d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74a2d-107">Properties</span></span>
<span data-ttu-id="74a2d-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74a2d-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="74a2d-109">Relações</span><span class="sxs-lookup"><span data-stu-id="74a2d-109">Relationships</span></span>
| <span data-ttu-id="74a2d-110">Relação</span><span class="sxs-lookup"><span data-stu-id="74a2d-110">Relationship</span></span> | <span data-ttu-id="74a2d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="74a2d-111">Type</span></span>   |<span data-ttu-id="74a2d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="74a2d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74a2d-113">fill</span><span class="sxs-lookup"><span data-stu-id="74a2d-113">fill</span></span>|[<span data-ttu-id="74a2d-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="74a2d-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="74a2d-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74a2d-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="74a2d-117">font</span><span class="sxs-lookup"><span data-stu-id="74a2d-117">font</span></span>|[<span data-ttu-id="74a2d-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="74a2d-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="74a2d-p102">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74a2d-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74a2d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74a2d-121">JSON representation</span></span>

<span data-ttu-id="74a2d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74a2d-122">Here is a JSON representation of the resource.</span></span>

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