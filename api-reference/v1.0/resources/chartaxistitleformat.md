---
title: Tipo de recurso ChartAxisTitleFormat
description: Representa a formatação do título do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3ae74b7353a0b4198b42a04fdd420eb3447d4c11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029845"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="88168-103">Tipo de recurso ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="88168-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="88168-104">Representa a formatação do título do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="88168-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="88168-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="88168-105">Methods</span></span>
<span data-ttu-id="88168-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88168-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="88168-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88168-107">Properties</span></span>
<span data-ttu-id="88168-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="88168-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="88168-109">Relações</span><span class="sxs-lookup"><span data-stu-id="88168-109">Relationships</span></span>
| <span data-ttu-id="88168-110">Relação</span><span class="sxs-lookup"><span data-stu-id="88168-110">Relationship</span></span> | <span data-ttu-id="88168-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="88168-111">Type</span></span>   |<span data-ttu-id="88168-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="88168-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88168-113">font</span><span class="sxs-lookup"><span data-stu-id="88168-113">font</span></span>|[<span data-ttu-id="88168-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="88168-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="88168-115">Representa os atributos de fonte, como nome, tamanho, cor, etc., do objeto do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="88168-115">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="88168-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="88168-116">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88168-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88168-117">JSON representation</span></span>

<span data-ttu-id="88168-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88168-118">Here is a JSON representation of the resource.</span></span>

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
