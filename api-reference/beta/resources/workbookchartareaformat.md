---
title: tipo de recurso workbookChartAreaFormat
description: Encapsula as propriedades de formato da área de gráfico geral.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 69183153f066ba2b3521ec1519babb991491431e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519397"
---
# <a name="workbookchartareaformat-resource-type"></a><span data-ttu-id="7d691-103">tipo de recurso workbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="7d691-103">workbookChartAreaFormat resource type</span></span>

<span data-ttu-id="7d691-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7d691-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d691-105">Encapsula as propriedades de formato da área de gráfico geral.</span><span class="sxs-lookup"><span data-stu-id="7d691-105">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="7d691-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d691-106">Methods</span></span>
<span data-ttu-id="7d691-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d691-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="7d691-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d691-108">Properties</span></span>
<span data-ttu-id="7d691-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7d691-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7d691-110">Relações</span><span class="sxs-lookup"><span data-stu-id="7d691-110">Relationships</span></span>
| <span data-ttu-id="7d691-111">Relação</span><span class="sxs-lookup"><span data-stu-id="7d691-111">Relationship</span></span> | <span data-ttu-id="7d691-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d691-112">Type</span></span>   |<span data-ttu-id="7d691-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d691-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d691-114">fill</span><span class="sxs-lookup"><span data-stu-id="7d691-114">fill</span></span>|[<span data-ttu-id="7d691-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="7d691-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="7d691-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d691-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="7d691-118">font</span><span class="sxs-lookup"><span data-stu-id="7d691-118">font</span></span>|[<span data-ttu-id="7d691-119">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="7d691-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="7d691-120">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="7d691-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="7d691-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d691-121">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d691-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d691-122">JSON representation</span></span>

<span data-ttu-id="7d691-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d691-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
  "suppressions": []
}
-->
