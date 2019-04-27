---
title: tipo de recurso workbookRangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 76b84a86c0d5796b4831fa362ee98c0b1093e830
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348514"
---
# <a name="workbookrangefont-resource-type"></a><span data-ttu-id="151f3-103">tipo de recurso workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="151f3-103">workbookRangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="151f3-104">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="151f3-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="151f3-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="151f3-105">Methods</span></span>

| <span data-ttu-id="151f3-106">Método</span><span class="sxs-lookup"><span data-stu-id="151f3-106">Method</span></span>           | <span data-ttu-id="151f3-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="151f3-107">Return Type</span></span>    |<span data-ttu-id="151f3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="151f3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="151f3-109">Obter workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="151f3-109">Get workbookRangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="151f3-110">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="151f3-110">workbookRangeFont</span></span>](workbookrangefont.md) |<span data-ttu-id="151f3-111">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="151f3-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="151f3-112">Update</span><span class="sxs-lookup"><span data-stu-id="151f3-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="151f3-113">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="151f3-113">workbookRangeFont</span></span>](workbookrangefont.md)   |<span data-ttu-id="151f3-114">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="151f3-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="151f3-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="151f3-115">Properties</span></span>
| <span data-ttu-id="151f3-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="151f3-116">Property</span></span>     | <span data-ttu-id="151f3-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="151f3-117">Type</span></span>   |<span data-ttu-id="151f3-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="151f3-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="151f3-119">bold</span><span class="sxs-lookup"><span data-stu-id="151f3-119">bold</span></span>|<span data-ttu-id="151f3-120">booliano</span><span class="sxs-lookup"><span data-stu-id="151f3-120">boolean</span></span>|<span data-ttu-id="151f3-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="151f3-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="151f3-122">color</span><span class="sxs-lookup"><span data-stu-id="151f3-122">color</span></span>|<span data-ttu-id="151f3-123">string</span><span class="sxs-lookup"><span data-stu-id="151f3-123">string</span></span>|<span data-ttu-id="151f3-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="151f3-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="151f3-127">italic</span><span class="sxs-lookup"><span data-stu-id="151f3-127">italic</span></span>|<span data-ttu-id="151f3-128">booliano</span><span class="sxs-lookup"><span data-stu-id="151f3-128">boolean</span></span>|<span data-ttu-id="151f3-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="151f3-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="151f3-130">name</span><span class="sxs-lookup"><span data-stu-id="151f3-130">name</span></span>|<span data-ttu-id="151f3-131">string</span><span class="sxs-lookup"><span data-stu-id="151f3-131">string</span></span>|<span data-ttu-id="151f3-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="151f3-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="151f3-133">size</span><span class="sxs-lookup"><span data-stu-id="151f3-133">size</span></span>|<span data-ttu-id="151f3-134">Double</span><span class="sxs-lookup"><span data-stu-id="151f3-134">double</span></span>|<span data-ttu-id="151f3-135">Font Size</span><span class="sxs-lookup"><span data-stu-id="151f3-135">Font size.</span></span>|
|<span data-ttu-id="151f3-136">underline</span><span class="sxs-lookup"><span data-stu-id="151f3-136">underline</span></span>| <span data-ttu-id="151f3-137">String</span><span class="sxs-lookup"><span data-stu-id="151f3-137">String</span></span> |<span data-ttu-id="151f3-138">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="151f3-138">Type of underline applied to the font.</span></span> <span data-ttu-id="151f3-139">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="151f3-139">Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="151f3-140">Relações</span><span class="sxs-lookup"><span data-stu-id="151f3-140">Relationships</span></span>
<span data-ttu-id="151f3-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="151f3-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="151f3-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="151f3-142">JSON representation</span></span>

<span data-ttu-id="151f3-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="151f3-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
