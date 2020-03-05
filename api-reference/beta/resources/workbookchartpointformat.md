---
title: tipo de recurso workbookChartPointFormat
description: Representa um objeto de formatação para os pontos do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9e947fa02624f2c24ea6433dc2e62eb0da218308
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519278"
---
# <a name="workbookchartpointformat-resource-type"></a><span data-ttu-id="0df6a-103">tipo de recurso workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="0df6a-103">workbookChartPointFormat resource type</span></span>

<span data-ttu-id="0df6a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0df6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df6a-105">Representa um objeto de formatação para os pontos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="0df6a-105">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="0df6a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0df6a-106">Methods</span></span>
<span data-ttu-id="0df6a-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0df6a-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="0df6a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0df6a-108">Properties</span></span>
<span data-ttu-id="0df6a-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0df6a-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0df6a-110">Relações</span><span class="sxs-lookup"><span data-stu-id="0df6a-110">Relationships</span></span>
| <span data-ttu-id="0df6a-111">Relação</span><span class="sxs-lookup"><span data-stu-id="0df6a-111">Relationship</span></span> | <span data-ttu-id="0df6a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="0df6a-112">Type</span></span>   |<span data-ttu-id="0df6a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0df6a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0df6a-114">fill</span><span class="sxs-lookup"><span data-stu-id="0df6a-114">fill</span></span>|[<span data-ttu-id="0df6a-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="0df6a-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="0df6a-116">Representa o formato de preenchimento de um gráfico, que inclui informações sobre a formatação da tela de fundo.</span><span class="sxs-lookup"><span data-stu-id="0df6a-116">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="0df6a-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0df6a-117">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0df6a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0df6a-118">JSON representation</span></span>

<span data-ttu-id="0df6a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0df6a-119">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
