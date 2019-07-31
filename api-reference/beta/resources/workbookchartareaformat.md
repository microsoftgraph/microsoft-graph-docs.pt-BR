---
title: tipo de recurso workbookChartAreaFormat
description: Encapsula as propriedades de formato da área de gráfico geral.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: afb3bc154295495893da4f0b183d1737c3b3d090
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964092"
---
# <a name="workbookchartareaformat-resource-type"></a><span data-ttu-id="61359-103">tipo de recurso workbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="61359-103">workbookChartAreaFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61359-104">Encapsula as propriedades de formato da área de gráfico geral.</span><span class="sxs-lookup"><span data-stu-id="61359-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="61359-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="61359-105">Methods</span></span>
<span data-ttu-id="61359-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61359-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="61359-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61359-107">Properties</span></span>
<span data-ttu-id="61359-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="61359-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="61359-109">Relações</span><span class="sxs-lookup"><span data-stu-id="61359-109">Relationships</span></span>
| <span data-ttu-id="61359-110">Relação</span><span class="sxs-lookup"><span data-stu-id="61359-110">Relationship</span></span> | <span data-ttu-id="61359-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="61359-111">Type</span></span>   |<span data-ttu-id="61359-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="61359-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61359-113">fill</span><span class="sxs-lookup"><span data-stu-id="61359-113">fill</span></span>|[<span data-ttu-id="61359-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="61359-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="61359-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61359-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="61359-117">font</span><span class="sxs-lookup"><span data-stu-id="61359-117">font</span></span>|[<span data-ttu-id="61359-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="61359-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="61359-119">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="61359-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="61359-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61359-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61359-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61359-121">JSON representation</span></span>

<span data-ttu-id="61359-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61359-122">Here is a JSON representation of the resource.</span></span>

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
