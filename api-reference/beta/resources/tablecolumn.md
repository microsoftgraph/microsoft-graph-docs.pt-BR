---
title: Tipo de recurso TableColumn
description: Representa uma coluna em uma tabela.
author: lumine2008
ms.openlocfilehash: b68051403bf57d84b51850255c8f98c0b76ea9c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354646"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="c62a3-103">Tipo de recurso TableColumn</span><span class="sxs-lookup"><span data-stu-id="c62a3-103">TableColumn resource type</span></span>

> <span data-ttu-id="c62a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c62a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c62a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c62a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c62a3-106">Representa uma coluna em uma tabela.</span><span class="sxs-lookup"><span data-stu-id="c62a3-106">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="c62a3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c62a3-107">Methods</span></span>

| <span data-ttu-id="c62a3-108">Método</span><span class="sxs-lookup"><span data-stu-id="c62a3-108">Method</span></span>           | <span data-ttu-id="c62a3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c62a3-109">Return Type</span></span>    |<span data-ttu-id="c62a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c62a3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c62a3-111">Get TableColumn</span><span class="sxs-lookup"><span data-stu-id="c62a3-111">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="c62a3-112">TableColumn</span><span class="sxs-lookup"><span data-stu-id="c62a3-112">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="c62a3-113">Leia as propriedades e os relacionamentos do objeto tableColumn.</span><span class="sxs-lookup"><span data-stu-id="c62a3-113">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="c62a3-114">Update</span><span class="sxs-lookup"><span data-stu-id="c62a3-114">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="c62a3-115">TableColumn</span><span class="sxs-lookup"><span data-stu-id="c62a3-115">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="c62a3-116">Atualize o objeto TableColumn.</span><span class="sxs-lookup"><span data-stu-id="c62a3-116">Update TableColumn object.</span></span> |
|[<span data-ttu-id="c62a3-117">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="c62a3-117">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="c62a3-118">Range</span><span class="sxs-lookup"><span data-stu-id="c62a3-118">Range</span></span>](range.md)|<span data-ttu-id="c62a3-119">Obtém o objeto de intervalo associado ao corpo de dados da coluna.</span><span class="sxs-lookup"><span data-stu-id="c62a3-119">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="c62a3-120">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="c62a3-120">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="c62a3-121">Range</span><span class="sxs-lookup"><span data-stu-id="c62a3-121">Range</span></span>](range.md)|<span data-ttu-id="c62a3-122">Obtém o objeto de intervalo associado à linha de cabeçalho da coluna.</span><span class="sxs-lookup"><span data-stu-id="c62a3-122">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="c62a3-123">Range</span><span class="sxs-lookup"><span data-stu-id="c62a3-123">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="c62a3-124">Range</span><span class="sxs-lookup"><span data-stu-id="c62a3-124">Range</span></span>](range.md)|<span data-ttu-id="c62a3-125">Obtém o objeto de intervalo associado a toda a coluna.</span><span class="sxs-lookup"><span data-stu-id="c62a3-125">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="c62a3-126">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="c62a3-126">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="c62a3-127">Range</span><span class="sxs-lookup"><span data-stu-id="c62a3-127">Range</span></span>](range.md)|<span data-ttu-id="c62a3-128">Obtém o objeto de intervalo associado à linha de totais da coluna.</span><span class="sxs-lookup"><span data-stu-id="c62a3-128">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="c62a3-129">Delete</span><span class="sxs-lookup"><span data-stu-id="c62a3-129">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="c62a3-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c62a3-130">None</span></span>|<span data-ttu-id="c62a3-131">Exclui a coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="c62a3-131">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="c62a3-132">List</span><span class="sxs-lookup"><span data-stu-id="c62a3-132">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="c62a3-133">Coleção [TableColumn](tablecolumn.md)</span><span class="sxs-lookup"><span data-stu-id="c62a3-133">[TableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="c62a3-134">Obtenha uma coleção de objetos tableColumn.</span><span class="sxs-lookup"><span data-stu-id="c62a3-134">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="c62a3-135">Itemat</span><span class="sxs-lookup"><span data-stu-id="c62a3-135">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="c62a3-136">TableColumn</span><span class="sxs-lookup"><span data-stu-id="c62a3-136">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="c62a3-137">Obtém uma coluna com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="c62a3-137">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="c62a3-138">Add</span><span class="sxs-lookup"><span data-stu-id="c62a3-138">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="c62a3-139">TableColumn</span><span class="sxs-lookup"><span data-stu-id="c62a3-139">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="c62a3-140">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="c62a3-140">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="c62a3-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c62a3-141">Properties</span></span>
| <span data-ttu-id="c62a3-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c62a3-142">Property</span></span>     | <span data-ttu-id="c62a3-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="c62a3-143">Type</span></span>   |<span data-ttu-id="c62a3-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="c62a3-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c62a3-145">id</span><span class="sxs-lookup"><span data-stu-id="c62a3-145">id</span></span>|<span data-ttu-id="c62a3-146">inteiro</span><span class="sxs-lookup"><span data-stu-id="c62a3-146">int</span></span>|<span data-ttu-id="c62a3-p102">Retorna uma chave exclusiva que identifica a coluna na tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c62a3-p102">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="c62a3-149">índice</span><span class="sxs-lookup"><span data-stu-id="c62a3-149">index</span></span>|<span data-ttu-id="c62a3-150">inteiro</span><span class="sxs-lookup"><span data-stu-id="c62a3-150">int</span></span>|<span data-ttu-id="c62a3-p103">Retorna o número de índice da coluna na coleção de colunas da tabela. Indexado com zero. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c62a3-p103">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="c62a3-154">name</span><span class="sxs-lookup"><span data-stu-id="c62a3-154">name</span></span>|<span data-ttu-id="c62a3-155">string</span><span class="sxs-lookup"><span data-stu-id="c62a3-155">string</span></span>|<span data-ttu-id="c62a3-p104">Retorna o nome da coluna da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c62a3-p104">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="c62a3-158">values</span><span class="sxs-lookup"><span data-stu-id="c62a3-158">values</span></span>|<span data-ttu-id="c62a3-159">json</span><span class="sxs-lookup"><span data-stu-id="c62a3-159">json</span></span>|<span data-ttu-id="c62a3-p105">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="c62a3-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c62a3-163">Relações</span><span class="sxs-lookup"><span data-stu-id="c62a3-163">Relationships</span></span>
| <span data-ttu-id="c62a3-164">Relação</span><span class="sxs-lookup"><span data-stu-id="c62a3-164">Relationship</span></span> | <span data-ttu-id="c62a3-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="c62a3-165">Type</span></span>   |<span data-ttu-id="c62a3-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="c62a3-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c62a3-167">filtro</span><span class="sxs-lookup"><span data-stu-id="c62a3-167">filter</span></span>|[<span data-ttu-id="c62a3-168">Filter</span><span class="sxs-lookup"><span data-stu-id="c62a3-168">Filter</span></span>](filter.md)|<span data-ttu-id="c62a3-p106">Recupera o filtro aplicado à coluna. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c62a3-p106">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c62a3-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c62a3-171">JSON representation</span></span>

<span data-ttu-id="c62a3-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c62a3-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableColumn"
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