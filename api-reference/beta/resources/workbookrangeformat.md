---
title: tipo de recurso workbookRangeFormat
description: Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6ec27300e720892debbd458970063f1b79270597
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007064"
---
# <a name="workbookrangeformat-resource-type"></a><span data-ttu-id="8aab3-103">tipo de recurso workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="8aab3-103">workbookRangeFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aab3-104">Um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.</span><span class="sxs-lookup"><span data-stu-id="8aab3-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="8aab3-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8aab3-105">Methods</span></span>

| <span data-ttu-id="8aab3-106">Método</span><span class="sxs-lookup"><span data-stu-id="8aab3-106">Method</span></span>           | <span data-ttu-id="8aab3-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8aab3-107">Return Type</span></span>    |<span data-ttu-id="8aab3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aab3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8aab3-109">Obter workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="8aab3-109">Get workbookRangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="8aab3-110">workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="8aab3-110">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="8aab3-111">Leia as propriedades e relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="8aab3-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="8aab3-112">Criar workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="8aab3-112">Create workbookRangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="8aab3-113">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="8aab3-113">workbookRangeBorder</span></span>](workbookrangeborder.md)| <span data-ttu-id="8aab3-114">Crie uma nova RangeBorder postando na coleção de bordas.</span><span class="sxs-lookup"><span data-stu-id="8aab3-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="8aab3-115">List borders</span><span class="sxs-lookup"><span data-stu-id="8aab3-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="8aab3-116">coleção [workbookRangeBorder](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="8aab3-116">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>| <span data-ttu-id="8aab3-117">Obtenha uma coleção de objetos RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="8aab3-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="8aab3-118">Update</span><span class="sxs-lookup"><span data-stu-id="8aab3-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="8aab3-119">workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="8aab3-119">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="8aab3-120">Atualize o objeto RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="8aab3-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="8aab3-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="8aab3-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="8aab3-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8aab3-122">None</span></span>|<span data-ttu-id="8aab3-123">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="8aab3-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="8aab3-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="8aab3-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="8aab3-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8aab3-125">None</span></span>|<span data-ttu-id="8aab3-126">Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="8aab3-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="8aab3-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8aab3-127">Properties</span></span>
| <span data-ttu-id="8aab3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8aab3-128">Property</span></span>     | <span data-ttu-id="8aab3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aab3-129">Type</span></span>   |<span data-ttu-id="8aab3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aab3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8aab3-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="8aab3-131">columnWidth</span></span>|<span data-ttu-id="8aab3-132">double</span><span class="sxs-lookup"><span data-stu-id="8aab3-132">double</span></span>|<span data-ttu-id="8aab3-p101">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="8aab3-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="8aab3-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="8aab3-135">horizontalAlignment</span></span>|<span data-ttu-id="8aab3-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aab3-136">string</span></span>|<span data-ttu-id="8aab3-p102">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="8aab3-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="8aab3-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="8aab3-139">rowHeight</span></span>|<span data-ttu-id="8aab3-140">duplo</span><span class="sxs-lookup"><span data-stu-id="8aab3-140">double</span></span>|<span data-ttu-id="8aab3-p103">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="8aab3-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="8aab3-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="8aab3-143">verticalAlignment</span></span>|<span data-ttu-id="8aab3-144">string</span><span class="sxs-lookup"><span data-stu-id="8aab3-144">string</span></span>|<span data-ttu-id="8aab3-p104">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="8aab3-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="8aab3-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="8aab3-147">wrapText</span></span>|<span data-ttu-id="8aab3-148">booliano</span><span class="sxs-lookup"><span data-stu-id="8aab3-148">boolean</span></span>|<span data-ttu-id="8aab3-p105">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="8aab3-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="8aab3-151">Relações</span><span class="sxs-lookup"><span data-stu-id="8aab3-151">Relationships</span></span>
| <span data-ttu-id="8aab3-152">Relação</span><span class="sxs-lookup"><span data-stu-id="8aab3-152">Relationship</span></span> | <span data-ttu-id="8aab3-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aab3-153">Type</span></span>   |<span data-ttu-id="8aab3-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aab3-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8aab3-155">Borders</span><span class="sxs-lookup"><span data-stu-id="8aab3-155">borders</span></span>|<span data-ttu-id="8aab3-156">coleção [workbookRangeBorder](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="8aab3-156">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>|<span data-ttu-id="8aab3-157">Coleção de objetos de borda que se aplicam a todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8aab3-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="8aab3-158">fill</span><span class="sxs-lookup"><span data-stu-id="8aab3-158">fill</span></span>|[<span data-ttu-id="8aab3-159">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="8aab3-159">workbookRangeFill</span></span>](workbookrangefill.md)|<span data-ttu-id="8aab3-p106">Retorna o objeto de preenchimento definido em todo o intervalo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8aab3-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="8aab3-162">font</span><span class="sxs-lookup"><span data-stu-id="8aab3-162">font</span></span>|[<span data-ttu-id="8aab3-163">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="8aab3-163">workbookRangeFont</span></span>](workbookrangefont.md)|<span data-ttu-id="8aab3-164">Retorna o objeto Font definido em todo o intervalo selecionado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8aab3-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="8aab3-165">protection</span><span class="sxs-lookup"><span data-stu-id="8aab3-165">protection</span></span>|[<span data-ttu-id="8aab3-166">formatProtection</span><span class="sxs-lookup"><span data-stu-id="8aab3-166">formatProtection</span></span>](formatprotection.md)|<span data-ttu-id="8aab3-167">Retorna o objeto de proteção de formato para um intervalo.</span><span class="sxs-lookup"><span data-stu-id="8aab3-167">Returns the format protection object for a range.</span></span> <span data-ttu-id="8aab3-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8aab3-168">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8aab3-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8aab3-169">JSON representation</span></span>

<span data-ttu-id="8aab3-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8aab3-170">Here is a JSON representation of the resource.</span></span>

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
