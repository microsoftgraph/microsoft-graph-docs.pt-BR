---
title: Tipo de recurso TableColumn
description: Representa uma coluna em uma tabela.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7c2506c34e25ba4b3754e1fd7b13557b21176e09
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882114"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="d5713-103">Tipo de recurso TableColumn</span><span class="sxs-lookup"><span data-stu-id="d5713-103">TableColumn resource type</span></span>

<span data-ttu-id="d5713-104">Representa uma coluna em uma tabela.</span><span class="sxs-lookup"><span data-stu-id="d5713-104">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="d5713-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5713-105">Methods</span></span>

| <span data-ttu-id="d5713-106">Método</span><span class="sxs-lookup"><span data-stu-id="d5713-106">Method</span></span>           | <span data-ttu-id="d5713-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5713-107">Return Type</span></span>    |<span data-ttu-id="d5713-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5713-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d5713-109">Get TableColumn</span><span class="sxs-lookup"><span data-stu-id="d5713-109">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="d5713-110">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d5713-110">WorkbookTableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="d5713-111">Leia as propriedades e os relacionamentos do objeto tableColumn.</span><span class="sxs-lookup"><span data-stu-id="d5713-111">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="d5713-112">Update</span><span class="sxs-lookup"><span data-stu-id="d5713-112">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="d5713-113">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d5713-113">WorkbookTableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="d5713-114">Atualize o objeto TableColumn.</span><span class="sxs-lookup"><span data-stu-id="d5713-114">Update TableColumn object.</span></span> |
|[<span data-ttu-id="d5713-115">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="d5713-115">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="d5713-116">Range</span><span class="sxs-lookup"><span data-stu-id="d5713-116">Range</span></span>](range.md)|<span data-ttu-id="d5713-117">Obtém o objeto de intervalo associado ao corpo de dados da coluna.</span><span class="sxs-lookup"><span data-stu-id="d5713-117">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="d5713-118">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="d5713-118">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="d5713-119">Range</span><span class="sxs-lookup"><span data-stu-id="d5713-119">Range</span></span>](range.md)|<span data-ttu-id="d5713-120">Obtém o objeto de intervalo associado à linha de cabeçalho da coluna.</span><span class="sxs-lookup"><span data-stu-id="d5713-120">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="d5713-121">Range</span><span class="sxs-lookup"><span data-stu-id="d5713-121">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="d5713-122">Range</span><span class="sxs-lookup"><span data-stu-id="d5713-122">Range</span></span>](range.md)|<span data-ttu-id="d5713-123">Obtém o objeto de intervalo associado a toda a coluna.</span><span class="sxs-lookup"><span data-stu-id="d5713-123">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="d5713-124">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="d5713-124">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="d5713-125">Range</span><span class="sxs-lookup"><span data-stu-id="d5713-125">Range</span></span>](range.md)|<span data-ttu-id="d5713-126">Obtém o objeto de intervalo associado à linha de totais da coluna.</span><span class="sxs-lookup"><span data-stu-id="d5713-126">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="d5713-127">Delete</span><span class="sxs-lookup"><span data-stu-id="d5713-127">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="d5713-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5713-128">None</span></span>|<span data-ttu-id="d5713-129">Exclui a coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="d5713-129">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="d5713-130">List</span><span class="sxs-lookup"><span data-stu-id="d5713-130">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="d5713-131">Coleção [WorkbookTableColumn](tablecolumn.md)</span><span class="sxs-lookup"><span data-stu-id="d5713-131">[WorkbookTableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="d5713-132">Obtenha uma coleção de objetos tableColumn.</span><span class="sxs-lookup"><span data-stu-id="d5713-132">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="d5713-133">Itemat</span><span class="sxs-lookup"><span data-stu-id="d5713-133">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="d5713-134">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d5713-134">WorkbookTableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="d5713-135">Obtém uma coluna com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="d5713-135">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="d5713-136">Add</span><span class="sxs-lookup"><span data-stu-id="d5713-136">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="d5713-137">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d5713-137">WorkbookTableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="d5713-138">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="d5713-138">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5713-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5713-139">Properties</span></span>
| <span data-ttu-id="d5713-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5713-140">Property</span></span>     | <span data-ttu-id="d5713-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5713-141">Type</span></span>   |<span data-ttu-id="d5713-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5713-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5713-143">id</span><span class="sxs-lookup"><span data-stu-id="d5713-143">id</span></span>|<span data-ttu-id="d5713-144">string</span><span class="sxs-lookup"><span data-stu-id="d5713-144">string</span></span>|<span data-ttu-id="d5713-145">Retorna uma chave exclusiva que identifica a coluna na tabela.</span><span class="sxs-lookup"><span data-stu-id="d5713-145">Returns a unique key that identifies the column within the table.</span></span> <span data-ttu-id="d5713-146">Essa propriedade deve ser interpretada como um valor de cadeia de caracteres opacas e não deve ser analisada para qualquer outro tipo.</span><span class="sxs-lookup"><span data-stu-id="d5713-146">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="d5713-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5713-147">Read-only.</span></span>|
|<span data-ttu-id="d5713-148">índice</span><span class="sxs-lookup"><span data-stu-id="d5713-148">index</span></span>|<span data-ttu-id="d5713-149">int</span><span class="sxs-lookup"><span data-stu-id="d5713-149">int</span></span>|<span data-ttu-id="d5713-p102">Retorna o número de índice da coluna na coleção de colunas da tabela. Indexado com zero. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5713-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="d5713-153">name</span><span class="sxs-lookup"><span data-stu-id="d5713-153">name</span></span>|<span data-ttu-id="d5713-154">string</span><span class="sxs-lookup"><span data-stu-id="d5713-154">string</span></span>|<span data-ttu-id="d5713-p103">Retorna o nome da coluna da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5713-p103">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="d5713-157">values</span><span class="sxs-lookup"><span data-stu-id="d5713-157">values</span></span>|<span data-ttu-id="d5713-158">Json</span><span class="sxs-lookup"><span data-stu-id="d5713-158">Json</span></span>|<span data-ttu-id="d5713-p104">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="d5713-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5713-162">Relações</span><span class="sxs-lookup"><span data-stu-id="d5713-162">Relationships</span></span>
| <span data-ttu-id="d5713-163">Relação</span><span class="sxs-lookup"><span data-stu-id="d5713-163">Relationship</span></span> | <span data-ttu-id="d5713-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5713-164">Type</span></span>   |<span data-ttu-id="d5713-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5713-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5713-166">filter</span><span class="sxs-lookup"><span data-stu-id="d5713-166">filter</span></span>|[<span data-ttu-id="d5713-167">WorkbookFilter</span><span class="sxs-lookup"><span data-stu-id="d5713-167">WorkbookFilter</span></span>](filter.md)|<span data-ttu-id="d5713-p105">Recupera o filtro aplicado à coluna. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5713-p105">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5713-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5713-170">JSON representation</span></span>

<span data-ttu-id="d5713-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5713-171">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
