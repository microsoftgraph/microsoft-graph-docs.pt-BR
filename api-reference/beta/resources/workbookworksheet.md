---
title: tipo de recurso workbookWorksheet
description: Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 93386edf60e30069068ceb2fa437fb128b239302
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963854"
---
# <a name="workbookworksheet-resource-type"></a><span data-ttu-id="d321e-104">tipo de recurso workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d321e-104">workbookWorksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d321e-105">Uma planilha do Excel é uma grade de células.</span><span class="sxs-lookup"><span data-stu-id="d321e-105">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="d321e-106">Ela pode conter dados, tabelas, gráficos, etc.</span><span class="sxs-lookup"><span data-stu-id="d321e-106">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="d321e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d321e-107">Methods</span></span>

| <span data-ttu-id="d321e-108">Método</span><span class="sxs-lookup"><span data-stu-id="d321e-108">Method</span></span>           | <span data-ttu-id="d321e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d321e-109">Return Type</span></span>    |<span data-ttu-id="d321e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d321e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d321e-111">Get Worksheet</span><span class="sxs-lookup"><span data-stu-id="d321e-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="d321e-112">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d321e-112">workbookWorksheet</span></span>](workbookworksheet.md) |<span data-ttu-id="d321e-113">Leia as propriedades e os relacionamentos do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="d321e-114">Create Chart</span><span class="sxs-lookup"><span data-stu-id="d321e-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="d321e-115">workbookChart</span><span class="sxs-lookup"><span data-stu-id="d321e-115">workbookChart</span></span>](workbookchart.md)| <span data-ttu-id="d321e-116">Crie um novo Gráfico ao postar na coleção de gráficos.</span><span class="sxs-lookup"><span data-stu-id="d321e-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="d321e-117">Nomes da lista</span><span class="sxs-lookup"><span data-stu-id="d321e-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="d321e-118">coleção [workbookNamedItem](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="d321e-118">[workbookNamedItem](workbooknameditem.md) collection</span></span>| <span data-ttu-id="d321e-119">Faça com que a coleção de itens nomeados seja associada à planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="d321e-120">Listar gráficos</span><span class="sxs-lookup"><span data-stu-id="d321e-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="d321e-121">coleção [workbookChart](workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="d321e-121">[workbookChart](workbookchart.md) collection</span></span>| <span data-ttu-id="d321e-122">Obtenha a coleção de objetos Chart.</span><span class="sxs-lookup"><span data-stu-id="d321e-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="d321e-123">Create Table</span><span class="sxs-lookup"><span data-stu-id="d321e-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="d321e-124">workbooktable</span><span class="sxs-lookup"><span data-stu-id="d321e-124">workbookTable</span></span>](workbooktable.md)| <span data-ttu-id="d321e-125">Crie uma nova Table postando na coleção de tabelas.</span><span class="sxs-lookup"><span data-stu-id="d321e-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="d321e-126">List tables</span><span class="sxs-lookup"><span data-stu-id="d321e-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="d321e-127">[](workbooktable.md) coleção workbooktable</span><span class="sxs-lookup"><span data-stu-id="d321e-127">[workbookTable](workbooktable.md) collection</span></span>| <span data-ttu-id="d321e-128">Obtenha uma coleção de objetos Table.</span><span class="sxs-lookup"><span data-stu-id="d321e-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="d321e-129">Atualização</span><span class="sxs-lookup"><span data-stu-id="d321e-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="d321e-130">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d321e-130">workbookWorksheet</span></span>](workbookworksheet.md)   |<span data-ttu-id="d321e-131">Atualize o objeto Worksheet.</span><span class="sxs-lookup"><span data-stu-id="d321e-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="d321e-132">Cell</span><span class="sxs-lookup"><span data-stu-id="d321e-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="d321e-133">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d321e-133">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d321e-p103">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="d321e-136">Range</span><span class="sxs-lookup"><span data-stu-id="d321e-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="d321e-137">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d321e-137">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d321e-138">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="d321e-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="d321e-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="d321e-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="d321e-140">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d321e-140">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d321e-p104">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="d321e-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="d321e-143">Delete</span><span class="sxs-lookup"><span data-stu-id="d321e-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="d321e-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d321e-144">None</span></span>|<span data-ttu-id="d321e-145">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d321e-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="d321e-146">List</span><span class="sxs-lookup"><span data-stu-id="d321e-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="d321e-147">coleção [workbookWorksheet](workbookworksheet.md)</span><span class="sxs-lookup"><span data-stu-id="d321e-147">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="d321e-148">Obtenha a coleção de objetos da planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="d321e-149">Add</span><span class="sxs-lookup"><span data-stu-id="d321e-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="d321e-150">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d321e-150">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="d321e-p105">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes.</span><span class="sxs-lookup"><span data-stu-id="d321e-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="d321e-153">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="d321e-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="d321e-154">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="d321e-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d321e-155">Obtenha uma coleção de objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="d321e-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d321e-156">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d321e-156">Properties</span></span>
| <span data-ttu-id="d321e-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d321e-157">Property</span></span>     | <span data-ttu-id="d321e-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="d321e-158">Type</span></span>   |<span data-ttu-id="d321e-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="d321e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d321e-160">id</span><span class="sxs-lookup"><span data-stu-id="d321e-160">id</span></span>|<span data-ttu-id="d321e-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d321e-161">string</span></span>|<span data-ttu-id="d321e-p106">Retorna um valor que identifica de forma exclusiva a planilha em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a planilha seja renomeada ou movida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d321e-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="d321e-165">name</span><span class="sxs-lookup"><span data-stu-id="d321e-165">name</span></span>|<span data-ttu-id="d321e-166">string</span><span class="sxs-lookup"><span data-stu-id="d321e-166">string</span></span>|<span data-ttu-id="d321e-167">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="d321e-168">position</span><span class="sxs-lookup"><span data-stu-id="d321e-168">position</span></span>|<span data-ttu-id="d321e-169">int</span><span class="sxs-lookup"><span data-stu-id="d321e-169">int</span></span>|<span data-ttu-id="d321e-170">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d321e-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="d321e-171">visibilidade</span><span class="sxs-lookup"><span data-stu-id="d321e-171">visibility</span></span>|<span data-ttu-id="d321e-172">string</span><span class="sxs-lookup"><span data-stu-id="d321e-172">string</span></span>|<span data-ttu-id="d321e-173">A visibilidade da planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="d321e-174">Os valores possíveis são: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="d321e-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d321e-175">Relações</span><span class="sxs-lookup"><span data-stu-id="d321e-175">Relationships</span></span>
| <span data-ttu-id="d321e-176">Relação</span><span class="sxs-lookup"><span data-stu-id="d321e-176">Relationship</span></span> | <span data-ttu-id="d321e-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="d321e-177">Type</span></span>   |<span data-ttu-id="d321e-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="d321e-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d321e-179">charts</span><span class="sxs-lookup"><span data-stu-id="d321e-179">charts</span></span>|<span data-ttu-id="d321e-180">coleção [workbookChart](workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="d321e-180">[workbookChart](workbookchart.md) collection</span></span>|<span data-ttu-id="d321e-181">Retorna uma coleção de gráficos que fazem parte da planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-181">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="d321e-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d321e-182">Read-only.</span></span>|
|<span data-ttu-id="d321e-183">names</span><span class="sxs-lookup"><span data-stu-id="d321e-183">names</span></span>|<span data-ttu-id="d321e-184">coleção [workbookNamedItem](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="d321e-184">[workbookNamedItem](workbooknameditem.md) collection</span></span>|<span data-ttu-id="d321e-185">Retorna a coleção de nomes associados à planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-185">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="d321e-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d321e-186">Read-only.</span></span>|
|<span data-ttu-id="d321e-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="d321e-187">pivotTables</span></span>|<span data-ttu-id="d321e-188">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="d321e-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d321e-189">Coleção de Tabelas Dinâmicas que fazem parte da planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="d321e-190">proteção</span><span class="sxs-lookup"><span data-stu-id="d321e-190">protection</span></span>|[<span data-ttu-id="d321e-191">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d321e-191">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md)|<span data-ttu-id="d321e-p110">Retorna o objeto de proteção da planilha para uma planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d321e-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="d321e-194">tables</span><span class="sxs-lookup"><span data-stu-id="d321e-194">tables</span></span>|<span data-ttu-id="d321e-195">[](workbooktable.md) coleção workbooktable</span><span class="sxs-lookup"><span data-stu-id="d321e-195">[workbookTable](workbooktable.md) collection</span></span>|<span data-ttu-id="d321e-196">Coleção de tabelas que fazem parte da planilha.</span><span class="sxs-lookup"><span data-stu-id="d321e-196">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="d321e-197">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d321e-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d321e-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d321e-198">JSON representation</span></span>

<span data-ttu-id="d321e-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d321e-199">Here is a JSON representation of the resource.</span></span>

<!-- {
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
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
