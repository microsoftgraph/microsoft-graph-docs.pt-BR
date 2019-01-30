---
title: Tipo de recurso Worksheet
description: Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: beffb9747045d0d3792d994237710e886ff0b3d8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640921"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="626f8-104">Tipo de recurso Worksheet</span><span class="sxs-lookup"><span data-stu-id="626f8-104">Worksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="626f8-p102">Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.</span><span class="sxs-lookup"><span data-stu-id="626f8-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="626f8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="626f8-107">Methods</span></span>

| <span data-ttu-id="626f8-108">Método</span><span class="sxs-lookup"><span data-stu-id="626f8-108">Method</span></span>           | <span data-ttu-id="626f8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="626f8-109">Return Type</span></span>    |<span data-ttu-id="626f8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="626f8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="626f8-111">Get Worksheet</span><span class="sxs-lookup"><span data-stu-id="626f8-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="626f8-112">Worksheet</span><span class="sxs-lookup"><span data-stu-id="626f8-112">Worksheet</span></span>](worksheet.md) |<span data-ttu-id="626f8-113">Leia as propriedades e os relacionamentos do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="626f8-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="626f8-114">Create Chart</span><span class="sxs-lookup"><span data-stu-id="626f8-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="626f8-115">Chart</span><span class="sxs-lookup"><span data-stu-id="626f8-115">Chart</span></span>](chart.md)| <span data-ttu-id="626f8-116">Crie um novo Gráfico ao postar na coleção de gráficos.</span><span class="sxs-lookup"><span data-stu-id="626f8-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="626f8-117">Nomes da lista</span><span class="sxs-lookup"><span data-stu-id="626f8-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="626f8-118">Coleção [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="626f8-118">[NamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="626f8-119">Faça com que a coleção de itens nomeados seja associada à planilha.</span><span class="sxs-lookup"><span data-stu-id="626f8-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="626f8-120">Listar gráficos</span><span class="sxs-lookup"><span data-stu-id="626f8-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="626f8-121">Coleção [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="626f8-121">[Chart](chart.md) collection</span></span>| <span data-ttu-id="626f8-122">Obtenha a coleção de objetos Chart.</span><span class="sxs-lookup"><span data-stu-id="626f8-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="626f8-123">Create Table</span><span class="sxs-lookup"><span data-stu-id="626f8-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="626f8-124">Table</span><span class="sxs-lookup"><span data-stu-id="626f8-124">Table</span></span>](table.md)| <span data-ttu-id="626f8-125">Crie uma nova Table postando na coleção de tabelas.</span><span class="sxs-lookup"><span data-stu-id="626f8-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="626f8-126">List tables</span><span class="sxs-lookup"><span data-stu-id="626f8-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="626f8-127">Coleção [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="626f8-127">[Table](table.md) collection</span></span>| <span data-ttu-id="626f8-128">Obtenha uma coleção de objetos Table.</span><span class="sxs-lookup"><span data-stu-id="626f8-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="626f8-129">Update</span><span class="sxs-lookup"><span data-stu-id="626f8-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="626f8-130">Worksheet</span><span class="sxs-lookup"><span data-stu-id="626f8-130">Worksheet</span></span>](worksheet.md)   |<span data-ttu-id="626f8-131">Atualize o objeto Worksheet.</span><span class="sxs-lookup"><span data-stu-id="626f8-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="626f8-132">Cell</span><span class="sxs-lookup"><span data-stu-id="626f8-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="626f8-133">Range</span><span class="sxs-lookup"><span data-stu-id="626f8-133">Range</span></span>](range.md)|<span data-ttu-id="626f8-p103">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="626f8-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="626f8-136">Range</span><span class="sxs-lookup"><span data-stu-id="626f8-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="626f8-137">Range</span><span class="sxs-lookup"><span data-stu-id="626f8-137">Range</span></span>](range.md)|<span data-ttu-id="626f8-138">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="626f8-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="626f8-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="626f8-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="626f8-140">Range</span><span class="sxs-lookup"><span data-stu-id="626f8-140">Range</span></span>](range.md)|<span data-ttu-id="626f8-p104">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="626f8-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="626f8-143">Delete</span><span class="sxs-lookup"><span data-stu-id="626f8-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="626f8-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="626f8-144">None</span></span>|<span data-ttu-id="626f8-145">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="626f8-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="626f8-146">List</span><span class="sxs-lookup"><span data-stu-id="626f8-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="626f8-147">Coleção [Worksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="626f8-147">[Worksheet](worksheet.md) collection</span></span> |<span data-ttu-id="626f8-148">Obtenha a coleção de objetos da planilha.</span><span class="sxs-lookup"><span data-stu-id="626f8-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="626f8-149">Add</span><span class="sxs-lookup"><span data-stu-id="626f8-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="626f8-150">Worksheet</span><span class="sxs-lookup"><span data-stu-id="626f8-150">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="626f8-p105">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes.</span><span class="sxs-lookup"><span data-stu-id="626f8-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="626f8-153">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="626f8-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="626f8-154">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="626f8-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="626f8-155">Obtenha uma coleção de objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="626f8-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="626f8-156">Propriedades</span><span class="sxs-lookup"><span data-stu-id="626f8-156">Properties</span></span>
| <span data-ttu-id="626f8-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="626f8-157">Property</span></span>     | <span data-ttu-id="626f8-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="626f8-158">Type</span></span>   |<span data-ttu-id="626f8-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="626f8-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="626f8-160">id</span><span class="sxs-lookup"><span data-stu-id="626f8-160">id</span></span>|<span data-ttu-id="626f8-161">string</span><span class="sxs-lookup"><span data-stu-id="626f8-161">string</span></span>|<span data-ttu-id="626f8-p106">Retorna um valor que identifica de forma exclusiva a planilha em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a planilha seja renomeada ou movida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="626f8-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="626f8-165">name</span><span class="sxs-lookup"><span data-stu-id="626f8-165">name</span></span>|<span data-ttu-id="626f8-166">string</span><span class="sxs-lookup"><span data-stu-id="626f8-166">string</span></span>|<span data-ttu-id="626f8-167">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="626f8-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="626f8-168">position</span><span class="sxs-lookup"><span data-stu-id="626f8-168">position</span></span>|<span data-ttu-id="626f8-169">int</span><span class="sxs-lookup"><span data-stu-id="626f8-169">int</span></span>|<span data-ttu-id="626f8-170">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="626f8-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="626f8-171">visibilidade</span><span class="sxs-lookup"><span data-stu-id="626f8-171">visibility</span></span>|<span data-ttu-id="626f8-172">string</span><span class="sxs-lookup"><span data-stu-id="626f8-172">string</span></span>|<span data-ttu-id="626f8-p107">A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="626f8-p107">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="626f8-175">Relações</span><span class="sxs-lookup"><span data-stu-id="626f8-175">Relationships</span></span>
| <span data-ttu-id="626f8-176">Relação</span><span class="sxs-lookup"><span data-stu-id="626f8-176">Relationship</span></span> | <span data-ttu-id="626f8-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="626f8-177">Type</span></span>   |<span data-ttu-id="626f8-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="626f8-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="626f8-179">charts</span><span class="sxs-lookup"><span data-stu-id="626f8-179">charts</span></span>|<span data-ttu-id="626f8-180">Coleção [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="626f8-180">[Chart](chart.md) collection</span></span>|<span data-ttu-id="626f8-p108">Retorna uma coleção de gráficos que fazem parte da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="626f8-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="626f8-183">names</span><span class="sxs-lookup"><span data-stu-id="626f8-183">names</span></span>|<span data-ttu-id="626f8-184">Coleção [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="626f8-184">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="626f8-p109">Retorna a coleção de nomes associados à planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="626f8-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="626f8-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="626f8-187">pivotTables</span></span>|<span data-ttu-id="626f8-188">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="626f8-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="626f8-189">Coleção de Tabelas Dinâmicas que fazem parte da planilha.</span><span class="sxs-lookup"><span data-stu-id="626f8-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="626f8-190">protection</span><span class="sxs-lookup"><span data-stu-id="626f8-190">protection</span></span>|[<span data-ttu-id="626f8-191">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="626f8-191">WorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="626f8-p110">Retorna o objeto de proteção da planilha para uma planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="626f8-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="626f8-194">tables</span><span class="sxs-lookup"><span data-stu-id="626f8-194">tables</span></span>|<span data-ttu-id="626f8-195">Coleção [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="626f8-195">[Table](table.md) collection</span></span>|<span data-ttu-id="626f8-p111">Coleção de tabelas que fazem parte da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="626f8-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="626f8-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="626f8-198">JSON representation</span></span>

<span data-ttu-id="626f8-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="626f8-199">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
