---
title: Tipo de recurso ChartPointFormat
description: Representa um objeto de formatação para os pontos do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c71b7158b7ba3cef208fb6bf983d077c9474e77c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533105"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="df4fd-103">Tipo de recurso ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="df4fd-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="df4fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df4fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df4fd-105">Representa um objeto de formatação para os pontos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="df4fd-105">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="df4fd-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="df4fd-106">Methods</span></span>
<span data-ttu-id="df4fd-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df4fd-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="df4fd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df4fd-108">Properties</span></span>
<span data-ttu-id="df4fd-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="df4fd-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="df4fd-110">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="df4fd-110">Relationships</span></span>
| <span data-ttu-id="df4fd-111">Relação</span><span class="sxs-lookup"><span data-stu-id="df4fd-111">Relationship</span></span> | <span data-ttu-id="df4fd-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="df4fd-112">Type</span></span>   |<span data-ttu-id="df4fd-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="df4fd-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df4fd-114">fill</span><span class="sxs-lookup"><span data-stu-id="df4fd-114">fill</span></span>|[<span data-ttu-id="df4fd-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="df4fd-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="df4fd-116">Representa o formato de preenchimento de um gráfico, que inclui informações sobre a formatação da tela de fundo.</span><span class="sxs-lookup"><span data-stu-id="df4fd-116">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="df4fd-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df4fd-117">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="df4fd-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df4fd-118">JSON representation</span></span>

<span data-ttu-id="df4fd-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df4fd-119">Here is a JSON representation of the resource.</span></span>

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
