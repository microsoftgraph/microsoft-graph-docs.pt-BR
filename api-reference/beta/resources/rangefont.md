---
title: Tipo de recurso RangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5500ad7a2ea16336e9be617678c4c85562e04bb3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571132"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="09a65-103">Tipo de recurso RangeFont</span><span class="sxs-lookup"><span data-stu-id="09a65-103">RangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09a65-104">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.</span><span class="sxs-lookup"><span data-stu-id="09a65-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="09a65-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="09a65-105">Methods</span></span>

| <span data-ttu-id="09a65-106">Método</span><span class="sxs-lookup"><span data-stu-id="09a65-106">Method</span></span>           | <span data-ttu-id="09a65-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="09a65-107">Return Type</span></span>    |<span data-ttu-id="09a65-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="09a65-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09a65-109">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="09a65-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="09a65-110">RangeFont</span><span class="sxs-lookup"><span data-stu-id="09a65-110">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="09a65-111">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="09a65-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="09a65-112">Update</span><span class="sxs-lookup"><span data-stu-id="09a65-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="09a65-113">RangeFont</span><span class="sxs-lookup"><span data-stu-id="09a65-113">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="09a65-114">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="09a65-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="09a65-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09a65-115">Properties</span></span>
| <span data-ttu-id="09a65-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09a65-116">Property</span></span>     | <span data-ttu-id="09a65-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="09a65-117">Type</span></span>   |<span data-ttu-id="09a65-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="09a65-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09a65-119">bold</span><span class="sxs-lookup"><span data-stu-id="09a65-119">bold</span></span>|<span data-ttu-id="09a65-120">booliano</span><span class="sxs-lookup"><span data-stu-id="09a65-120">boolean</span></span>|<span data-ttu-id="09a65-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="09a65-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="09a65-122">color</span><span class="sxs-lookup"><span data-stu-id="09a65-122">color</span></span>|<span data-ttu-id="09a65-123">string</span><span class="sxs-lookup"><span data-stu-id="09a65-123">string</span></span>|<span data-ttu-id="09a65-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="09a65-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="09a65-127">italic</span><span class="sxs-lookup"><span data-stu-id="09a65-127">italic</span></span>|<span data-ttu-id="09a65-128">booliano</span><span class="sxs-lookup"><span data-stu-id="09a65-128">boolean</span></span>|<span data-ttu-id="09a65-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="09a65-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="09a65-130">name</span><span class="sxs-lookup"><span data-stu-id="09a65-130">name</span></span>|<span data-ttu-id="09a65-131">string</span><span class="sxs-lookup"><span data-stu-id="09a65-131">string</span></span>|<span data-ttu-id="09a65-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="09a65-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="09a65-133">size</span><span class="sxs-lookup"><span data-stu-id="09a65-133">size</span></span>|<span data-ttu-id="09a65-134">Double</span><span class="sxs-lookup"><span data-stu-id="09a65-134">double</span></span>|<span data-ttu-id="09a65-135">Font Size</span><span class="sxs-lookup"><span data-stu-id="09a65-135">Font size.</span></span>|
|<span data-ttu-id="09a65-136">underline</span><span class="sxs-lookup"><span data-stu-id="09a65-136">underline</span></span>| <span data-ttu-id="09a65-137">cadeia de caracteres de enum</span><span class="sxs-lookup"><span data-stu-id="09a65-137">enum-string</span></span> |<span data-ttu-id="09a65-p102">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="09a65-p102">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09a65-140">Relações</span><span class="sxs-lookup"><span data-stu-id="09a65-140">Relationships</span></span>
<span data-ttu-id="09a65-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09a65-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="09a65-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09a65-142">JSON representation</span></span>

<span data-ttu-id="09a65-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09a65-143">Here is a JSON representation of the resource.</span></span>

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
  "underline": "None | Single | Double | SingleAccountant | DoubleAccountant"
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
