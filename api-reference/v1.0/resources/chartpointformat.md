---
title: Tipo de recurso ChartPointFormat
description: Representa um objeto de formatação para os pontos do gráfico.
ms.openlocfilehash: f06b31ad030dd587128f35667145f19d5cbd2e7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005437"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="dfe71-103">Tipo de recurso ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="dfe71-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="dfe71-104">Representa um objeto de formatação para os pontos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="dfe71-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="dfe71-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="dfe71-105">Methods</span></span>
<span data-ttu-id="dfe71-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dfe71-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="dfe71-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dfe71-107">Properties</span></span>
<span data-ttu-id="dfe71-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dfe71-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="dfe71-109">Relações</span><span class="sxs-lookup"><span data-stu-id="dfe71-109">Relationships</span></span>
| <span data-ttu-id="dfe71-110">Relação</span><span class="sxs-lookup"><span data-stu-id="dfe71-110">Relationship</span></span> | <span data-ttu-id="dfe71-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfe71-111">Type</span></span>   |<span data-ttu-id="dfe71-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfe71-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfe71-113">fill</span><span class="sxs-lookup"><span data-stu-id="dfe71-113">fill</span></span>|[<span data-ttu-id="dfe71-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="dfe71-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="dfe71-p101">Representa o formato de preenchimento de um gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dfe71-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dfe71-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dfe71-117">JSON representation</span></span>

<span data-ttu-id="dfe71-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dfe71-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->