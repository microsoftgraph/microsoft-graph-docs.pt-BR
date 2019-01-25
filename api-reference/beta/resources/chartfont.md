---
title: Tipo de recurso ChartFont
description: Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c507a966dc6b29e46935c5c77a85b557a84cc69c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518321"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="b3b58-103">Tipo de recurso ChartFont</span><span class="sxs-lookup"><span data-stu-id="b3b58-103">ChartFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3b58-104">Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="b3b58-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="b3b58-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3b58-105">Methods</span></span>

| <span data-ttu-id="b3b58-106">Método</span><span class="sxs-lookup"><span data-stu-id="b3b58-106">Method</span></span>           | <span data-ttu-id="b3b58-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3b58-107">Return Type</span></span>    |<span data-ttu-id="b3b58-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3b58-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3b58-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="b3b58-109">[Get ChartFont](../api/chartfont-get.md)</span></span> | <span data-ttu-id="b3b58-110">ChartFont</span><span class="sxs-lookup"><span data-stu-id="b3b58-110">[ChartFont](chartfont.md)</span></span> |<span data-ttu-id="b3b58-111">Leia as propriedades e os relacionamentos do objeto chartFont.</span><span class="sxs-lookup"><span data-stu-id="b3b58-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="b3b58-112">Update</span><span class="sxs-lookup"><span data-stu-id="b3b58-112">Update</span></span>](../api/chartfont-update.md) | <span data-ttu-id="b3b58-113">ChartFont</span><span class="sxs-lookup"><span data-stu-id="b3b58-113">[ChartFont](chartfont.md)</span></span>   |<span data-ttu-id="b3b58-114">Atualize o objeto ChartFont.</span><span class="sxs-lookup"><span data-stu-id="b3b58-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b3b58-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3b58-115">Properties</span></span>
| <span data-ttu-id="b3b58-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3b58-116">Property</span></span>     | <span data-ttu-id="b3b58-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3b58-117">Type</span></span>   |<span data-ttu-id="b3b58-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3b58-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3b58-119">bold</span><span class="sxs-lookup"><span data-stu-id="b3b58-119">bold</span></span>|<span data-ttu-id="b3b58-120">booliano</span><span class="sxs-lookup"><span data-stu-id="b3b58-120">boolean</span></span>|<span data-ttu-id="b3b58-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="b3b58-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="b3b58-122">color</span><span class="sxs-lookup"><span data-stu-id="b3b58-122">color</span></span>|<span data-ttu-id="b3b58-123">string</span><span class="sxs-lookup"><span data-stu-id="b3b58-123">string</span></span>|<span data-ttu-id="b3b58-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="b3b58-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="b3b58-127">italic</span><span class="sxs-lookup"><span data-stu-id="b3b58-127">italic</span></span>|<span data-ttu-id="b3b58-128">booliano</span><span class="sxs-lookup"><span data-stu-id="b3b58-128">boolean</span></span>|<span data-ttu-id="b3b58-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="b3b58-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="b3b58-130">name</span><span class="sxs-lookup"><span data-stu-id="b3b58-130">name</span></span>|<span data-ttu-id="b3b58-131">string</span><span class="sxs-lookup"><span data-stu-id="b3b58-131">string</span></span>|<span data-ttu-id="b3b58-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="b3b58-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="b3b58-133">size</span><span class="sxs-lookup"><span data-stu-id="b3b58-133">size</span></span>|<span data-ttu-id="b3b58-134">Double</span><span class="sxs-lookup"><span data-stu-id="b3b58-134">double</span></span>|<span data-ttu-id="b3b58-135">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="b3b58-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="b3b58-136">underline</span><span class="sxs-lookup"><span data-stu-id="b3b58-136">underline</span></span>|<span data-ttu-id="b3b58-137">string</span><span class="sxs-lookup"><span data-stu-id="b3b58-137">string</span></span>|<span data-ttu-id="b3b58-p102">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None` e `Single`.</span><span class="sxs-lookup"><span data-stu-id="b3b58-p102">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3b58-140">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="b3b58-140">Relationships</span></span>
<span data-ttu-id="b3b58-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3b58-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b3b58-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3b58-142">JSON representation</span></span>

<span data-ttu-id="b3b58-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3b58-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartfont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
