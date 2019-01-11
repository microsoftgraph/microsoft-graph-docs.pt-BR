---
title: Tipo de recurso ChartFont
description: Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
ms.openlocfilehash: 9b2d6e07f5049449d71be45b41585ed3bd300b7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850782"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="ff90f-103">Tipo de recurso ChartFont</span><span class="sxs-lookup"><span data-stu-id="ff90f-103">ChartFont resource type</span></span>

<span data-ttu-id="ff90f-104">Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="ff90f-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="ff90f-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ff90f-105">Methods</span></span>

| <span data-ttu-id="ff90f-106">Método</span><span class="sxs-lookup"><span data-stu-id="ff90f-106">Method</span></span>           | <span data-ttu-id="ff90f-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ff90f-107">Return Type</span></span>    |<span data-ttu-id="ff90f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff90f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff90f-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="ff90f-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="ff90f-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ff90f-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="ff90f-111">Leia as propriedades e os relacionamentos do objeto chartFont.</span><span class="sxs-lookup"><span data-stu-id="ff90f-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="ff90f-112">Update</span><span class="sxs-lookup"><span data-stu-id="ff90f-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="ff90f-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ff90f-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="ff90f-114">Atualize o objeto ChartFont.</span><span class="sxs-lookup"><span data-stu-id="ff90f-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff90f-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff90f-115">Properties</span></span>
| <span data-ttu-id="ff90f-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff90f-116">Property</span></span>     | <span data-ttu-id="ff90f-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff90f-117">Type</span></span>   |<span data-ttu-id="ff90f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff90f-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff90f-119">bold</span><span class="sxs-lookup"><span data-stu-id="ff90f-119">bold</span></span>|<span data-ttu-id="ff90f-120">booliano</span><span class="sxs-lookup"><span data-stu-id="ff90f-120">boolean</span></span>|<span data-ttu-id="ff90f-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="ff90f-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="ff90f-122">color</span><span class="sxs-lookup"><span data-stu-id="ff90f-122">color</span></span>|<span data-ttu-id="ff90f-123">string</span><span class="sxs-lookup"><span data-stu-id="ff90f-123">string</span></span>|<span data-ttu-id="ff90f-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="ff90f-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="ff90f-127">italic</span><span class="sxs-lookup"><span data-stu-id="ff90f-127">italic</span></span>|<span data-ttu-id="ff90f-128">booliano</span><span class="sxs-lookup"><span data-stu-id="ff90f-128">boolean</span></span>|<span data-ttu-id="ff90f-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="ff90f-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="ff90f-130">name</span><span class="sxs-lookup"><span data-stu-id="ff90f-130">name</span></span>|<span data-ttu-id="ff90f-131">string</span><span class="sxs-lookup"><span data-stu-id="ff90f-131">string</span></span>|<span data-ttu-id="ff90f-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="ff90f-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="ff90f-133">size</span><span class="sxs-lookup"><span data-stu-id="ff90f-133">size</span></span>|<span data-ttu-id="ff90f-134">Double</span><span class="sxs-lookup"><span data-stu-id="ff90f-134">double</span></span>|<span data-ttu-id="ff90f-135">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="ff90f-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="ff90f-136">underline</span><span class="sxs-lookup"><span data-stu-id="ff90f-136">underline</span></span>|<span data-ttu-id="ff90f-137">string</span><span class="sxs-lookup"><span data-stu-id="ff90f-137">string</span></span>|<span data-ttu-id="ff90f-138">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="ff90f-138">Type of underline applied to the font.</span></span> <span data-ttu-id="ff90f-139">Os valores possíveis são: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="ff90f-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff90f-140">Relações</span><span class="sxs-lookup"><span data-stu-id="ff90f-140">Relationships</span></span>
<span data-ttu-id="ff90f-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff90f-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ff90f-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff90f-142">JSON representation</span></span>

<span data-ttu-id="ff90f-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff90f-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
