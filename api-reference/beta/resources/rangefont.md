---
title: Tipo de recurso RangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2dee07b7d2573081650bdd15799e4884c774e171
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640158"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="2dddd-103">Tipo de recurso RangeFont</span><span class="sxs-lookup"><span data-stu-id="2dddd-103">RangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dddd-104">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.</span><span class="sxs-lookup"><span data-stu-id="2dddd-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="2dddd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2dddd-105">Methods</span></span>

| <span data-ttu-id="2dddd-106">Método</span><span class="sxs-lookup"><span data-stu-id="2dddd-106">Method</span></span>           | <span data-ttu-id="2dddd-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2dddd-107">Return Type</span></span>    |<span data-ttu-id="2dddd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dddd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2dddd-109">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="2dddd-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="2dddd-110">RangeFont</span><span class="sxs-lookup"><span data-stu-id="2dddd-110">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="2dddd-111">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="2dddd-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="2dddd-112">Update</span><span class="sxs-lookup"><span data-stu-id="2dddd-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="2dddd-113">RangeFont</span><span class="sxs-lookup"><span data-stu-id="2dddd-113">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="2dddd-114">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="2dddd-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2dddd-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2dddd-115">Properties</span></span>
| <span data-ttu-id="2dddd-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2dddd-116">Property</span></span>     | <span data-ttu-id="2dddd-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dddd-117">Type</span></span>   |<span data-ttu-id="2dddd-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dddd-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dddd-119">bold</span><span class="sxs-lookup"><span data-stu-id="2dddd-119">bold</span></span>|<span data-ttu-id="2dddd-120">booliano</span><span class="sxs-lookup"><span data-stu-id="2dddd-120">boolean</span></span>|<span data-ttu-id="2dddd-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="2dddd-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="2dddd-122">color</span><span class="sxs-lookup"><span data-stu-id="2dddd-122">color</span></span>|<span data-ttu-id="2dddd-123">string</span><span class="sxs-lookup"><span data-stu-id="2dddd-123">string</span></span>|<span data-ttu-id="2dddd-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="2dddd-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="2dddd-127">italic</span><span class="sxs-lookup"><span data-stu-id="2dddd-127">italic</span></span>|<span data-ttu-id="2dddd-128">booliano</span><span class="sxs-lookup"><span data-stu-id="2dddd-128">boolean</span></span>|<span data-ttu-id="2dddd-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="2dddd-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="2dddd-130">name</span><span class="sxs-lookup"><span data-stu-id="2dddd-130">name</span></span>|<span data-ttu-id="2dddd-131">string</span><span class="sxs-lookup"><span data-stu-id="2dddd-131">string</span></span>|<span data-ttu-id="2dddd-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="2dddd-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="2dddd-133">size</span><span class="sxs-lookup"><span data-stu-id="2dddd-133">size</span></span>|<span data-ttu-id="2dddd-134">Double</span><span class="sxs-lookup"><span data-stu-id="2dddd-134">double</span></span>|<span data-ttu-id="2dddd-135">Font Size</span><span class="sxs-lookup"><span data-stu-id="2dddd-135">Font size.</span></span>|
|<span data-ttu-id="2dddd-136">underline</span><span class="sxs-lookup"><span data-stu-id="2dddd-136">underline</span></span>|<span data-ttu-id="2dddd-137">string</span><span class="sxs-lookup"><span data-stu-id="2dddd-137">string</span></span>|<span data-ttu-id="2dddd-p102">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="2dddd-p102">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dddd-140">Relações</span><span class="sxs-lookup"><span data-stu-id="2dddd-140">Relationships</span></span>
<span data-ttu-id="2dddd-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2dddd-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2dddd-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2dddd-142">JSON representation</span></span>

<span data-ttu-id="2dddd-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2dddd-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
