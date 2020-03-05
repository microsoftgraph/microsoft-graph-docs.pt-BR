---
title: Tipo de recurso RangeFormat
description: Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: edf239d5e14ca65ee4ae15f846182e5678f89f46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447014"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="ea458-103">Tipo de recurso RangeFormat</span><span class="sxs-lookup"><span data-stu-id="ea458-103">RangeFormat resource type</span></span>

<span data-ttu-id="ea458-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ea458-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea458-105">Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.</span><span class="sxs-lookup"><span data-stu-id="ea458-105">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="ea458-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea458-106">Methods</span></span>

| <span data-ttu-id="ea458-107">Método</span><span class="sxs-lookup"><span data-stu-id="ea458-107">Method</span></span>           | <span data-ttu-id="ea458-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea458-108">Return Type</span></span>    |<span data-ttu-id="ea458-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea458-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea458-110">Get RangeFormat</span><span class="sxs-lookup"><span data-stu-id="ea458-110">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="ea458-111">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="ea458-111">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="ea458-112">Leia as propriedades e relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="ea458-112">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="ea458-113">Create RangeBorder</span><span class="sxs-lookup"><span data-stu-id="ea458-113">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="ea458-114">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="ea458-114">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="ea458-115">Crie uma nova RangeBorder postando na coleção de bordas.</span><span class="sxs-lookup"><span data-stu-id="ea458-115">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="ea458-116">List borders</span><span class="sxs-lookup"><span data-stu-id="ea458-116">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="ea458-117">Coleção [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="ea458-117">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="ea458-118">Obtenha uma coleção de objetos RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="ea458-118">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="ea458-119">Update</span><span class="sxs-lookup"><span data-stu-id="ea458-119">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="ea458-120">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="ea458-120">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="ea458-121">Atualize o objeto RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="ea458-121">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="ea458-122">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="ea458-122">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="ea458-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea458-123">None</span></span>|<span data-ttu-id="ea458-124">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="ea458-124">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="ea458-125">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="ea458-125">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="ea458-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea458-126">None</span></span>|<span data-ttu-id="ea458-127">Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="ea458-127">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea458-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea458-128">Properties</span></span>
| <span data-ttu-id="ea458-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea458-129">Property</span></span>     | <span data-ttu-id="ea458-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea458-130">Type</span></span>   |<span data-ttu-id="ea458-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea458-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea458-132">columnWidth</span><span class="sxs-lookup"><span data-stu-id="ea458-132">columnWidth</span></span>|<span data-ttu-id="ea458-133">double</span><span class="sxs-lookup"><span data-stu-id="ea458-133">double</span></span>|<span data-ttu-id="ea458-p101">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="ea458-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="ea458-136">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="ea458-136">horizontalAlignment</span></span>|<span data-ttu-id="ea458-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea458-137">string</span></span>|<span data-ttu-id="ea458-138">Representa o alinhamento horizontal do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="ea458-138">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="ea458-139">Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="ea458-139">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="ea458-140">rowHeight</span><span class="sxs-lookup"><span data-stu-id="ea458-140">rowHeight</span></span>|<span data-ttu-id="ea458-141">duplo</span><span class="sxs-lookup"><span data-stu-id="ea458-141">double</span></span>|<span data-ttu-id="ea458-p103">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="ea458-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="ea458-144">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="ea458-144">verticalAlignment</span></span>|<span data-ttu-id="ea458-145">string</span><span class="sxs-lookup"><span data-stu-id="ea458-145">string</span></span>|<span data-ttu-id="ea458-146">Representa o alinhamento vertical do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="ea458-146">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="ea458-147">Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="ea458-147">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="ea458-148">wrapText</span><span class="sxs-lookup"><span data-stu-id="ea458-148">wrapText</span></span>|<span data-ttu-id="ea458-149">booliano</span><span class="sxs-lookup"><span data-stu-id="ea458-149">boolean</span></span>|<span data-ttu-id="ea458-p105">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="ea458-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea458-152">Relações</span><span class="sxs-lookup"><span data-stu-id="ea458-152">Relationships</span></span>
| <span data-ttu-id="ea458-153">Relação</span><span class="sxs-lookup"><span data-stu-id="ea458-153">Relationship</span></span> | <span data-ttu-id="ea458-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea458-154">Type</span></span>   |<span data-ttu-id="ea458-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea458-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea458-156">Borders</span><span class="sxs-lookup"><span data-stu-id="ea458-156">borders</span></span>|<span data-ttu-id="ea458-157">Coleção [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="ea458-157">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="ea458-158">Coleção de objetos de borda que se aplicam a todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea458-158">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="ea458-159">fill</span><span class="sxs-lookup"><span data-stu-id="ea458-159">fill</span></span>|[<span data-ttu-id="ea458-160">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="ea458-160">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="ea458-p106">Retorna o objeto de preenchimento definido em todo o intervalo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea458-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="ea458-163">font</span><span class="sxs-lookup"><span data-stu-id="ea458-163">font</span></span>|[<span data-ttu-id="ea458-164">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="ea458-164">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="ea458-165">Retorna o objeto Font definido em todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea458-165">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="ea458-166">protection</span><span class="sxs-lookup"><span data-stu-id="ea458-166">protection</span></span>|[<span data-ttu-id="ea458-167">WorkbookFormatProtection</span><span class="sxs-lookup"><span data-stu-id="ea458-167">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="ea458-168">Retorna o objeto de proteção de formato para um intervalo.</span><span class="sxs-lookup"><span data-stu-id="ea458-168">Returns the format protection object for a range.</span></span> <span data-ttu-id="ea458-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea458-169">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea458-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea458-170">JSON representation</span></span>

<span data-ttu-id="ea458-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea458-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
