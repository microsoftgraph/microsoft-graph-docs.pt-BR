---
title: Tipo de recurso RangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.
ms.openlocfilehash: fc1f3e35bb2ea612dd462d97075ad9757e27bf22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033786"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="67cea-103">Tipo de recurso RangeFont</span><span class="sxs-lookup"><span data-stu-id="67cea-103">RangeFont resource type</span></span>

> <span data-ttu-id="67cea-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="67cea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67cea-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="67cea-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67cea-106">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.</span><span class="sxs-lookup"><span data-stu-id="67cea-106">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="67cea-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="67cea-107">Methods</span></span>

| <span data-ttu-id="67cea-108">Método</span><span class="sxs-lookup"><span data-stu-id="67cea-108">Method</span></span>           | <span data-ttu-id="67cea-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="67cea-109">Return Type</span></span>    |<span data-ttu-id="67cea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="67cea-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67cea-111">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="67cea-111">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="67cea-112">RangeFont</span><span class="sxs-lookup"><span data-stu-id="67cea-112">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="67cea-113">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="67cea-113">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="67cea-114">Update</span><span class="sxs-lookup"><span data-stu-id="67cea-114">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="67cea-115">RangeFont</span><span class="sxs-lookup"><span data-stu-id="67cea-115">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="67cea-116">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="67cea-116">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="67cea-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67cea-117">Properties</span></span>
| <span data-ttu-id="67cea-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67cea-118">Property</span></span>     | <span data-ttu-id="67cea-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="67cea-119">Type</span></span>   |<span data-ttu-id="67cea-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="67cea-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67cea-121">bold</span><span class="sxs-lookup"><span data-stu-id="67cea-121">bold</span></span>|<span data-ttu-id="67cea-122">booliano</span><span class="sxs-lookup"><span data-stu-id="67cea-122">boolean</span></span>|<span data-ttu-id="67cea-123">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="67cea-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="67cea-124">color</span><span class="sxs-lookup"><span data-stu-id="67cea-124">color</span></span>|<span data-ttu-id="67cea-125">string</span><span class="sxs-lookup"><span data-stu-id="67cea-125">string</span></span>|<span data-ttu-id="67cea-p102">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="67cea-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="67cea-129">italic</span><span class="sxs-lookup"><span data-stu-id="67cea-129">italic</span></span>|<span data-ttu-id="67cea-130">booliano</span><span class="sxs-lookup"><span data-stu-id="67cea-130">boolean</span></span>|<span data-ttu-id="67cea-131">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="67cea-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="67cea-132">name</span><span class="sxs-lookup"><span data-stu-id="67cea-132">name</span></span>|<span data-ttu-id="67cea-133">string</span><span class="sxs-lookup"><span data-stu-id="67cea-133">string</span></span>|<span data-ttu-id="67cea-134">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="67cea-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="67cea-135">size</span><span class="sxs-lookup"><span data-stu-id="67cea-135">size</span></span>|<span data-ttu-id="67cea-136">Double</span><span class="sxs-lookup"><span data-stu-id="67cea-136">double</span></span>|<span data-ttu-id="67cea-137">Font Size</span><span class="sxs-lookup"><span data-stu-id="67cea-137">Font size.</span></span>|
|<span data-ttu-id="67cea-138">underline</span><span class="sxs-lookup"><span data-stu-id="67cea-138">underline</span></span>|<span data-ttu-id="67cea-139">string</span><span class="sxs-lookup"><span data-stu-id="67cea-139">string</span></span>|<span data-ttu-id="67cea-p103">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="67cea-p103">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67cea-142">Relações</span><span class="sxs-lookup"><span data-stu-id="67cea-142">Relationships</span></span>
<span data-ttu-id="67cea-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67cea-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="67cea-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67cea-144">JSON representation</span></span>

<span data-ttu-id="67cea-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67cea-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->