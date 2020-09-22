---
title: Tipo de recurso RangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 95a58a62355c70b1f2588b83594ab5497ac3db49
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037069"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="e6d08-103">Tipo de recurso RangeFont</span><span class="sxs-lookup"><span data-stu-id="e6d08-103">RangeFont resource type</span></span>

<span data-ttu-id="e6d08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6d08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6d08-105">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="e6d08-105">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="e6d08-106">Methods</span><span class="sxs-lookup"><span data-stu-id="e6d08-106">Methods</span></span>

| <span data-ttu-id="e6d08-107">Método</span><span class="sxs-lookup"><span data-stu-id="e6d08-107">Method</span></span>           | <span data-ttu-id="e6d08-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6d08-108">Return Type</span></span>    |<span data-ttu-id="e6d08-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6d08-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6d08-110">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="e6d08-110">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="e6d08-111">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="e6d08-111">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="e6d08-112">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="e6d08-112">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="e6d08-113">Update</span><span class="sxs-lookup"><span data-stu-id="e6d08-113">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="e6d08-114">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="e6d08-114">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="e6d08-115">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="e6d08-115">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6d08-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6d08-116">Properties</span></span>
| <span data-ttu-id="e6d08-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6d08-117">Property</span></span>     | <span data-ttu-id="e6d08-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6d08-118">Type</span></span>   |<span data-ttu-id="e6d08-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6d08-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6d08-120">bold</span><span class="sxs-lookup"><span data-stu-id="e6d08-120">bold</span></span>|<span data-ttu-id="e6d08-121">booliano</span><span class="sxs-lookup"><span data-stu-id="e6d08-121">boolean</span></span>|<span data-ttu-id="e6d08-122">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="e6d08-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="e6d08-123">color</span><span class="sxs-lookup"><span data-stu-id="e6d08-123">color</span></span>|<span data-ttu-id="e6d08-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6d08-124">string</span></span>|<span data-ttu-id="e6d08-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="e6d08-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="e6d08-128">italic</span><span class="sxs-lookup"><span data-stu-id="e6d08-128">italic</span></span>|<span data-ttu-id="e6d08-129">booliano</span><span class="sxs-lookup"><span data-stu-id="e6d08-129">boolean</span></span>|<span data-ttu-id="e6d08-130">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="e6d08-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="e6d08-131">nome</span><span class="sxs-lookup"><span data-stu-id="e6d08-131">name</span></span>|<span data-ttu-id="e6d08-132">string</span><span class="sxs-lookup"><span data-stu-id="e6d08-132">string</span></span>|<span data-ttu-id="e6d08-133">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="e6d08-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="e6d08-134">size</span><span class="sxs-lookup"><span data-stu-id="e6d08-134">size</span></span>|<span data-ttu-id="e6d08-135">Double</span><span class="sxs-lookup"><span data-stu-id="e6d08-135">double</span></span>|<span data-ttu-id="e6d08-136">Font Size</span><span class="sxs-lookup"><span data-stu-id="e6d08-136">Font size.</span></span>|
|<span data-ttu-id="e6d08-137">underline</span><span class="sxs-lookup"><span data-stu-id="e6d08-137">underline</span></span>|<span data-ttu-id="e6d08-138">string</span><span class="sxs-lookup"><span data-stu-id="e6d08-138">string</span></span>|<span data-ttu-id="e6d08-139">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="e6d08-139">Type of underline applied to the font.</span></span> <span data-ttu-id="e6d08-140">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="e6d08-140">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6d08-141">Relações</span><span class="sxs-lookup"><span data-stu-id="e6d08-141">Relationships</span></span>
<span data-ttu-id="e6d08-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6d08-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6d08-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6d08-143">JSON representation</span></span>

<span data-ttu-id="e6d08-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6d08-144">Here is a JSON representation of the resource.</span></span>

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

