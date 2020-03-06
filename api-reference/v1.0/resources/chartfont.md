---
title: Tipo de recurso ChartFont
description: Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1768e40edde1d02c109e77c7e7ca3c2dd0ffdafa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531852"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="c1597-103">Tipo de recurso ChartFont</span><span class="sxs-lookup"><span data-stu-id="c1597-103">ChartFont resource type</span></span>

<span data-ttu-id="c1597-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1597-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1597-105">Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="c1597-105">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="c1597-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c1597-106">Methods</span></span>

| <span data-ttu-id="c1597-107">Método</span><span class="sxs-lookup"><span data-stu-id="c1597-107">Method</span></span>           | <span data-ttu-id="c1597-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c1597-108">Return Type</span></span>    |<span data-ttu-id="c1597-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1597-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1597-110">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="c1597-110">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="c1597-111">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c1597-111">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="c1597-112">Leia as propriedades e os relacionamentos do objeto chartFont.</span><span class="sxs-lookup"><span data-stu-id="c1597-112">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="c1597-113">Update</span><span class="sxs-lookup"><span data-stu-id="c1597-113">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="c1597-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c1597-114">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="c1597-115">Atualize o objeto ChartFont.</span><span class="sxs-lookup"><span data-stu-id="c1597-115">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c1597-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1597-116">Properties</span></span>
| <span data-ttu-id="c1597-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1597-117">Property</span></span>     | <span data-ttu-id="c1597-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1597-118">Type</span></span>   |<span data-ttu-id="c1597-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1597-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1597-120">bold</span><span class="sxs-lookup"><span data-stu-id="c1597-120">bold</span></span>|<span data-ttu-id="c1597-121">booliano</span><span class="sxs-lookup"><span data-stu-id="c1597-121">boolean</span></span>|<span data-ttu-id="c1597-122">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="c1597-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="c1597-123">color</span><span class="sxs-lookup"><span data-stu-id="c1597-123">color</span></span>|<span data-ttu-id="c1597-124">string</span><span class="sxs-lookup"><span data-stu-id="c1597-124">string</span></span>|<span data-ttu-id="c1597-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="c1597-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="c1597-128">italic</span><span class="sxs-lookup"><span data-stu-id="c1597-128">italic</span></span>|<span data-ttu-id="c1597-129">booliano</span><span class="sxs-lookup"><span data-stu-id="c1597-129">boolean</span></span>|<span data-ttu-id="c1597-130">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="c1597-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="c1597-131">nome</span><span class="sxs-lookup"><span data-stu-id="c1597-131">name</span></span>|<span data-ttu-id="c1597-132">string</span><span class="sxs-lookup"><span data-stu-id="c1597-132">string</span></span>|<span data-ttu-id="c1597-133">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="c1597-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="c1597-134">size</span><span class="sxs-lookup"><span data-stu-id="c1597-134">size</span></span>|<span data-ttu-id="c1597-135">Double</span><span class="sxs-lookup"><span data-stu-id="c1597-135">double</span></span>|<span data-ttu-id="c1597-136">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="c1597-136">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="c1597-137">underline</span><span class="sxs-lookup"><span data-stu-id="c1597-137">underline</span></span>|<span data-ttu-id="c1597-138">string</span><span class="sxs-lookup"><span data-stu-id="c1597-138">string</span></span>|<span data-ttu-id="c1597-139">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="c1597-139">Type of underline applied to the font.</span></span> <span data-ttu-id="c1597-140">Os valores possíveis são: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="c1597-140">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1597-141">Relações</span><span class="sxs-lookup"><span data-stu-id="c1597-141">Relationships</span></span>
<span data-ttu-id="c1597-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1597-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c1597-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1597-143">JSON representation</span></span>

<span data-ttu-id="c1597-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1597-144">Here is a JSON representation of the resource.</span></span>

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
