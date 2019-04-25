---
title: Tipo de recurso ChartAxisTitleFormat
description: Representa a formatação do título do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26d305d8bd4a0059123f77bd86cbbf5fd01dcea7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569077"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="80a80-103">Tipo de recurso ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="80a80-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="80a80-104">Representa a formatação do título do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="80a80-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="80a80-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="80a80-105">Methods</span></span>
<span data-ttu-id="80a80-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80a80-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="80a80-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80a80-107">Properties</span></span>
<span data-ttu-id="80a80-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="80a80-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="80a80-109">Relações</span><span class="sxs-lookup"><span data-stu-id="80a80-109">Relationships</span></span>
| <span data-ttu-id="80a80-110">Relação</span><span class="sxs-lookup"><span data-stu-id="80a80-110">Relationship</span></span> | <span data-ttu-id="80a80-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="80a80-111">Type</span></span>   |<span data-ttu-id="80a80-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="80a80-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80a80-113">font</span><span class="sxs-lookup"><span data-stu-id="80a80-113">font</span></span>|[<span data-ttu-id="80a80-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="80a80-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="80a80-115">Representa os atributos de fonte, como nome, tamanho, cor, etc., do objeto do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="80a80-115">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="80a80-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80a80-116">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80a80-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80a80-117">JSON representation</span></span>

<span data-ttu-id="80a80-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80a80-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
