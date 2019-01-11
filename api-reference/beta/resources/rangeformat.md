---
title: Tipo de recurso RangeFormat
description: Um objeto de formatação que engloba a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.
localization_priority: Normal
ms.openlocfilehash: 38844e2f43dcb56021e25ad189529b36cc8eb456
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880763"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="d5e32-103">Tipo de recurso RangeFormat</span><span class="sxs-lookup"><span data-stu-id="d5e32-103">RangeFormat resource type</span></span>

> <span data-ttu-id="d5e32-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5e32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5e32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5e32-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5e32-106">Um objeto de formatação que engloba a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.</span><span class="sxs-lookup"><span data-stu-id="d5e32-106">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="d5e32-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5e32-107">Methods</span></span>

| <span data-ttu-id="d5e32-108">Método</span><span class="sxs-lookup"><span data-stu-id="d5e32-108">Method</span></span>           | <span data-ttu-id="d5e32-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5e32-109">Return Type</span></span>    |<span data-ttu-id="d5e32-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e32-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d5e32-111">Get RangeFormat</span><span class="sxs-lookup"><span data-stu-id="d5e32-111">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="d5e32-112">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="d5e32-112">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="d5e32-113">Leia as propriedades e relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="d5e32-113">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="d5e32-114">Create RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d5e32-114">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="d5e32-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d5e32-115">RangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="d5e32-116">Crie uma nova RangeBorder postando na coleção de bordas.</span><span class="sxs-lookup"><span data-stu-id="d5e32-116">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="d5e32-117">List borders</span><span class="sxs-lookup"><span data-stu-id="d5e32-117">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="d5e32-118">Coleção [RangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="d5e32-118">[RangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="d5e32-119">Obtenha uma coleção de objetos RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="d5e32-119">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="d5e32-120">Update</span><span class="sxs-lookup"><span data-stu-id="d5e32-120">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="d5e32-121">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="d5e32-121">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="d5e32-122">Atualize o objeto RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="d5e32-122">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="d5e32-123">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="d5e32-123">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="d5e32-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5e32-124">None</span></span>|<span data-ttu-id="d5e32-125">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="d5e32-125">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="d5e32-126">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="d5e32-126">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="d5e32-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5e32-127">None</span></span>|<span data-ttu-id="d5e32-128">Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="d5e32-128">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5e32-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5e32-129">Properties</span></span>
| <span data-ttu-id="d5e32-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5e32-130">Property</span></span>     | <span data-ttu-id="d5e32-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5e32-131">Type</span></span>   |<span data-ttu-id="d5e32-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e32-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5e32-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="d5e32-133">columnWidth</span></span>|<span data-ttu-id="d5e32-134">double</span><span class="sxs-lookup"><span data-stu-id="d5e32-134">double</span></span>|<span data-ttu-id="d5e32-p102">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="d5e32-p102">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="d5e32-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="d5e32-137">horizontalAlignment</span></span>|<span data-ttu-id="d5e32-138">string</span><span class="sxs-lookup"><span data-stu-id="d5e32-138">string</span></span>|<span data-ttu-id="d5e32-p103">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="d5e32-p103">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="d5e32-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="d5e32-141">rowHeight</span></span>|<span data-ttu-id="d5e32-142">double</span><span class="sxs-lookup"><span data-stu-id="d5e32-142">double</span></span>|<span data-ttu-id="d5e32-p104">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="d5e32-p104">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="d5e32-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="d5e32-145">verticalAlignment</span></span>|<span data-ttu-id="d5e32-146">string</span><span class="sxs-lookup"><span data-stu-id="d5e32-146">string</span></span>|<span data-ttu-id="d5e32-p105">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="d5e32-p105">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="d5e32-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="d5e32-149">wrapText</span></span>|<span data-ttu-id="d5e32-150">booliano</span><span class="sxs-lookup"><span data-stu-id="d5e32-150">boolean</span></span>|<span data-ttu-id="d5e32-p106">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="d5e32-p106">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5e32-153">Relações</span><span class="sxs-lookup"><span data-stu-id="d5e32-153">Relationships</span></span>
| <span data-ttu-id="d5e32-154">Relação</span><span class="sxs-lookup"><span data-stu-id="d5e32-154">Relationship</span></span> | <span data-ttu-id="d5e32-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5e32-155">Type</span></span>   |<span data-ttu-id="d5e32-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e32-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5e32-157">borders</span><span class="sxs-lookup"><span data-stu-id="d5e32-157">borders</span></span>|<span data-ttu-id="d5e32-158">Coleção [RangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="d5e32-158">[RangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="d5e32-159">Coleção de objetos de borda que se aplicam a todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5e32-159">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="d5e32-160">fill</span><span class="sxs-lookup"><span data-stu-id="d5e32-160">fill</span></span>|[<span data-ttu-id="d5e32-161">RangeFill</span><span class="sxs-lookup"><span data-stu-id="d5e32-161">RangeFill</span></span>](rangefill.md)|<span data-ttu-id="d5e32-p107">Retorna o objeto de preenchimento definido em todo o intervalo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5e32-p107">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="d5e32-164">font</span><span class="sxs-lookup"><span data-stu-id="d5e32-164">font</span></span>|[<span data-ttu-id="d5e32-165">RangeFont</span><span class="sxs-lookup"><span data-stu-id="d5e32-165">RangeFont</span></span>](rangefont.md)|<span data-ttu-id="d5e32-166">Retorna o objeto Font definido em todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5e32-166">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="d5e32-167">protection</span><span class="sxs-lookup"><span data-stu-id="d5e32-167">protection</span></span>|[<span data-ttu-id="d5e32-168">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="d5e32-168">FormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="d5e32-p108">Retorna o objeto de proteção de formato para um intervalo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5e32-p108">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5e32-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5e32-171">JSON representation</span></span>

<span data-ttu-id="d5e32-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5e32-172">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
