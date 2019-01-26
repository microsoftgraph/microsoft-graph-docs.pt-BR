---
title: Tipo de recurso ChartFont
description: Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 7e9815d5d6d9bf7e7b0ef4ae97881e12c7ba9181
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573624"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="95847-103">Tipo de recurso ChartFont</span><span class="sxs-lookup"><span data-stu-id="95847-103">ChartFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95847-104">Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="95847-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="95847-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="95847-105">Methods</span></span>

| <span data-ttu-id="95847-106">Método</span><span class="sxs-lookup"><span data-stu-id="95847-106">Method</span></span>           | <span data-ttu-id="95847-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="95847-107">Return Type</span></span>    |<span data-ttu-id="95847-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="95847-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95847-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="95847-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="95847-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="95847-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="95847-111">Leia as propriedades e os relacionamentos do objeto chartFont.</span><span class="sxs-lookup"><span data-stu-id="95847-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="95847-112">Update</span><span class="sxs-lookup"><span data-stu-id="95847-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="95847-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="95847-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="95847-114">Atualize o objeto ChartFont.</span><span class="sxs-lookup"><span data-stu-id="95847-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="95847-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95847-115">Properties</span></span>
| <span data-ttu-id="95847-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95847-116">Property</span></span>     | <span data-ttu-id="95847-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="95847-117">Type</span></span>   |<span data-ttu-id="95847-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="95847-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95847-119">bold</span><span class="sxs-lookup"><span data-stu-id="95847-119">bold</span></span>|<span data-ttu-id="95847-120">booliano</span><span class="sxs-lookup"><span data-stu-id="95847-120">boolean</span></span>|<span data-ttu-id="95847-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="95847-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="95847-122">color</span><span class="sxs-lookup"><span data-stu-id="95847-122">color</span></span>|<span data-ttu-id="95847-123">string</span><span class="sxs-lookup"><span data-stu-id="95847-123">string</span></span>|<span data-ttu-id="95847-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="95847-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="95847-127">italic</span><span class="sxs-lookup"><span data-stu-id="95847-127">italic</span></span>|<span data-ttu-id="95847-128">booliano</span><span class="sxs-lookup"><span data-stu-id="95847-128">boolean</span></span>|<span data-ttu-id="95847-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="95847-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="95847-130">name</span><span class="sxs-lookup"><span data-stu-id="95847-130">name</span></span>|<span data-ttu-id="95847-131">string</span><span class="sxs-lookup"><span data-stu-id="95847-131">string</span></span>|<span data-ttu-id="95847-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="95847-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="95847-133">size</span><span class="sxs-lookup"><span data-stu-id="95847-133">size</span></span>|<span data-ttu-id="95847-134">Double</span><span class="sxs-lookup"><span data-stu-id="95847-134">double</span></span>|<span data-ttu-id="95847-135">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="95847-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="95847-136">underline</span><span class="sxs-lookup"><span data-stu-id="95847-136">underline</span></span>|<span data-ttu-id="95847-137">string</span><span class="sxs-lookup"><span data-stu-id="95847-137">string</span></span>|<span data-ttu-id="95847-138">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="95847-138">Type of underline applied to the font.</span></span> <span data-ttu-id="95847-139">Os valores possíveis são: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="95847-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95847-140">Relações</span><span class="sxs-lookup"><span data-stu-id="95847-140">Relationships</span></span>
<span data-ttu-id="95847-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95847-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="95847-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95847-142">JSON representation</span></span>

<span data-ttu-id="95847-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95847-143">Here is a JSON representation of the resource.</span></span>

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
