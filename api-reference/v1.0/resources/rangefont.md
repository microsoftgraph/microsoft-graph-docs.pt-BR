---
title: Tipo de recurso RangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.
ms.openlocfilehash: bafb7c052458c7b3f4001d7e999acc14c7aaabee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006365"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="17675-103">Tipo de recurso RangeFont</span><span class="sxs-lookup"><span data-stu-id="17675-103">RangeFont resource type</span></span>

<span data-ttu-id="17675-104">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.</span><span class="sxs-lookup"><span data-stu-id="17675-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="17675-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="17675-105">Methods</span></span>

| <span data-ttu-id="17675-106">Método</span><span class="sxs-lookup"><span data-stu-id="17675-106">Method</span></span>           | <span data-ttu-id="17675-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="17675-107">Return Type</span></span>    |<span data-ttu-id="17675-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="17675-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17675-109">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="17675-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="17675-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="17675-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="17675-111">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="17675-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="17675-112">Update</span><span class="sxs-lookup"><span data-stu-id="17675-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="17675-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="17675-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="17675-114">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="17675-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="17675-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17675-115">Properties</span></span>
| <span data-ttu-id="17675-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17675-116">Property</span></span>     | <span data-ttu-id="17675-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="17675-117">Type</span></span>   |<span data-ttu-id="17675-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="17675-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17675-119">bold</span><span class="sxs-lookup"><span data-stu-id="17675-119">bold</span></span>|<span data-ttu-id="17675-120">booliano</span><span class="sxs-lookup"><span data-stu-id="17675-120">boolean</span></span>|<span data-ttu-id="17675-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="17675-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="17675-122">color</span><span class="sxs-lookup"><span data-stu-id="17675-122">color</span></span>|<span data-ttu-id="17675-123">string</span><span class="sxs-lookup"><span data-stu-id="17675-123">string</span></span>|<span data-ttu-id="17675-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="17675-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="17675-127">italic</span><span class="sxs-lookup"><span data-stu-id="17675-127">italic</span></span>|<span data-ttu-id="17675-128">booliano</span><span class="sxs-lookup"><span data-stu-id="17675-128">boolean</span></span>|<span data-ttu-id="17675-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="17675-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="17675-130">name</span><span class="sxs-lookup"><span data-stu-id="17675-130">name</span></span>|<span data-ttu-id="17675-131">string</span><span class="sxs-lookup"><span data-stu-id="17675-131">string</span></span>|<span data-ttu-id="17675-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="17675-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="17675-133">size</span><span class="sxs-lookup"><span data-stu-id="17675-133">size</span></span>|<span data-ttu-id="17675-134">Double</span><span class="sxs-lookup"><span data-stu-id="17675-134">double</span></span>|<span data-ttu-id="17675-135">Font Size</span><span class="sxs-lookup"><span data-stu-id="17675-135">Font size.</span></span>|
|<span data-ttu-id="17675-136">underline</span><span class="sxs-lookup"><span data-stu-id="17675-136">underline</span></span>|<span data-ttu-id="17675-137">string</span><span class="sxs-lookup"><span data-stu-id="17675-137">string</span></span>|<span data-ttu-id="17675-138">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="17675-138">Type of underline applied to the font.</span></span> <span data-ttu-id="17675-139">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="17675-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17675-140">Relações</span><span class="sxs-lookup"><span data-stu-id="17675-140">Relationships</span></span>
<span data-ttu-id="17675-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17675-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="17675-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17675-142">JSON representation</span></span>

<span data-ttu-id="17675-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17675-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->