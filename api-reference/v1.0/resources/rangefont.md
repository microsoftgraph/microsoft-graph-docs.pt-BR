---
title: Tipo de recurso RangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 829b391d561aae63ae94972c55039acfdf4c48d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579519"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="1d714-103">Tipo de recurso RangeFont</span><span class="sxs-lookup"><span data-stu-id="1d714-103">RangeFont resource type</span></span>

<span data-ttu-id="1d714-104">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="1d714-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="1d714-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d714-105">Methods</span></span>

| <span data-ttu-id="1d714-106">Método</span><span class="sxs-lookup"><span data-stu-id="1d714-106">Method</span></span>           | <span data-ttu-id="1d714-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1d714-107">Return Type</span></span>    |<span data-ttu-id="1d714-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d714-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d714-109">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="1d714-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="1d714-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="1d714-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="1d714-111">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="1d714-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="1d714-112">Update</span><span class="sxs-lookup"><span data-stu-id="1d714-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="1d714-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="1d714-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="1d714-114">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="1d714-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d714-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d714-115">Properties</span></span>
| <span data-ttu-id="1d714-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d714-116">Property</span></span>     | <span data-ttu-id="1d714-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d714-117">Type</span></span>   |<span data-ttu-id="1d714-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d714-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d714-119">bold</span><span class="sxs-lookup"><span data-stu-id="1d714-119">bold</span></span>|<span data-ttu-id="1d714-120">booliano</span><span class="sxs-lookup"><span data-stu-id="1d714-120">boolean</span></span>|<span data-ttu-id="1d714-121">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="1d714-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="1d714-122">color</span><span class="sxs-lookup"><span data-stu-id="1d714-122">color</span></span>|<span data-ttu-id="1d714-123">string</span><span class="sxs-lookup"><span data-stu-id="1d714-123">string</span></span>|<span data-ttu-id="1d714-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="1d714-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="1d714-127">italic</span><span class="sxs-lookup"><span data-stu-id="1d714-127">italic</span></span>|<span data-ttu-id="1d714-128">booliano</span><span class="sxs-lookup"><span data-stu-id="1d714-128">boolean</span></span>|<span data-ttu-id="1d714-129">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="1d714-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="1d714-130">name</span><span class="sxs-lookup"><span data-stu-id="1d714-130">name</span></span>|<span data-ttu-id="1d714-131">string</span><span class="sxs-lookup"><span data-stu-id="1d714-131">string</span></span>|<span data-ttu-id="1d714-132">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="1d714-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="1d714-133">size</span><span class="sxs-lookup"><span data-stu-id="1d714-133">size</span></span>|<span data-ttu-id="1d714-134">Double</span><span class="sxs-lookup"><span data-stu-id="1d714-134">double</span></span>|<span data-ttu-id="1d714-135">Font Size</span><span class="sxs-lookup"><span data-stu-id="1d714-135">Font size.</span></span>|
|<span data-ttu-id="1d714-136">underline</span><span class="sxs-lookup"><span data-stu-id="1d714-136">underline</span></span>|<span data-ttu-id="1d714-137">string</span><span class="sxs-lookup"><span data-stu-id="1d714-137">string</span></span>|<span data-ttu-id="1d714-138">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="1d714-138">Type of underline applied to the font.</span></span> <span data-ttu-id="1d714-139">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="1d714-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d714-140">Relações</span><span class="sxs-lookup"><span data-stu-id="1d714-140">Relationships</span></span>
<span data-ttu-id="1d714-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d714-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1d714-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d714-142">JSON representation</span></span>

<span data-ttu-id="1d714-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d714-143">Here is a JSON representation of the resource.</span></span>

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
