---
title: tipo de recurso workbookChartTitleFormat
description: Abrange as propriedades de formatação do título do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b7235e8b1d9d5867b47c66a462e9c94b86a528dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519250"
---
# <a name="workbookcharttitleformat-resource-type"></a><span data-ttu-id="d1bf0-103">tipo de recurso workbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="d1bf0-103">workbookChartTitleFormat resource type</span></span>

<span data-ttu-id="d1bf0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d1bf0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1bf0-105">Abrange as propriedades de formatação do título do gráfico.</span><span class="sxs-lookup"><span data-stu-id="d1bf0-105">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="d1bf0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d1bf0-106">Methods</span></span>
<span data-ttu-id="d1bf0-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1bf0-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="d1bf0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1bf0-108">Properties</span></span>
<span data-ttu-id="d1bf0-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d1bf0-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d1bf0-110">Relações</span><span class="sxs-lookup"><span data-stu-id="d1bf0-110">Relationships</span></span>
| <span data-ttu-id="d1bf0-111">Relação</span><span class="sxs-lookup"><span data-stu-id="d1bf0-111">Relationship</span></span> | <span data-ttu-id="d1bf0-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1bf0-112">Type</span></span>   |<span data-ttu-id="d1bf0-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1bf0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1bf0-114">fill</span><span class="sxs-lookup"><span data-stu-id="d1bf0-114">fill</span></span>|[<span data-ttu-id="d1bf0-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="d1bf0-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="d1bf0-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1bf0-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="d1bf0-118">font</span><span class="sxs-lookup"><span data-stu-id="d1bf0-118">font</span></span>|[<span data-ttu-id="d1bf0-119">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d1bf0-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="d1bf0-120">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="d1bf0-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="d1bf0-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1bf0-121">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="d1bf0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1bf0-122">JSON representation</span></span>

<span data-ttu-id="d1bf0-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1bf0-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
  "description": "workbookChartTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
