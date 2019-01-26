---
title: Tipo de recurso ChartTitleFormat
description: Abrange as propriedades de formatação do título do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7dd9400873234fd73ebe506a49caf6583d05b75b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574009"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="90ef6-103">Tipo de recurso ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="90ef6-103">ChartTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="methods"></a><span data-ttu-id="90ef6-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="90ef6-104">Methods</span></span>
<span data-ttu-id="90ef6-105">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90ef6-105">None</span></span>

## <a name="properties"></a><span data-ttu-id="90ef6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90ef6-106">Properties</span></span>
<span data-ttu-id="90ef6-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90ef6-107">None</span></span>

## <a name="relationships"></a><span data-ttu-id="90ef6-108">Relações</span><span class="sxs-lookup"><span data-stu-id="90ef6-108">Relationships</span></span>
| <span data-ttu-id="90ef6-109">Relação</span><span class="sxs-lookup"><span data-stu-id="90ef6-109">Relationship</span></span> | <span data-ttu-id="90ef6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="90ef6-110">Type</span></span>   |<span data-ttu-id="90ef6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ef6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90ef6-112">fill</span><span class="sxs-lookup"><span data-stu-id="90ef6-112">fill</span></span>|[<span data-ttu-id="90ef6-113">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="90ef6-113">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="90ef6-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90ef6-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="90ef6-116">font</span><span class="sxs-lookup"><span data-stu-id="90ef6-116">font</span></span>|[<span data-ttu-id="90ef6-117">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="90ef6-117">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="90ef6-p102">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90ef6-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="90ef6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90ef6-120">JSON representation</span></span>

<span data-ttu-id="90ef6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90ef6-121">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/charttitleformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
