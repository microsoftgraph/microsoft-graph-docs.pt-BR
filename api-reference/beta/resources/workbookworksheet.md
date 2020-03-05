---
title: tipo de recurso workbookWorksheet
description: Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: edb6e13c975c0dc65c19604aef7256d63a409141
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519103"
---
# <a name="workbookworksheet-resource-type"></a><span data-ttu-id="0886b-104">tipo de recurso workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="0886b-104">workbookWorksheet resource type</span></span>

<span data-ttu-id="0886b-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0886b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0886b-106">Uma planilha do Excel é uma grade de células.</span><span class="sxs-lookup"><span data-stu-id="0886b-106">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="0886b-107">Ela pode conter dados, tabelas, gráficos, etc.</span><span class="sxs-lookup"><span data-stu-id="0886b-107">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="0886b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0886b-108">Methods</span></span>

| <span data-ttu-id="0886b-109">Método</span><span class="sxs-lookup"><span data-stu-id="0886b-109">Method</span></span>           | <span data-ttu-id="0886b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0886b-110">Return Type</span></span>    |<span data-ttu-id="0886b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0886b-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0886b-112">Get Worksheet</span><span class="sxs-lookup"><span data-stu-id="0886b-112">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="0886b-113">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="0886b-113">workbookWorksheet</span></span>](workbookworksheet.md) |<span data-ttu-id="0886b-114">Leia as propriedades e os relacionamentos do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-114">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="0886b-115">Create Chart</span><span class="sxs-lookup"><span data-stu-id="0886b-115">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="0886b-116">workbookChart</span><span class="sxs-lookup"><span data-stu-id="0886b-116">workbookChart</span></span>](workbookchart.md)| <span data-ttu-id="0886b-117">Crie um novo Gráfico ao postar na coleção de gráficos.</span><span class="sxs-lookup"><span data-stu-id="0886b-117">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="0886b-118">Nomes da lista</span><span class="sxs-lookup"><span data-stu-id="0886b-118">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="0886b-119">coleção [workbookNamedItem](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="0886b-119">[workbookNamedItem](workbooknameditem.md) collection</span></span>| <span data-ttu-id="0886b-120">Faça com que a coleção de itens nomeados seja associada à planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-120">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="0886b-121">Listar gráficos</span><span class="sxs-lookup"><span data-stu-id="0886b-121">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="0886b-122">coleção [workbookChart](workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="0886b-122">[workbookChart](workbookchart.md) collection</span></span>| <span data-ttu-id="0886b-123">Obtenha a coleção de objetos Chart.</span><span class="sxs-lookup"><span data-stu-id="0886b-123">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="0886b-124">Create Table</span><span class="sxs-lookup"><span data-stu-id="0886b-124">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="0886b-125">workbooktable</span><span class="sxs-lookup"><span data-stu-id="0886b-125">workbookTable</span></span>](workbooktable.md)| <span data-ttu-id="0886b-126">Crie uma nova Table postando na coleção de tabelas.</span><span class="sxs-lookup"><span data-stu-id="0886b-126">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="0886b-127">List tables</span><span class="sxs-lookup"><span data-stu-id="0886b-127">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="0886b-128">coleção [workbooktable](workbooktable.md)</span><span class="sxs-lookup"><span data-stu-id="0886b-128">[workbookTable](workbooktable.md) collection</span></span>| <span data-ttu-id="0886b-129">Obtenha uma coleção de objetos Table.</span><span class="sxs-lookup"><span data-stu-id="0886b-129">Get a Table object collection.</span></span>|
|[<span data-ttu-id="0886b-130">Atualização</span><span class="sxs-lookup"><span data-stu-id="0886b-130">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="0886b-131">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="0886b-131">workbookWorksheet</span></span>](workbookworksheet.md)   |<span data-ttu-id="0886b-132">Atualize o objeto Worksheet.</span><span class="sxs-lookup"><span data-stu-id="0886b-132">Update Worksheet object.</span></span> |
|[<span data-ttu-id="0886b-133">Cell</span><span class="sxs-lookup"><span data-stu-id="0886b-133">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="0886b-134">workbookRange</span><span class="sxs-lookup"><span data-stu-id="0886b-134">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="0886b-p103">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="0886b-137">Range</span><span class="sxs-lookup"><span data-stu-id="0886b-137">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="0886b-138">workbookRange</span><span class="sxs-lookup"><span data-stu-id="0886b-138">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="0886b-139">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="0886b-139">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="0886b-140">Usedrange</span><span class="sxs-lookup"><span data-stu-id="0886b-140">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="0886b-141">workbookRange</span><span class="sxs-lookup"><span data-stu-id="0886b-141">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="0886b-p104">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="0886b-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="0886b-144">Delete</span><span class="sxs-lookup"><span data-stu-id="0886b-144">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="0886b-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0886b-145">None</span></span>|<span data-ttu-id="0886b-146">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0886b-146">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="0886b-147">List</span><span class="sxs-lookup"><span data-stu-id="0886b-147">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="0886b-148">coleção [workbookWorksheet](workbookworksheet.md)</span><span class="sxs-lookup"><span data-stu-id="0886b-148">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="0886b-149">Obtenha a coleção de objetos da planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-149">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="0886b-150">Add</span><span class="sxs-lookup"><span data-stu-id="0886b-150">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="0886b-151">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="0886b-151">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="0886b-p105">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes.</span><span class="sxs-lookup"><span data-stu-id="0886b-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="0886b-154">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="0886b-154">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="0886b-155">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="0886b-155">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="0886b-156">Obtenha uma coleção de objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="0886b-156">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="0886b-157">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0886b-157">Properties</span></span>
| <span data-ttu-id="0886b-158">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0886b-158">Property</span></span>     | <span data-ttu-id="0886b-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="0886b-159">Type</span></span>   |<span data-ttu-id="0886b-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="0886b-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0886b-161">id</span><span class="sxs-lookup"><span data-stu-id="0886b-161">id</span></span>|<span data-ttu-id="0886b-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0886b-162">string</span></span>|<span data-ttu-id="0886b-p106">Retorna um valor que identifica de forma exclusiva a planilha em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a planilha seja renomeada ou movida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0886b-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="0886b-166">name</span><span class="sxs-lookup"><span data-stu-id="0886b-166">name</span></span>|<span data-ttu-id="0886b-167">string</span><span class="sxs-lookup"><span data-stu-id="0886b-167">string</span></span>|<span data-ttu-id="0886b-168">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-168">The display name of the worksheet.</span></span>|
|<span data-ttu-id="0886b-169">position</span><span class="sxs-lookup"><span data-stu-id="0886b-169">position</span></span>|<span data-ttu-id="0886b-170">int</span><span class="sxs-lookup"><span data-stu-id="0886b-170">int</span></span>|<span data-ttu-id="0886b-171">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0886b-171">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="0886b-172">visibilidade</span><span class="sxs-lookup"><span data-stu-id="0886b-172">visibility</span></span>|<span data-ttu-id="0886b-173">string</span><span class="sxs-lookup"><span data-stu-id="0886b-173">string</span></span>|<span data-ttu-id="0886b-174">A visibilidade da planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-174">The Visibility of the worksheet.</span></span> <span data-ttu-id="0886b-175">Os valores possíveis são: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="0886b-175">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0886b-176">Relações</span><span class="sxs-lookup"><span data-stu-id="0886b-176">Relationships</span></span>
| <span data-ttu-id="0886b-177">Relação</span><span class="sxs-lookup"><span data-stu-id="0886b-177">Relationship</span></span> | <span data-ttu-id="0886b-178">Tipo</span><span class="sxs-lookup"><span data-stu-id="0886b-178">Type</span></span>   |<span data-ttu-id="0886b-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="0886b-179">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0886b-180">charts</span><span class="sxs-lookup"><span data-stu-id="0886b-180">charts</span></span>|<span data-ttu-id="0886b-181">coleção [workbookChart](workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="0886b-181">[workbookChart](workbookchart.md) collection</span></span>|<span data-ttu-id="0886b-182">Retorna uma coleção de gráficos que fazem parte da planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-182">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="0886b-183">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0886b-183">Read-only.</span></span>|
|<span data-ttu-id="0886b-184">names</span><span class="sxs-lookup"><span data-stu-id="0886b-184">names</span></span>|<span data-ttu-id="0886b-185">coleção [workbookNamedItem](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="0886b-185">[workbookNamedItem](workbooknameditem.md) collection</span></span>|<span data-ttu-id="0886b-186">Retorna a coleção de nomes associados à planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-186">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="0886b-187">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0886b-187">Read-only.</span></span>|
|<span data-ttu-id="0886b-188">pivotTables</span><span class="sxs-lookup"><span data-stu-id="0886b-188">pivotTables</span></span>|<span data-ttu-id="0886b-189">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="0886b-189">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="0886b-190">Coleção de Tabelas Dinâmicas que fazem parte da planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-190">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="0886b-191">proteção</span><span class="sxs-lookup"><span data-stu-id="0886b-191">protection</span></span>|[<span data-ttu-id="0886b-192">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="0886b-192">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md)|<span data-ttu-id="0886b-p110">Retorna o objeto de proteção da planilha para uma planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0886b-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="0886b-195">tables</span><span class="sxs-lookup"><span data-stu-id="0886b-195">tables</span></span>|<span data-ttu-id="0886b-196">coleção [workbooktable](workbooktable.md)</span><span class="sxs-lookup"><span data-stu-id="0886b-196">[workbookTable](workbooktable.md) collection</span></span>|<span data-ttu-id="0886b-197">Coleção de tabelas que fazem parte da planilha.</span><span class="sxs-lookup"><span data-stu-id="0886b-197">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="0886b-198">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0886b-198">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0886b-199">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0886b-199">JSON representation</span></span>

<span data-ttu-id="0886b-200">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0886b-200">Here is a JSON representation of the resource.</span></span>

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
