---
title: Tipo de recurso ChartAreaFormat
description: Encapsula as propriedades de formato da área de gráfico geral.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ee39e1fc58fe604ff24433dcb540b44e22bb3ee9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033002"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="41a31-103">Tipo de recurso ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="41a31-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="41a31-104">Encapsula as propriedades de formato da área de gráfico geral.</span><span class="sxs-lookup"><span data-stu-id="41a31-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="41a31-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="41a31-105">Methods</span></span>
<span data-ttu-id="41a31-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41a31-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="41a31-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41a31-107">Properties</span></span>
<span data-ttu-id="41a31-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="41a31-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="41a31-109">Relações</span><span class="sxs-lookup"><span data-stu-id="41a31-109">Relationships</span></span>
| <span data-ttu-id="41a31-110">Relação</span><span class="sxs-lookup"><span data-stu-id="41a31-110">Relationship</span></span> | <span data-ttu-id="41a31-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="41a31-111">Type</span></span>   |<span data-ttu-id="41a31-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="41a31-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41a31-113">fill</span><span class="sxs-lookup"><span data-stu-id="41a31-113">fill</span></span>|[<span data-ttu-id="41a31-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="41a31-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="41a31-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41a31-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="41a31-117">font</span><span class="sxs-lookup"><span data-stu-id="41a31-117">font</span></span>|[<span data-ttu-id="41a31-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="41a31-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="41a31-119">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="41a31-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="41a31-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41a31-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41a31-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41a31-121">JSON representation</span></span>

<span data-ttu-id="41a31-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41a31-122">Here is a JSON representation of the resource.</span></span>

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
