---
title: Tipo de recurso ChartFont
description: Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9241691296b93eb21e19e10b81f36e692fea0692
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032991"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="4984c-103">Tipo de recurso ChartFont</span><span class="sxs-lookup"><span data-stu-id="4984c-103">ChartFont resource type</span></span>

<span data-ttu-id="4984c-104">Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="4984c-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="4984c-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4984c-105">Methods</span></span>

| <span data-ttu-id="4984c-106">Método</span><span class="sxs-lookup"><span data-stu-id="4984c-106">Method</span></span>           | <span data-ttu-id="4984c-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4984c-107">Return Type</span></span>    |<span data-ttu-id="4984c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4984c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4984c-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="4984c-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="4984c-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="4984c-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="4984c-111">Leia as propriedades e os relacionamentos do objeto chartFont.</span><span class="sxs-lookup"><span data-stu-id="4984c-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="4984c-112">Update</span><span class="sxs-lookup"><span data-stu-id="4984c-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="4984c-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="4984c-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="4984c-114">Atualize o objeto ChartFont.</span><span class="sxs-lookup"><span data-stu-id="4984c-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4984c-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4984c-115">Properties</span></span>
| <span data-ttu-id="4984c-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4984c-116">Property</span></span>     | <span data-ttu-id="4984c-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="4984c-117">Type</span></span>   |<span data-ttu-id="4984c-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="4984c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4984c-119">bold</span><span class="sxs-lookup"><span data-stu-id="4984c-119">bold</span></span>|<span data-ttu-id="4984c-120">booliano</span><span class="sxs-lookup"><span data-stu-id="4984c-120">boolean</span></span>|<span data-ttu-id="4984c-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="4984c-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="4984c-122">color</span><span class="sxs-lookup"><span data-stu-id="4984c-122">color</span></span>|<span data-ttu-id="4984c-123">string</span><span class="sxs-lookup"><span data-stu-id="4984c-123">string</span></span>|<span data-ttu-id="4984c-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="4984c-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="4984c-127">italic</span><span class="sxs-lookup"><span data-stu-id="4984c-127">italic</span></span>|<span data-ttu-id="4984c-128">booliano</span><span class="sxs-lookup"><span data-stu-id="4984c-128">boolean</span></span>|<span data-ttu-id="4984c-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="4984c-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="4984c-130">name</span><span class="sxs-lookup"><span data-stu-id="4984c-130">name</span></span>|<span data-ttu-id="4984c-131">string</span><span class="sxs-lookup"><span data-stu-id="4984c-131">string</span></span>|<span data-ttu-id="4984c-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="4984c-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="4984c-133">size</span><span class="sxs-lookup"><span data-stu-id="4984c-133">size</span></span>|<span data-ttu-id="4984c-134">Double</span><span class="sxs-lookup"><span data-stu-id="4984c-134">double</span></span>|<span data-ttu-id="4984c-135">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="4984c-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="4984c-136">underline</span><span class="sxs-lookup"><span data-stu-id="4984c-136">underline</span></span>|<span data-ttu-id="4984c-137">string</span><span class="sxs-lookup"><span data-stu-id="4984c-137">string</span></span>|<span data-ttu-id="4984c-138">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="4984c-138">Type of underline applied to the font.</span></span> <span data-ttu-id="4984c-139">Os valores possíveis são: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="4984c-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4984c-140">Relações</span><span class="sxs-lookup"><span data-stu-id="4984c-140">Relationships</span></span>
<span data-ttu-id="4984c-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4984c-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4984c-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4984c-142">JSON representation</span></span>

<span data-ttu-id="4984c-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4984c-143">Here is a JSON representation of the resource.</span></span>

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
