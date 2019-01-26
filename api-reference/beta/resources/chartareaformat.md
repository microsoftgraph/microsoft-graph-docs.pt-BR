---
title: Tipo de recurso ChartAreaFormat
description: Abrange as propriedades de formatação da área geral do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 637b1a886c237d6ad1f6432bf2d183c97005f981
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570852"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="97a72-103">Tipo de recurso ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="97a72-103">ChartAreaFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97a72-104">Abrange as propriedades de formatação da área geral do gráfico.</span><span class="sxs-lookup"><span data-stu-id="97a72-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="97a72-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="97a72-105">Methods</span></span>
<span data-ttu-id="97a72-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97a72-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="97a72-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97a72-107">Properties</span></span>
<span data-ttu-id="97a72-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97a72-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="97a72-109">Relações</span><span class="sxs-lookup"><span data-stu-id="97a72-109">Relationships</span></span>
| <span data-ttu-id="97a72-110">Relação</span><span class="sxs-lookup"><span data-stu-id="97a72-110">Relationship</span></span> | <span data-ttu-id="97a72-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="97a72-111">Type</span></span>   |<span data-ttu-id="97a72-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="97a72-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97a72-113">fill</span><span class="sxs-lookup"><span data-stu-id="97a72-113">fill</span></span>|[<span data-ttu-id="97a72-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="97a72-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="97a72-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97a72-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="97a72-117">font</span><span class="sxs-lookup"><span data-stu-id="97a72-117">font</span></span>|[<span data-ttu-id="97a72-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="97a72-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="97a72-p102">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97a72-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97a72-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97a72-121">JSON representation</span></span>

<span data-ttu-id="97a72-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97a72-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartareaformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
