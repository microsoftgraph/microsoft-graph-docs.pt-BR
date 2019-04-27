---
title: tipo de recurso workbookChartTitleFormat
description: Abrange as propriedades de formatação do título do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3827b44ae24a63f8fe048575633cc3b5508ac300
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348518"
---
# <a name="workbookcharttitleformat-resource-type"></a><span data-ttu-id="f2a12-103">tipo de recurso workbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="f2a12-103">workbookChartTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2a12-104">Abrange as propriedades de formatação do título do gráfico.</span><span class="sxs-lookup"><span data-stu-id="f2a12-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="f2a12-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2a12-105">Methods</span></span>
<span data-ttu-id="f2a12-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2a12-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="f2a12-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2a12-107">Properties</span></span>
<span data-ttu-id="f2a12-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f2a12-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f2a12-109">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="f2a12-109">Relationships</span></span>
| <span data-ttu-id="f2a12-110">Relação</span><span class="sxs-lookup"><span data-stu-id="f2a12-110">Relationship</span></span> | <span data-ttu-id="f2a12-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2a12-111">Type</span></span>   |<span data-ttu-id="f2a12-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2a12-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2a12-113">fill</span><span class="sxs-lookup"><span data-stu-id="f2a12-113">fill</span></span>|[<span data-ttu-id="f2a12-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="f2a12-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="f2a12-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2a12-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="f2a12-117">font</span><span class="sxs-lookup"><span data-stu-id="f2a12-117">font</span></span>|[<span data-ttu-id="f2a12-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="f2a12-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="f2a12-119">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="f2a12-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="f2a12-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2a12-120">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="f2a12-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2a12-121">JSON representation</span></span>

<span data-ttu-id="f2a12-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2a12-122">Here is a JSON representation of the resource.</span></span>

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
