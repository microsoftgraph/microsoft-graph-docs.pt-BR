---
title: Tipo de recurso ChartFont
description: Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4187d2837835520864ec3a1ef5c47b578b3d3da4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920944"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="cdd7e-103">Tipo de recurso ChartFont</span><span class="sxs-lookup"><span data-stu-id="cdd7e-103">ChartFont resource type</span></span>

> <span data-ttu-id="cdd7e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdd7e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cdd7e-106">Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-106">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="cdd7e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cdd7e-107">Methods</span></span>

| <span data-ttu-id="cdd7e-108">Método</span><span class="sxs-lookup"><span data-stu-id="cdd7e-108">Method</span></span>           | <span data-ttu-id="cdd7e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cdd7e-109">Return Type</span></span>    |<span data-ttu-id="cdd7e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdd7e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cdd7e-111">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="cdd7e-111">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="cdd7e-112">ChartFont</span><span class="sxs-lookup"><span data-stu-id="cdd7e-112">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="cdd7e-113">Leia as propriedades e os relacionamentos do objeto chartFont.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-113">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="cdd7e-114">Update</span><span class="sxs-lookup"><span data-stu-id="cdd7e-114">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="cdd7e-115">ChartFont</span><span class="sxs-lookup"><span data-stu-id="cdd7e-115">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="cdd7e-116">Atualize o objeto ChartFont.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-116">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cdd7e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cdd7e-117">Properties</span></span>
| <span data-ttu-id="cdd7e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdd7e-118">Property</span></span>     | <span data-ttu-id="cdd7e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdd7e-119">Type</span></span>   |<span data-ttu-id="cdd7e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdd7e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdd7e-121">bold</span><span class="sxs-lookup"><span data-stu-id="cdd7e-121">bold</span></span>|<span data-ttu-id="cdd7e-122">booliano</span><span class="sxs-lookup"><span data-stu-id="cdd7e-122">boolean</span></span>|<span data-ttu-id="cdd7e-123">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="cdd7e-124">color</span><span class="sxs-lookup"><span data-stu-id="cdd7e-124">color</span></span>|<span data-ttu-id="cdd7e-125">string</span><span class="sxs-lookup"><span data-stu-id="cdd7e-125">string</span></span>|<span data-ttu-id="cdd7e-p102">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="cdd7e-129">italic</span><span class="sxs-lookup"><span data-stu-id="cdd7e-129">italic</span></span>|<span data-ttu-id="cdd7e-130">booliano</span><span class="sxs-lookup"><span data-stu-id="cdd7e-130">boolean</span></span>|<span data-ttu-id="cdd7e-131">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="cdd7e-132">name</span><span class="sxs-lookup"><span data-stu-id="cdd7e-132">name</span></span>|<span data-ttu-id="cdd7e-133">string</span><span class="sxs-lookup"><span data-stu-id="cdd7e-133">string</span></span>|<span data-ttu-id="cdd7e-134">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="cdd7e-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="cdd7e-135">size</span><span class="sxs-lookup"><span data-stu-id="cdd7e-135">size</span></span>|<span data-ttu-id="cdd7e-136">Double</span><span class="sxs-lookup"><span data-stu-id="cdd7e-136">double</span></span>|<span data-ttu-id="cdd7e-137">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-137">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="cdd7e-138">underline</span><span class="sxs-lookup"><span data-stu-id="cdd7e-138">underline</span></span>|<span data-ttu-id="cdd7e-139">string</span><span class="sxs-lookup"><span data-stu-id="cdd7e-139">string</span></span>|<span data-ttu-id="cdd7e-p103">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None` e `Single`.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-p103">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdd7e-142">Relações</span><span class="sxs-lookup"><span data-stu-id="cdd7e-142">Relationships</span></span>
<span data-ttu-id="cdd7e-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cdd7e-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cdd7e-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cdd7e-144">JSON representation</span></span>

<span data-ttu-id="cdd7e-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cdd7e-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
