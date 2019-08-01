---
title: Tipo de recurso RangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fe49cc3209164778bbeed625b3c24c7cc8ee3238
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034899"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="1a5c7-103">Tipo de recurso RangeFont</span><span class="sxs-lookup"><span data-stu-id="1a5c7-103">RangeFont resource type</span></span>

<span data-ttu-id="1a5c7-104">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="1a5c7-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="1a5c7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a5c7-105">Methods</span></span>

| <span data-ttu-id="1a5c7-106">Método</span><span class="sxs-lookup"><span data-stu-id="1a5c7-106">Method</span></span>           | <span data-ttu-id="1a5c7-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a5c7-107">Return Type</span></span>    |<span data-ttu-id="1a5c7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a5c7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a5c7-109">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="1a5c7-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="1a5c7-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="1a5c7-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="1a5c7-111">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="1a5c7-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="1a5c7-112">Update</span><span class="sxs-lookup"><span data-stu-id="1a5c7-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="1a5c7-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="1a5c7-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="1a5c7-114">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="1a5c7-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1a5c7-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a5c7-115">Properties</span></span>
| <span data-ttu-id="1a5c7-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a5c7-116">Property</span></span>     | <span data-ttu-id="1a5c7-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a5c7-117">Type</span></span>   |<span data-ttu-id="1a5c7-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a5c7-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a5c7-119">bold</span><span class="sxs-lookup"><span data-stu-id="1a5c7-119">bold</span></span>|<span data-ttu-id="1a5c7-120">booliano</span><span class="sxs-lookup"><span data-stu-id="1a5c7-120">boolean</span></span>|<span data-ttu-id="1a5c7-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="1a5c7-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="1a5c7-122">color</span><span class="sxs-lookup"><span data-stu-id="1a5c7-122">color</span></span>|<span data-ttu-id="1a5c7-123">string</span><span class="sxs-lookup"><span data-stu-id="1a5c7-123">string</span></span>|<span data-ttu-id="1a5c7-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="1a5c7-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="1a5c7-127">italic</span><span class="sxs-lookup"><span data-stu-id="1a5c7-127">italic</span></span>|<span data-ttu-id="1a5c7-128">booliano</span><span class="sxs-lookup"><span data-stu-id="1a5c7-128">boolean</span></span>|<span data-ttu-id="1a5c7-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="1a5c7-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="1a5c7-130">name</span><span class="sxs-lookup"><span data-stu-id="1a5c7-130">name</span></span>|<span data-ttu-id="1a5c7-131">string</span><span class="sxs-lookup"><span data-stu-id="1a5c7-131">string</span></span>|<span data-ttu-id="1a5c7-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="1a5c7-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="1a5c7-133">size</span><span class="sxs-lookup"><span data-stu-id="1a5c7-133">size</span></span>|<span data-ttu-id="1a5c7-134">Double</span><span class="sxs-lookup"><span data-stu-id="1a5c7-134">double</span></span>|<span data-ttu-id="1a5c7-135">Font Size</span><span class="sxs-lookup"><span data-stu-id="1a5c7-135">Font size.</span></span>|
|<span data-ttu-id="1a5c7-136">underline</span><span class="sxs-lookup"><span data-stu-id="1a5c7-136">underline</span></span>|<span data-ttu-id="1a5c7-137">string</span><span class="sxs-lookup"><span data-stu-id="1a5c7-137">string</span></span>|<span data-ttu-id="1a5c7-138">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="1a5c7-138">Type of underline applied to the font.</span></span> <span data-ttu-id="1a5c7-139">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="1a5c7-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a5c7-140">Relações</span><span class="sxs-lookup"><span data-stu-id="1a5c7-140">Relationships</span></span>
<span data-ttu-id="1a5c7-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a5c7-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1a5c7-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a5c7-142">JSON representation</span></span>

<span data-ttu-id="1a5c7-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a5c7-143">Here is a JSON representation of the resource.</span></span>

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
