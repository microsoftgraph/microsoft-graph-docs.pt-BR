---
title: Tipo de recurso ChartAreaFormat
description: Encapsula as propriedades de formato da área de gráfico geral.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a447b604807f3ae223445db953d45928eda9f36b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569386"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="c907a-103">Tipo de recurso ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="c907a-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="c907a-104">Encapsula as propriedades de formato da área de gráfico geral.</span><span class="sxs-lookup"><span data-stu-id="c907a-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="c907a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c907a-105">Methods</span></span>
<span data-ttu-id="c907a-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c907a-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c907a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c907a-107">Properties</span></span>
<span data-ttu-id="c907a-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c907a-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c907a-109">Relações</span><span class="sxs-lookup"><span data-stu-id="c907a-109">Relationships</span></span>
| <span data-ttu-id="c907a-110">Relação</span><span class="sxs-lookup"><span data-stu-id="c907a-110">Relationship</span></span> | <span data-ttu-id="c907a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c907a-111">Type</span></span>   |<span data-ttu-id="c907a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c907a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c907a-113">fill</span><span class="sxs-lookup"><span data-stu-id="c907a-113">fill</span></span>|[<span data-ttu-id="c907a-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="c907a-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="c907a-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c907a-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="c907a-117">font</span><span class="sxs-lookup"><span data-stu-id="c907a-117">font</span></span>|[<span data-ttu-id="c907a-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c907a-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="c907a-119">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="c907a-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="c907a-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c907a-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c907a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c907a-121">JSON representation</span></span>

<span data-ttu-id="c907a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c907a-122">Here is a JSON representation of the resource.</span></span>

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
