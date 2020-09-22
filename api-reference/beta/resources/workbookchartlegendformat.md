---
title: tipo de recurso workbookChartLegendFormat
description: Encapsula as propriedades de formato de uma legenda de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d62fef73879fc54eb9d459db2c550cbe91153f05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971451"
---
# <a name="workbookchartlegendformat-resource-type"></a><span data-ttu-id="026a2-103">tipo de recurso workbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="026a2-103">workbookChartLegendFormat resource type</span></span>

<span data-ttu-id="026a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="026a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="026a2-105">Encapsula as propriedades de formato de uma legenda de gráfico.</span><span class="sxs-lookup"><span data-stu-id="026a2-105">Encapsulates the format properties of a chart legend.</span></span>

## <a name="methods"></a><span data-ttu-id="026a2-106">Methods</span><span class="sxs-lookup"><span data-stu-id="026a2-106">Methods</span></span>
<span data-ttu-id="026a2-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="026a2-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="026a2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="026a2-108">Properties</span></span>
<span data-ttu-id="026a2-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="026a2-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="026a2-110">Relações</span><span class="sxs-lookup"><span data-stu-id="026a2-110">Relationships</span></span>
| <span data-ttu-id="026a2-111">Relação</span><span class="sxs-lookup"><span data-stu-id="026a2-111">Relationship</span></span> | <span data-ttu-id="026a2-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="026a2-112">Type</span></span>   |<span data-ttu-id="026a2-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="026a2-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="026a2-114">fill</span><span class="sxs-lookup"><span data-stu-id="026a2-114">fill</span></span>|[<span data-ttu-id="026a2-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="026a2-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="026a2-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="026a2-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="026a2-118">fonte</span><span class="sxs-lookup"><span data-stu-id="026a2-118">font</span></span>|[<span data-ttu-id="026a2-119">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="026a2-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="026a2-120">Representa os atributos de fonte, como nome da fonte, tamanho da fonte, cor, etc. de uma legenda do gráfico.</span><span class="sxs-lookup"><span data-stu-id="026a2-120">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="026a2-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="026a2-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="026a2-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="026a2-122">JSON representation</span></span>

<span data-ttu-id="026a2-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="026a2-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "workbookChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


