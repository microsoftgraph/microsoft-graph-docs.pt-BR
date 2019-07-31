---
title: tipo de recurso workbookRangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b3982a8026cd720fe614b11405a37bed8626042d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964032"
---
# <a name="workbookrangefont-resource-type"></a><span data-ttu-id="5cadd-103">tipo de recurso workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="5cadd-103">workbookRangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cadd-104">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="5cadd-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="5cadd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="5cadd-105">Methods</span></span>

| <span data-ttu-id="5cadd-106">Método</span><span class="sxs-lookup"><span data-stu-id="5cadd-106">Method</span></span>           | <span data-ttu-id="5cadd-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5cadd-107">Return Type</span></span>    |<span data-ttu-id="5cadd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cadd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cadd-109">Obter workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="5cadd-109">Get workbookRangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="5cadd-110">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="5cadd-110">workbookRangeFont</span></span>](workbookrangefont.md) |<span data-ttu-id="5cadd-111">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="5cadd-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="5cadd-112">Update</span><span class="sxs-lookup"><span data-stu-id="5cadd-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="5cadd-113">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="5cadd-113">workbookRangeFont</span></span>](workbookrangefont.md)   |<span data-ttu-id="5cadd-114">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="5cadd-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cadd-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cadd-115">Properties</span></span>
| <span data-ttu-id="5cadd-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cadd-116">Property</span></span>     | <span data-ttu-id="5cadd-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cadd-117">Type</span></span>   |<span data-ttu-id="5cadd-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cadd-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cadd-119">bold</span><span class="sxs-lookup"><span data-stu-id="5cadd-119">bold</span></span>|<span data-ttu-id="5cadd-120">booliano</span><span class="sxs-lookup"><span data-stu-id="5cadd-120">boolean</span></span>|<span data-ttu-id="5cadd-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="5cadd-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="5cadd-122">color</span><span class="sxs-lookup"><span data-stu-id="5cadd-122">color</span></span>|<span data-ttu-id="5cadd-123">string</span><span class="sxs-lookup"><span data-stu-id="5cadd-123">string</span></span>|<span data-ttu-id="5cadd-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="5cadd-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="5cadd-127">italic</span><span class="sxs-lookup"><span data-stu-id="5cadd-127">italic</span></span>|<span data-ttu-id="5cadd-128">booliano</span><span class="sxs-lookup"><span data-stu-id="5cadd-128">boolean</span></span>|<span data-ttu-id="5cadd-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="5cadd-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="5cadd-130">name</span><span class="sxs-lookup"><span data-stu-id="5cadd-130">name</span></span>|<span data-ttu-id="5cadd-131">string</span><span class="sxs-lookup"><span data-stu-id="5cadd-131">string</span></span>|<span data-ttu-id="5cadd-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="5cadd-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="5cadd-133">size</span><span class="sxs-lookup"><span data-stu-id="5cadd-133">size</span></span>|<span data-ttu-id="5cadd-134">Double</span><span class="sxs-lookup"><span data-stu-id="5cadd-134">double</span></span>|<span data-ttu-id="5cadd-135">Font Size</span><span class="sxs-lookup"><span data-stu-id="5cadd-135">Font size.</span></span>|
|<span data-ttu-id="5cadd-136">underline</span><span class="sxs-lookup"><span data-stu-id="5cadd-136">underline</span></span>| <span data-ttu-id="5cadd-137">String</span><span class="sxs-lookup"><span data-stu-id="5cadd-137">String</span></span> |<span data-ttu-id="5cadd-138">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="5cadd-138">Type of underline applied to the font.</span></span> <span data-ttu-id="5cadd-139">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="5cadd-139">Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cadd-140">Relações</span><span class="sxs-lookup"><span data-stu-id="5cadd-140">Relationships</span></span>
<span data-ttu-id="5cadd-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cadd-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5cadd-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cadd-142">JSON representation</span></span>

<span data-ttu-id="5cadd-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cadd-143">Here is a JSON representation of the resource.</span></span>

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
