---
title: Tipo de recurso ChartFont
description: Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c507a966dc6b29e46935c5c77a85b557a84cc69c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543714"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="e0491-103">Tipo de recurso ChartFont</span><span class="sxs-lookup"><span data-stu-id="e0491-103">ChartFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0491-104">Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="e0491-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="e0491-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e0491-105">Methods</span></span>

| <span data-ttu-id="e0491-106">Método</span><span class="sxs-lookup"><span data-stu-id="e0491-106">Method</span></span>           | <span data-ttu-id="e0491-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e0491-107">Return Type</span></span>    |<span data-ttu-id="e0491-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0491-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0491-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="e0491-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="e0491-110">ChartFont</span><span class="sxs-lookup"><span data-stu-id="e0491-110">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="e0491-111">Leia as propriedades e os relacionamentos do objeto chartFont.</span><span class="sxs-lookup"><span data-stu-id="e0491-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="e0491-112">Update</span><span class="sxs-lookup"><span data-stu-id="e0491-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="e0491-113">ChartFont</span><span class="sxs-lookup"><span data-stu-id="e0491-113">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="e0491-114">Atualize o objeto ChartFont.</span><span class="sxs-lookup"><span data-stu-id="e0491-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e0491-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0491-115">Properties</span></span>
| <span data-ttu-id="e0491-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0491-116">Property</span></span>     | <span data-ttu-id="e0491-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0491-117">Type</span></span>   |<span data-ttu-id="e0491-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0491-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0491-119">bold</span><span class="sxs-lookup"><span data-stu-id="e0491-119">bold</span></span>|<span data-ttu-id="e0491-120">booliano</span><span class="sxs-lookup"><span data-stu-id="e0491-120">boolean</span></span>|<span data-ttu-id="e0491-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="e0491-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="e0491-122">color</span><span class="sxs-lookup"><span data-stu-id="e0491-122">color</span></span>|<span data-ttu-id="e0491-123">string</span><span class="sxs-lookup"><span data-stu-id="e0491-123">string</span></span>|<span data-ttu-id="e0491-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="e0491-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="e0491-127">italic</span><span class="sxs-lookup"><span data-stu-id="e0491-127">italic</span></span>|<span data-ttu-id="e0491-128">booliano</span><span class="sxs-lookup"><span data-stu-id="e0491-128">boolean</span></span>|<span data-ttu-id="e0491-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="e0491-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="e0491-130">name</span><span class="sxs-lookup"><span data-stu-id="e0491-130">name</span></span>|<span data-ttu-id="e0491-131">string</span><span class="sxs-lookup"><span data-stu-id="e0491-131">string</span></span>|<span data-ttu-id="e0491-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="e0491-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="e0491-133">size</span><span class="sxs-lookup"><span data-stu-id="e0491-133">size</span></span>|<span data-ttu-id="e0491-134">Double</span><span class="sxs-lookup"><span data-stu-id="e0491-134">double</span></span>|<span data-ttu-id="e0491-135">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="e0491-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="e0491-136">underline</span><span class="sxs-lookup"><span data-stu-id="e0491-136">underline</span></span>|<span data-ttu-id="e0491-137">string</span><span class="sxs-lookup"><span data-stu-id="e0491-137">string</span></span>|<span data-ttu-id="e0491-p102">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None` e `Single`.</span><span class="sxs-lookup"><span data-stu-id="e0491-p102">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0491-140">Relações</span><span class="sxs-lookup"><span data-stu-id="e0491-140">Relationships</span></span>
<span data-ttu-id="e0491-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0491-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e0491-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0491-142">JSON representation</span></span>

<span data-ttu-id="e0491-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0491-143">Here is a JSON representation of the resource.</span></span>

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
