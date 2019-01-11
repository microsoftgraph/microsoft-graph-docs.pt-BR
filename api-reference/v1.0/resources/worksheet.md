---
title: Tipo de recurso Worksheet
description: Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.
localization_priority: Priority
ms.openlocfilehash: 50d531aee3ed242f30be2c225ae9cd38bd6c6e89
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884809"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="d2c2a-104">Tipo de recurso Worksheet</span><span class="sxs-lookup"><span data-stu-id="d2c2a-104">Worksheet resource type</span></span>

<span data-ttu-id="d2c2a-p102">Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="d2c2a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2c2a-107">Methods</span></span>

| <span data-ttu-id="d2c2a-108">Método</span><span class="sxs-lookup"><span data-stu-id="d2c2a-108">Method</span></span>           | <span data-ttu-id="d2c2a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d2c2a-109">Return Type</span></span>    |<span data-ttu-id="d2c2a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2c2a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2c2a-111">Get Worksheet</span><span class="sxs-lookup"><span data-stu-id="d2c2a-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="d2c2a-112">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d2c2a-112">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="d2c2a-113">Leia as propriedades e os relacionamentos do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="d2c2a-114">Create Chart</span><span class="sxs-lookup"><span data-stu-id="d2c2a-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="d2c2a-115">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="d2c2a-115">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="d2c2a-116">Crie um novo Gráfico ao postar na coleção de gráficos.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="d2c2a-117">Nomes da lista</span><span class="sxs-lookup"><span data-stu-id="d2c2a-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="d2c2a-118">Coleção [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="d2c2a-118">[WorkbookNamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="d2c2a-119">Faça com que a coleção de itens nomeados seja associada à planilha.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="d2c2a-120">Listar gráficos</span><span class="sxs-lookup"><span data-stu-id="d2c2a-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="d2c2a-121">Coleção [WorkbookChart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="d2c2a-121">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="d2c2a-122">Obtenha a coleção de objetos Chart.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="d2c2a-123">Create Table</span><span class="sxs-lookup"><span data-stu-id="d2c2a-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="d2c2a-124">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="d2c2a-124">WorkbookTable</span></span>](table.md)| <span data-ttu-id="d2c2a-125">Crie uma nova Table postando na coleção de tabelas.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="d2c2a-126">List tables</span><span class="sxs-lookup"><span data-stu-id="d2c2a-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="d2c2a-127">Coleção [WorkbookTable](table.md)</span><span class="sxs-lookup"><span data-stu-id="d2c2a-127">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="d2c2a-128">Obtenha uma coleção de objetos Table.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="d2c2a-129">Update</span><span class="sxs-lookup"><span data-stu-id="d2c2a-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="d2c2a-130">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d2c2a-130">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="d2c2a-131">Atualize o objeto Worksheet.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="d2c2a-132">Cell</span><span class="sxs-lookup"><span data-stu-id="d2c2a-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="d2c2a-133">Range</span><span class="sxs-lookup"><span data-stu-id="d2c2a-133">Range</span></span>](range.md)|<span data-ttu-id="d2c2a-p103">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="d2c2a-136">Range</span><span class="sxs-lookup"><span data-stu-id="d2c2a-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="d2c2a-137">Range</span><span class="sxs-lookup"><span data-stu-id="d2c2a-137">Range</span></span>](range.md)|<span data-ttu-id="d2c2a-138">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="d2c2a-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="d2c2a-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="d2c2a-140">Range</span><span class="sxs-lookup"><span data-stu-id="d2c2a-140">Range</span></span>](range.md)|<span data-ttu-id="d2c2a-p104">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="d2c2a-143">Delete</span><span class="sxs-lookup"><span data-stu-id="d2c2a-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="d2c2a-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2c2a-144">None</span></span>|<span data-ttu-id="d2c2a-145">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="d2c2a-146">List</span><span class="sxs-lookup"><span data-stu-id="d2c2a-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="d2c2a-147">Coleção [WorkbookWorksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="d2c2a-147">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="d2c2a-148">Obtenha a coleção de objetos da planilha.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="d2c2a-149">Add</span><span class="sxs-lookup"><span data-stu-id="d2c2a-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="d2c2a-150">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d2c2a-150">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="d2c2a-p105">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="d2c2a-153">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="d2c2a-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="d2c2a-154">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="d2c2a-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d2c2a-155">Obtenha uma coleção de objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2c2a-156">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2c2a-156">Properties</span></span>
| <span data-ttu-id="d2c2a-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2c2a-157">Property</span></span>     | <span data-ttu-id="d2c2a-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2c2a-158">Type</span></span>   |<span data-ttu-id="d2c2a-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2c2a-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2c2a-160">id</span><span class="sxs-lookup"><span data-stu-id="d2c2a-160">id</span></span>|<span data-ttu-id="d2c2a-161">string</span><span class="sxs-lookup"><span data-stu-id="d2c2a-161">string</span></span>|<span data-ttu-id="d2c2a-p106">Retorna um valor que identifica de forma exclusiva a planilha em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a planilha seja renomeada ou movida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="d2c2a-165">name</span><span class="sxs-lookup"><span data-stu-id="d2c2a-165">name</span></span>|<span data-ttu-id="d2c2a-166">string</span><span class="sxs-lookup"><span data-stu-id="d2c2a-166">string</span></span>|<span data-ttu-id="d2c2a-167">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="d2c2a-168">position</span><span class="sxs-lookup"><span data-stu-id="d2c2a-168">position</span></span>|<span data-ttu-id="d2c2a-169">int</span><span class="sxs-lookup"><span data-stu-id="d2c2a-169">int</span></span>|<span data-ttu-id="d2c2a-170">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="d2c2a-171">visibilidade</span><span class="sxs-lookup"><span data-stu-id="d2c2a-171">visibility</span></span>|<span data-ttu-id="d2c2a-172">string</span><span class="sxs-lookup"><span data-stu-id="d2c2a-172">string</span></span>|<span data-ttu-id="d2c2a-173">A visibilidade da planilha.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="d2c2a-174">Os valores possíveis são: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2c2a-175">Relações</span><span class="sxs-lookup"><span data-stu-id="d2c2a-175">Relationships</span></span>
| <span data-ttu-id="d2c2a-176">Relação</span><span class="sxs-lookup"><span data-stu-id="d2c2a-176">Relationship</span></span> | <span data-ttu-id="d2c2a-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2c2a-177">Type</span></span>   |<span data-ttu-id="d2c2a-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2c2a-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2c2a-179">charts</span><span class="sxs-lookup"><span data-stu-id="d2c2a-179">charts</span></span>|<span data-ttu-id="d2c2a-180">Coleção [WorkbookChart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="d2c2a-180">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="d2c2a-p108">Retorna uma coleção de gráficos que fazem parte da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="d2c2a-183">names</span><span class="sxs-lookup"><span data-stu-id="d2c2a-183">names</span></span>|<span data-ttu-id="d2c2a-184">Coleção [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="d2c2a-184">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="d2c2a-p109">Retorna a coleção de nomes associados à planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="d2c2a-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="d2c2a-187">pivotTables</span></span>|<span data-ttu-id="d2c2a-188">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="d2c2a-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d2c2a-189">Coleção de Tabelas Dinâmicas que fazem parte da planilha.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="d2c2a-190">protection</span><span class="sxs-lookup"><span data-stu-id="d2c2a-190">protection</span></span>|[<span data-ttu-id="d2c2a-191">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d2c2a-191">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="d2c2a-p110">Retorna o objeto de proteção da planilha para uma planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="d2c2a-194">tables</span><span class="sxs-lookup"><span data-stu-id="d2c2a-194">tables</span></span>|<span data-ttu-id="d2c2a-195">Coleção [WorkbookTable](table.md)</span><span class="sxs-lookup"><span data-stu-id="d2c2a-195">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="d2c2a-p111">Coleção de tabelas que fazem parte da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2c2a-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2c2a-198">JSON representation</span></span>

<span data-ttu-id="d2c2a-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2c2a-199">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
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
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
