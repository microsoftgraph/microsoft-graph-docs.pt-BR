---
title: Tipo de recurso ChartLineFormat
description: Abrange as opções de formatação dos elementos de linha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b4409eb18dab41d43adc038b702a65fa8d63e4de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517929"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="f530e-103">Tipo de recurso ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="f530e-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f530e-104">Abrange as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="f530e-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="f530e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f530e-105">Methods</span></span>

| <span data-ttu-id="f530e-106">Método</span><span class="sxs-lookup"><span data-stu-id="f530e-106">Method</span></span>           | <span data-ttu-id="f530e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f530e-107">Return Type</span></span>    |<span data-ttu-id="f530e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f530e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f530e-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="f530e-109">[Get ChartLineFormat](../api/chartlineformat-get.md)</span></span> | <span data-ttu-id="f530e-110">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="f530e-110">[ChartLineFormat](chartlineformat.md)</span></span> |<span data-ttu-id="f530e-111">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="f530e-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="f530e-112">Update</span><span class="sxs-lookup"><span data-stu-id="f530e-112">Update</span></span>](../api/chartlineformat-update.md) | <span data-ttu-id="f530e-113">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="f530e-113">[ChartLineFormat](chartlineformat.md)</span></span> |<span data-ttu-id="f530e-114">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="f530e-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="f530e-115">Clear</span><span class="sxs-lookup"><span data-stu-id="f530e-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="f530e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f530e-116">None</span></span>|<span data-ttu-id="f530e-117">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="f530e-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="f530e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f530e-118">Properties</span></span>
| <span data-ttu-id="f530e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f530e-119">Property</span></span>     | <span data-ttu-id="f530e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f530e-120">Type</span></span>   |<span data-ttu-id="f530e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f530e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f530e-122">color</span><span class="sxs-lookup"><span data-stu-id="f530e-122">color</span></span>|<span data-ttu-id="f530e-123">string</span><span class="sxs-lookup"><span data-stu-id="f530e-123">string</span></span>|<span data-ttu-id="f530e-124">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="f530e-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f530e-125">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="f530e-125">Relationships</span></span>
<span data-ttu-id="f530e-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f530e-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f530e-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f530e-127">JSON representation</span></span>

<span data-ttu-id="f530e-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f530e-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlineformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
