---
title: Tipo de recurso ChartPointFormat
description: Representa um objeto de formatação para os pontos do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c1b0a4a7d9076771da11061723f275079d429cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569064"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="11d18-103">Tipo de recurso ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="11d18-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="11d18-104">Representa um objeto de formatação para os pontos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="11d18-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="11d18-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="11d18-105">Methods</span></span>
<span data-ttu-id="11d18-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11d18-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="11d18-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11d18-107">Properties</span></span>
<span data-ttu-id="11d18-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="11d18-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="11d18-109">Relações</span><span class="sxs-lookup"><span data-stu-id="11d18-109">Relationships</span></span>
| <span data-ttu-id="11d18-110">Relação</span><span class="sxs-lookup"><span data-stu-id="11d18-110">Relationship</span></span> | <span data-ttu-id="11d18-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="11d18-111">Type</span></span>   |<span data-ttu-id="11d18-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="11d18-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11d18-113">fill</span><span class="sxs-lookup"><span data-stu-id="11d18-113">fill</span></span>|[<span data-ttu-id="11d18-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="11d18-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="11d18-115">Representa o formato de preenchimento de um gráfico, que inclui informações sobre a formatação da tela de fundo.</span><span class="sxs-lookup"><span data-stu-id="11d18-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="11d18-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11d18-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="11d18-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11d18-117">JSON representation</span></span>

<span data-ttu-id="11d18-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11d18-118">Here is a JSON representation of the resource.</span></span>

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
