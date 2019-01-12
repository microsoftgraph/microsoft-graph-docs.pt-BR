---
title: Tipo de recurso Worksheet
description: Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: d04ebafda64f9a081096fbf0fd94461b9765a6db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926523"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="69000-104">Tipo de recurso Worksheet</span><span class="sxs-lookup"><span data-stu-id="69000-104">Worksheet resource type</span></span>

> <span data-ttu-id="69000-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="69000-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69000-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="69000-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69000-p103">Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.</span><span class="sxs-lookup"><span data-stu-id="69000-p103">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="69000-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="69000-109">Methods</span></span>

| <span data-ttu-id="69000-110">Método</span><span class="sxs-lookup"><span data-stu-id="69000-110">Method</span></span>           | <span data-ttu-id="69000-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="69000-111">Return Type</span></span>    |<span data-ttu-id="69000-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="69000-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69000-113">Get Worksheet</span><span class="sxs-lookup"><span data-stu-id="69000-113">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="69000-114">Worksheet</span><span class="sxs-lookup"><span data-stu-id="69000-114">Worksheet</span></span>](worksheet.md) |<span data-ttu-id="69000-115">Leia as propriedades e os relacionamentos do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="69000-115">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="69000-116">Create Chart</span><span class="sxs-lookup"><span data-stu-id="69000-116">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="69000-117">Chart</span><span class="sxs-lookup"><span data-stu-id="69000-117">Chart</span></span>](chart.md)| <span data-ttu-id="69000-118">Crie um novo Gráfico ao postar na coleção de gráficos.</span><span class="sxs-lookup"><span data-stu-id="69000-118">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="69000-119">Nomes da lista</span><span class="sxs-lookup"><span data-stu-id="69000-119">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="69000-120">Coleção [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="69000-120">[NamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="69000-121">Faça com que a coleção de itens nomeados seja associada à planilha.</span><span class="sxs-lookup"><span data-stu-id="69000-121">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="69000-122">Listar gráficos</span><span class="sxs-lookup"><span data-stu-id="69000-122">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="69000-123">Coleção [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="69000-123">[Chart](chart.md) collection</span></span>| <span data-ttu-id="69000-124">Obtenha a coleção de objetos Chart.</span><span class="sxs-lookup"><span data-stu-id="69000-124">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="69000-125">Create Table</span><span class="sxs-lookup"><span data-stu-id="69000-125">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="69000-126">Table</span><span class="sxs-lookup"><span data-stu-id="69000-126">Table</span></span>](table.md)| <span data-ttu-id="69000-127">Crie uma nova Table postando na coleção de tabelas.</span><span class="sxs-lookup"><span data-stu-id="69000-127">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="69000-128">List tables</span><span class="sxs-lookup"><span data-stu-id="69000-128">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="69000-129">Coleção [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="69000-129">[Table](table.md) collection</span></span>| <span data-ttu-id="69000-130">Obtenha uma coleção de objetos Table.</span><span class="sxs-lookup"><span data-stu-id="69000-130">Get a Table object collection.</span></span>|
|[<span data-ttu-id="69000-131">Update</span><span class="sxs-lookup"><span data-stu-id="69000-131">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="69000-132">Worksheet</span><span class="sxs-lookup"><span data-stu-id="69000-132">Worksheet</span></span>](worksheet.md)   |<span data-ttu-id="69000-133">Atualize o objeto Worksheet.</span><span class="sxs-lookup"><span data-stu-id="69000-133">Update Worksheet object.</span></span> |
|[<span data-ttu-id="69000-134">Cell</span><span class="sxs-lookup"><span data-stu-id="69000-134">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="69000-135">Range</span><span class="sxs-lookup"><span data-stu-id="69000-135">Range</span></span>](range.md)|<span data-ttu-id="69000-p104">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="69000-p104">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="69000-138">Range</span><span class="sxs-lookup"><span data-stu-id="69000-138">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="69000-139">Range</span><span class="sxs-lookup"><span data-stu-id="69000-139">Range</span></span>](range.md)|<span data-ttu-id="69000-140">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="69000-140">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="69000-141">Usedrange</span><span class="sxs-lookup"><span data-stu-id="69000-141">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="69000-142">Range</span><span class="sxs-lookup"><span data-stu-id="69000-142">Range</span></span>](range.md)|<span data-ttu-id="69000-p105">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="69000-p105">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="69000-145">Delete</span><span class="sxs-lookup"><span data-stu-id="69000-145">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="69000-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69000-146">None</span></span>|<span data-ttu-id="69000-147">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="69000-147">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="69000-148">List</span><span class="sxs-lookup"><span data-stu-id="69000-148">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="69000-149">Coleção [Worksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="69000-149">[Worksheet](worksheet.md) collection</span></span> |<span data-ttu-id="69000-150">Obtenha a coleção de objetos da planilha.</span><span class="sxs-lookup"><span data-stu-id="69000-150">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="69000-151">Add</span><span class="sxs-lookup"><span data-stu-id="69000-151">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="69000-152">Worksheet</span><span class="sxs-lookup"><span data-stu-id="69000-152">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="69000-p106">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes.</span><span class="sxs-lookup"><span data-stu-id="69000-p106">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="69000-155">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="69000-155">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="69000-156">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="69000-156">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="69000-157">Obtenha uma coleção de objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="69000-157">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="69000-158">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69000-158">Properties</span></span>
| <span data-ttu-id="69000-159">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69000-159">Property</span></span>     | <span data-ttu-id="69000-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="69000-160">Type</span></span>   |<span data-ttu-id="69000-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="69000-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69000-162">id</span><span class="sxs-lookup"><span data-stu-id="69000-162">id</span></span>|<span data-ttu-id="69000-163">string</span><span class="sxs-lookup"><span data-stu-id="69000-163">string</span></span>|<span data-ttu-id="69000-p107">Retorna um valor que identifica de forma exclusiva a planilha em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a planilha seja renomeada ou movida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69000-p107">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="69000-167">name</span><span class="sxs-lookup"><span data-stu-id="69000-167">name</span></span>|<span data-ttu-id="69000-168">string</span><span class="sxs-lookup"><span data-stu-id="69000-168">string</span></span>|<span data-ttu-id="69000-169">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="69000-169">The display name of the worksheet.</span></span>|
|<span data-ttu-id="69000-170">position</span><span class="sxs-lookup"><span data-stu-id="69000-170">position</span></span>|<span data-ttu-id="69000-171">int</span><span class="sxs-lookup"><span data-stu-id="69000-171">int</span></span>|<span data-ttu-id="69000-172">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="69000-172">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="69000-173">visibilidade</span><span class="sxs-lookup"><span data-stu-id="69000-173">visibility</span></span>|<span data-ttu-id="69000-174">string</span><span class="sxs-lookup"><span data-stu-id="69000-174">string</span></span>|<span data-ttu-id="69000-p108">A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="69000-p108">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69000-177">Relações</span><span class="sxs-lookup"><span data-stu-id="69000-177">Relationships</span></span>
| <span data-ttu-id="69000-178">Relação</span><span class="sxs-lookup"><span data-stu-id="69000-178">Relationship</span></span> | <span data-ttu-id="69000-179">Tipo</span><span class="sxs-lookup"><span data-stu-id="69000-179">Type</span></span>   |<span data-ttu-id="69000-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="69000-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69000-181">charts</span><span class="sxs-lookup"><span data-stu-id="69000-181">charts</span></span>|<span data-ttu-id="69000-182">Coleção [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="69000-182">[Chart](chart.md) collection</span></span>|<span data-ttu-id="69000-p109">Retorna uma coleção de gráficos que fazem parte da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69000-p109">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="69000-185">names</span><span class="sxs-lookup"><span data-stu-id="69000-185">names</span></span>|<span data-ttu-id="69000-186">Coleção [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="69000-186">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="69000-p110">Retorna a coleção de nomes associados à planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69000-p110">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="69000-189">pivotTables</span><span class="sxs-lookup"><span data-stu-id="69000-189">pivotTables</span></span>|<span data-ttu-id="69000-190">Coleção [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="69000-190">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="69000-191">Coleção de Tabelas Dinâmicas que fazem parte da planilha.</span><span class="sxs-lookup"><span data-stu-id="69000-191">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="69000-192">protection</span><span class="sxs-lookup"><span data-stu-id="69000-192">protection</span></span>|[<span data-ttu-id="69000-193">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="69000-193">WorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="69000-p111">Retorna o objeto de proteção da planilha para uma planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69000-p111">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="69000-196">tables</span><span class="sxs-lookup"><span data-stu-id="69000-196">tables</span></span>|<span data-ttu-id="69000-197">Coleção [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="69000-197">[Table](table.md) collection</span></span>|<span data-ttu-id="69000-p112">Coleção de tabelas que fazem parte da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69000-p112">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69000-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69000-200">JSON representation</span></span>

<span data-ttu-id="69000-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69000-201">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
