---
title: Tipo de recurso RangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2dee07b7d2573081650bdd15799e4884c774e171
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563317"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="4774c-103">Tipo de recurso RangeFont</span><span class="sxs-lookup"><span data-stu-id="4774c-103">RangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4774c-104">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="4774c-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="4774c-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4774c-105">Methods</span></span>

| <span data-ttu-id="4774c-106">Método</span><span class="sxs-lookup"><span data-stu-id="4774c-106">Method</span></span>           | <span data-ttu-id="4774c-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4774c-107">Return Type</span></span>    |<span data-ttu-id="4774c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4774c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4774c-109">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="4774c-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="4774c-110">RangeFont</span><span class="sxs-lookup"><span data-stu-id="4774c-110">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="4774c-111">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="4774c-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="4774c-112">Update</span><span class="sxs-lookup"><span data-stu-id="4774c-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="4774c-113">RangeFont</span><span class="sxs-lookup"><span data-stu-id="4774c-113">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="4774c-114">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="4774c-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4774c-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4774c-115">Properties</span></span>
| <span data-ttu-id="4774c-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4774c-116">Property</span></span>     | <span data-ttu-id="4774c-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="4774c-117">Type</span></span>   |<span data-ttu-id="4774c-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="4774c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4774c-119">bold</span><span class="sxs-lookup"><span data-stu-id="4774c-119">bold</span></span>|<span data-ttu-id="4774c-120">booliano</span><span class="sxs-lookup"><span data-stu-id="4774c-120">boolean</span></span>|<span data-ttu-id="4774c-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="4774c-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="4774c-122">color</span><span class="sxs-lookup"><span data-stu-id="4774c-122">color</span></span>|<span data-ttu-id="4774c-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4774c-123">string</span></span>|<span data-ttu-id="4774c-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="4774c-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="4774c-127">italic</span><span class="sxs-lookup"><span data-stu-id="4774c-127">italic</span></span>|<span data-ttu-id="4774c-128">booliano</span><span class="sxs-lookup"><span data-stu-id="4774c-128">boolean</span></span>|<span data-ttu-id="4774c-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="4774c-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="4774c-130">name</span><span class="sxs-lookup"><span data-stu-id="4774c-130">name</span></span>|<span data-ttu-id="4774c-131">string</span><span class="sxs-lookup"><span data-stu-id="4774c-131">string</span></span>|<span data-ttu-id="4774c-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="4774c-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="4774c-133">size</span><span class="sxs-lookup"><span data-stu-id="4774c-133">size</span></span>|<span data-ttu-id="4774c-134">Double</span><span class="sxs-lookup"><span data-stu-id="4774c-134">double</span></span>|<span data-ttu-id="4774c-135">Font Size</span><span class="sxs-lookup"><span data-stu-id="4774c-135">Font size.</span></span>|
|<span data-ttu-id="4774c-136">underline</span><span class="sxs-lookup"><span data-stu-id="4774c-136">underline</span></span>|<span data-ttu-id="4774c-137">string</span><span class="sxs-lookup"><span data-stu-id="4774c-137">string</span></span>|<span data-ttu-id="4774c-p102">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="4774c-p102">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4774c-140">Relações</span><span class="sxs-lookup"><span data-stu-id="4774c-140">Relationships</span></span>
<span data-ttu-id="4774c-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4774c-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4774c-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4774c-142">JSON representation</span></span>

<span data-ttu-id="4774c-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4774c-143">Here is a JSON representation of the resource.</span></span>

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
