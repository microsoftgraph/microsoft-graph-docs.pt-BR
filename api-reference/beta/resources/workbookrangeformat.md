---
title: tipo de recurso workbookRangeFormat
description: Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 3ee55e1a398dab1727dfdc24d9ebd5c66b7440d3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348532"
---
# <a name="workbookrangeformat-resource-type"></a><span data-ttu-id="777ec-103">tipo de recurso workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="777ec-103">workbookRangeFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="777ec-104">Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.</span><span class="sxs-lookup"><span data-stu-id="777ec-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="777ec-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="777ec-105">Methods</span></span>

| <span data-ttu-id="777ec-106">Método</span><span class="sxs-lookup"><span data-stu-id="777ec-106">Method</span></span>           | <span data-ttu-id="777ec-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="777ec-107">Return Type</span></span>    |<span data-ttu-id="777ec-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="777ec-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="777ec-109">Obter workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="777ec-109">Get workbookRangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="777ec-110">workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="777ec-110">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="777ec-111">Leia as propriedades e relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="777ec-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="777ec-112">Criar workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="777ec-112">Create workbookRangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="777ec-113">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="777ec-113">workbookRangeBorder</span></span>](workbookrangeborder.md)| <span data-ttu-id="777ec-114">Crie uma nova RangeBorder postando na coleção de bordas.</span><span class="sxs-lookup"><span data-stu-id="777ec-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="777ec-115">List borders</span><span class="sxs-lookup"><span data-stu-id="777ec-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="777ec-116">coleção [workbookRangeBorder](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="777ec-116">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>| <span data-ttu-id="777ec-117">Obtenha uma coleção de objetos RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="777ec-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="777ec-118">Update</span><span class="sxs-lookup"><span data-stu-id="777ec-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="777ec-119">workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="777ec-119">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="777ec-120">Atualize o objeto RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="777ec-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="777ec-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="777ec-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="777ec-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="777ec-122">None</span></span>|<span data-ttu-id="777ec-123">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="777ec-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="777ec-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="777ec-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="777ec-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="777ec-125">None</span></span>|<span data-ttu-id="777ec-126">Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="777ec-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="777ec-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="777ec-127">Properties</span></span>
| <span data-ttu-id="777ec-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="777ec-128">Property</span></span>     | <span data-ttu-id="777ec-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="777ec-129">Type</span></span>   |<span data-ttu-id="777ec-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="777ec-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="777ec-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="777ec-131">columnWidth</span></span>|<span data-ttu-id="777ec-132">double</span><span class="sxs-lookup"><span data-stu-id="777ec-132">double</span></span>|<span data-ttu-id="777ec-p101">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="777ec-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="777ec-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="777ec-135">horizontalAlignment</span></span>|<span data-ttu-id="777ec-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="777ec-136">string</span></span>|<span data-ttu-id="777ec-p102">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="777ec-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="777ec-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="777ec-139">rowHeight</span></span>|<span data-ttu-id="777ec-140">duplo</span><span class="sxs-lookup"><span data-stu-id="777ec-140">double</span></span>|<span data-ttu-id="777ec-p103">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="777ec-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="777ec-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="777ec-143">verticalAlignment</span></span>|<span data-ttu-id="777ec-144">string</span><span class="sxs-lookup"><span data-stu-id="777ec-144">string</span></span>|<span data-ttu-id="777ec-p104">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="777ec-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="777ec-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="777ec-147">wrapText</span></span>|<span data-ttu-id="777ec-148">booliano</span><span class="sxs-lookup"><span data-stu-id="777ec-148">boolean</span></span>|<span data-ttu-id="777ec-p105">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="777ec-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="777ec-151">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="777ec-151">Relationships</span></span>
| <span data-ttu-id="777ec-152">Relação</span><span class="sxs-lookup"><span data-stu-id="777ec-152">Relationship</span></span> | <span data-ttu-id="777ec-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="777ec-153">Type</span></span>   |<span data-ttu-id="777ec-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="777ec-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="777ec-155">Borders</span><span class="sxs-lookup"><span data-stu-id="777ec-155">borders</span></span>|<span data-ttu-id="777ec-156">coleção [workbookRangeBorder](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="777ec-156">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>|<span data-ttu-id="777ec-157">Coleção de objetos de borda que se aplicam a todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="777ec-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="777ec-158">fill</span><span class="sxs-lookup"><span data-stu-id="777ec-158">fill</span></span>|[<span data-ttu-id="777ec-159">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="777ec-159">workbookRangeFill</span></span>](workbookrangefill.md)|<span data-ttu-id="777ec-p106">Retorna o objeto de preenchimento definido em todo o intervalo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="777ec-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="777ec-162">font</span><span class="sxs-lookup"><span data-stu-id="777ec-162">font</span></span>|[<span data-ttu-id="777ec-163">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="777ec-163">workbookRangeFont</span></span>](workbookrangefont.md)|<span data-ttu-id="777ec-164">Retorna o objeto Font definido em todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="777ec-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="777ec-165">protection</span><span class="sxs-lookup"><span data-stu-id="777ec-165">protection</span></span>|[<span data-ttu-id="777ec-166">formatProtection</span><span class="sxs-lookup"><span data-stu-id="777ec-166">formatProtection</span></span>](formatprotection.md)|<span data-ttu-id="777ec-167">Retorna o objeto de proteção de formato para um intervalo.</span><span class="sxs-lookup"><span data-stu-id="777ec-167">Returns the format protection object for a range.</span></span> <span data-ttu-id="777ec-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="777ec-168">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="777ec-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="777ec-169">JSON representation</span></span>

<span data-ttu-id="777ec-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="777ec-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
