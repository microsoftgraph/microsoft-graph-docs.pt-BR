---
title: tipo de recurso workbookRangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9ddbb607a243f4571d53dcf887f80a171b230748
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519173"
---
# <a name="workbookrangefont-resource-type"></a><span data-ttu-id="99c64-103">tipo de recurso workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="99c64-103">workbookRangeFont resource type</span></span>

<span data-ttu-id="99c64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99c64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99c64-105">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="99c64-105">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="99c64-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="99c64-106">Methods</span></span>

| <span data-ttu-id="99c64-107">Método</span><span class="sxs-lookup"><span data-stu-id="99c64-107">Method</span></span>           | <span data-ttu-id="99c64-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="99c64-108">Return Type</span></span>    |<span data-ttu-id="99c64-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="99c64-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99c64-110">Obter workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="99c64-110">Get workbookRangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="99c64-111">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="99c64-111">workbookRangeFont</span></span>](workbookrangefont.md) |<span data-ttu-id="99c64-112">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="99c64-112">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="99c64-113">Update</span><span class="sxs-lookup"><span data-stu-id="99c64-113">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="99c64-114">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="99c64-114">workbookRangeFont</span></span>](workbookrangefont.md)   |<span data-ttu-id="99c64-115">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="99c64-115">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="99c64-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99c64-116">Properties</span></span>
| <span data-ttu-id="99c64-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99c64-117">Property</span></span>     | <span data-ttu-id="99c64-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="99c64-118">Type</span></span>   |<span data-ttu-id="99c64-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="99c64-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99c64-120">bold</span><span class="sxs-lookup"><span data-stu-id="99c64-120">bold</span></span>|<span data-ttu-id="99c64-121">booliano</span><span class="sxs-lookup"><span data-stu-id="99c64-121">boolean</span></span>|<span data-ttu-id="99c64-122">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="99c64-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="99c64-123">color</span><span class="sxs-lookup"><span data-stu-id="99c64-123">color</span></span>|<span data-ttu-id="99c64-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99c64-124">string</span></span>|<span data-ttu-id="99c64-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="99c64-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="99c64-128">italic</span><span class="sxs-lookup"><span data-stu-id="99c64-128">italic</span></span>|<span data-ttu-id="99c64-129">booliano</span><span class="sxs-lookup"><span data-stu-id="99c64-129">boolean</span></span>|<span data-ttu-id="99c64-130">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="99c64-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="99c64-131">nome</span><span class="sxs-lookup"><span data-stu-id="99c64-131">name</span></span>|<span data-ttu-id="99c64-132">string</span><span class="sxs-lookup"><span data-stu-id="99c64-132">string</span></span>|<span data-ttu-id="99c64-133">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="99c64-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="99c64-134">size</span><span class="sxs-lookup"><span data-stu-id="99c64-134">size</span></span>|<span data-ttu-id="99c64-135">Double</span><span class="sxs-lookup"><span data-stu-id="99c64-135">double</span></span>|<span data-ttu-id="99c64-136">Font Size</span><span class="sxs-lookup"><span data-stu-id="99c64-136">Font size.</span></span>|
|<span data-ttu-id="99c64-137">underline</span><span class="sxs-lookup"><span data-stu-id="99c64-137">underline</span></span>| <span data-ttu-id="99c64-138">String</span><span class="sxs-lookup"><span data-stu-id="99c64-138">String</span></span> |<span data-ttu-id="99c64-139">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="99c64-139">Type of underline applied to the font.</span></span> <span data-ttu-id="99c64-140">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="99c64-140">Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99c64-141">Relações</span><span class="sxs-lookup"><span data-stu-id="99c64-141">Relationships</span></span>
<span data-ttu-id="99c64-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99c64-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="99c64-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99c64-143">JSON representation</span></span>

<span data-ttu-id="99c64-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99c64-144">Here is a JSON representation of the resource.</span></span>

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
