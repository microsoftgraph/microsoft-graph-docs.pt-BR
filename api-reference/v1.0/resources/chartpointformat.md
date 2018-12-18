---
title: Tipo de recurso ChartPointFormat
description: Representa um objeto de formatação para os pontos do gráfico.
author: lumine2008
ms.openlocfilehash: 94ba58eb60f80cf704de3d8a44e6e96f010429a7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311309"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="d2692-103">Tipo de recurso ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="d2692-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="d2692-104">Representa um objeto de formatação para os pontos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="d2692-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="d2692-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2692-105">Methods</span></span>
<span data-ttu-id="d2692-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2692-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="d2692-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2692-107">Properties</span></span>
<span data-ttu-id="d2692-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2692-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d2692-109">Relações</span><span class="sxs-lookup"><span data-stu-id="d2692-109">Relationships</span></span>
| <span data-ttu-id="d2692-110">Relação</span><span class="sxs-lookup"><span data-stu-id="d2692-110">Relationship</span></span> | <span data-ttu-id="d2692-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2692-111">Type</span></span>   |<span data-ttu-id="d2692-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2692-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2692-113">fill</span><span class="sxs-lookup"><span data-stu-id="d2692-113">fill</span></span>|[<span data-ttu-id="d2692-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="d2692-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="d2692-p101">Representa o formato de preenchimento de um gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2692-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d2692-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2692-117">JSON representation</span></span>

<span data-ttu-id="d2692-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2692-118">Here is a JSON representation of the resource.</span></span>

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