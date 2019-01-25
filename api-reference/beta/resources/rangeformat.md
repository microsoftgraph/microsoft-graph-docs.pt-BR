---
title: Tipo de recurso RangeFormat
description: Um objeto de formatação que engloba a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 58ed56b11b571237211307c8fb0dd1abaf27761f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511356"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="f2592-103">Tipo de recurso RangeFormat</span><span class="sxs-lookup"><span data-stu-id="f2592-103">RangeFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2592-104">Um objeto de formatação que engloba a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.</span><span class="sxs-lookup"><span data-stu-id="f2592-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="f2592-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2592-105">Methods</span></span>

| <span data-ttu-id="f2592-106">Método</span><span class="sxs-lookup"><span data-stu-id="f2592-106">Method</span></span>           | <span data-ttu-id="f2592-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2592-107">Return Type</span></span>    |<span data-ttu-id="f2592-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2592-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2592-109">Get RangeFormat</span><span class="sxs-lookup"><span data-stu-id="f2592-109">[Get RangeFormat](../api/rangeformat-get.md)</span></span> | [<span data-ttu-id="f2592-110">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="f2592-110">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="f2592-111">Leia as propriedades e relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="f2592-111">Read properties and relationships of rangeFormat object.</span></span>|
|<span data-ttu-id="f2592-112">Create RangeBorder</span><span class="sxs-lookup"><span data-stu-id="f2592-112">[Create RangeBorder](../api/rangeformat-post-borders.md)</span></span> |<span data-ttu-id="f2592-113">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="f2592-113">[RangeBorder](rangeborder.md)</span></span>| <span data-ttu-id="f2592-114">Crie uma nova RangeBorder postando na coleção de bordas.</span><span class="sxs-lookup"><span data-stu-id="f2592-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|<span data-ttu-id="f2592-115">List borders</span><span class="sxs-lookup"><span data-stu-id="f2592-115">[List borders](../api/rangeformat-list-borders.md)</span></span> |<span data-ttu-id="f2592-116">Coleção RangeBorder</span><span class="sxs-lookup"><span data-stu-id="f2592-116">[RangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="f2592-117">Obtenha uma coleção de objetos RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="f2592-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="f2592-118">Update</span><span class="sxs-lookup"><span data-stu-id="f2592-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="f2592-119">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="f2592-119">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="f2592-120">Atualize o objeto RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="f2592-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="f2592-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="f2592-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="f2592-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2592-122">None</span></span>|<span data-ttu-id="f2592-123">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="f2592-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="f2592-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="f2592-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="f2592-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2592-125">None</span></span>|<span data-ttu-id="f2592-126">Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="f2592-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2592-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2592-127">Properties</span></span>
| <span data-ttu-id="f2592-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2592-128">Property</span></span>     | <span data-ttu-id="f2592-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2592-129">Type</span></span>   |<span data-ttu-id="f2592-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2592-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2592-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="f2592-131">columnWidth</span></span>|<span data-ttu-id="f2592-132">double</span><span class="sxs-lookup"><span data-stu-id="f2592-132">double</span></span>|<span data-ttu-id="f2592-p101">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="f2592-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="f2592-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="f2592-135">horizontalAlignment</span></span>|<span data-ttu-id="f2592-136">string</span><span class="sxs-lookup"><span data-stu-id="f2592-136">string</span></span>|<span data-ttu-id="f2592-p102">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="f2592-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="f2592-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="f2592-139">rowHeight</span></span>|<span data-ttu-id="f2592-140">double</span><span class="sxs-lookup"><span data-stu-id="f2592-140">double</span></span>|<span data-ttu-id="f2592-p103">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="f2592-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="f2592-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="f2592-143">verticalAlignment</span></span>|<span data-ttu-id="f2592-144">string</span><span class="sxs-lookup"><span data-stu-id="f2592-144">string</span></span>|<span data-ttu-id="f2592-p104">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="f2592-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="f2592-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="f2592-147">wrapText</span></span>|<span data-ttu-id="f2592-148">booliano</span><span class="sxs-lookup"><span data-stu-id="f2592-148">boolean</span></span>|<span data-ttu-id="f2592-p105">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="f2592-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2592-151">Relações</span><span class="sxs-lookup"><span data-stu-id="f2592-151">Relationships</span></span>
| <span data-ttu-id="f2592-152">Relação</span><span class="sxs-lookup"><span data-stu-id="f2592-152">Relationship</span></span> | <span data-ttu-id="f2592-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2592-153">Type</span></span>   |<span data-ttu-id="f2592-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2592-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2592-155">borders</span><span class="sxs-lookup"><span data-stu-id="f2592-155">borders</span></span>|<span data-ttu-id="f2592-156">Coleção [RangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="f2592-156">[RangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="f2592-157">Coleção de objetos de borda que se aplicam a todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2592-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="f2592-158">fill</span><span class="sxs-lookup"><span data-stu-id="f2592-158">fill</span></span>|[<span data-ttu-id="f2592-159">RangeFill</span><span class="sxs-lookup"><span data-stu-id="f2592-159">RangeFill</span></span>](rangefill.md)|<span data-ttu-id="f2592-p106">Retorna o objeto de preenchimento definido em todo o intervalo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2592-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="f2592-162">font</span><span class="sxs-lookup"><span data-stu-id="f2592-162">font</span></span>|[<span data-ttu-id="f2592-163">RangeFont</span><span class="sxs-lookup"><span data-stu-id="f2592-163">RangeFont</span></span>](rangefont.md)|<span data-ttu-id="f2592-164">Retorna o objeto Font definido em todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2592-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="f2592-165">protection</span><span class="sxs-lookup"><span data-stu-id="f2592-165">protection</span></span>|[<span data-ttu-id="f2592-166">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="f2592-166">FormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="f2592-p107">Retorna o objeto de proteção de formato para um intervalo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2592-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2592-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2592-169">JSON representation</span></span>

<span data-ttu-id="f2592-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2592-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangeformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
