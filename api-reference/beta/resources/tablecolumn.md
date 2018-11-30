---
title: Tipo de recurso TableColumn
description: Representa uma coluna em uma tabela.
ms.openlocfilehash: 0195bde59ee2116b064b47b9659f682877efc16b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036683"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="876a0-103">Tipo de recurso TableColumn</span><span class="sxs-lookup"><span data-stu-id="876a0-103">TableColumn resource type</span></span>

> <span data-ttu-id="876a0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="876a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="876a0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="876a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="876a0-106">Representa uma coluna em uma tabela.</span><span class="sxs-lookup"><span data-stu-id="876a0-106">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="876a0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="876a0-107">Methods</span></span>

| <span data-ttu-id="876a0-108">Método</span><span class="sxs-lookup"><span data-stu-id="876a0-108">Method</span></span>           | <span data-ttu-id="876a0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="876a0-109">Return Type</span></span>    |<span data-ttu-id="876a0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="876a0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="876a0-111">Get TableColumn</span><span class="sxs-lookup"><span data-stu-id="876a0-111">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="876a0-112">TableColumn</span><span class="sxs-lookup"><span data-stu-id="876a0-112">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="876a0-113">Leia as propriedades e os relacionamentos do objeto tableColumn.</span><span class="sxs-lookup"><span data-stu-id="876a0-113">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="876a0-114">Update</span><span class="sxs-lookup"><span data-stu-id="876a0-114">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="876a0-115">TableColumn</span><span class="sxs-lookup"><span data-stu-id="876a0-115">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="876a0-116">Atualize o objeto TableColumn.</span><span class="sxs-lookup"><span data-stu-id="876a0-116">Update TableColumn object.</span></span> |
|[<span data-ttu-id="876a0-117">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="876a0-117">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="876a0-118">Range</span><span class="sxs-lookup"><span data-stu-id="876a0-118">Range</span></span>](range.md)|<span data-ttu-id="876a0-119">Obtém o objeto de intervalo associado ao corpo de dados da coluna.</span><span class="sxs-lookup"><span data-stu-id="876a0-119">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="876a0-120">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="876a0-120">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="876a0-121">Range</span><span class="sxs-lookup"><span data-stu-id="876a0-121">Range</span></span>](range.md)|<span data-ttu-id="876a0-122">Obtém o objeto de intervalo associado à linha de cabeçalho da coluna.</span><span class="sxs-lookup"><span data-stu-id="876a0-122">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="876a0-123">Range</span><span class="sxs-lookup"><span data-stu-id="876a0-123">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="876a0-124">Range</span><span class="sxs-lookup"><span data-stu-id="876a0-124">Range</span></span>](range.md)|<span data-ttu-id="876a0-125">Obtém o objeto de intervalo associado a toda a coluna.</span><span class="sxs-lookup"><span data-stu-id="876a0-125">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="876a0-126">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="876a0-126">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="876a0-127">Range</span><span class="sxs-lookup"><span data-stu-id="876a0-127">Range</span></span>](range.md)|<span data-ttu-id="876a0-128">Obtém o objeto de intervalo associado à linha de totais da coluna.</span><span class="sxs-lookup"><span data-stu-id="876a0-128">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="876a0-129">Delete</span><span class="sxs-lookup"><span data-stu-id="876a0-129">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="876a0-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="876a0-130">None</span></span>|<span data-ttu-id="876a0-131">Exclui a coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="876a0-131">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="876a0-132">List</span><span class="sxs-lookup"><span data-stu-id="876a0-132">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="876a0-133">Coleção [TableColumn](tablecolumn.md)</span><span class="sxs-lookup"><span data-stu-id="876a0-133">[TableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="876a0-134">Obtenha uma coleção de objetos tableColumn.</span><span class="sxs-lookup"><span data-stu-id="876a0-134">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="876a0-135">Itemat</span><span class="sxs-lookup"><span data-stu-id="876a0-135">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="876a0-136">TableColumn</span><span class="sxs-lookup"><span data-stu-id="876a0-136">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="876a0-137">Obtém uma coluna com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="876a0-137">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="876a0-138">Add</span><span class="sxs-lookup"><span data-stu-id="876a0-138">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="876a0-139">TableColumn</span><span class="sxs-lookup"><span data-stu-id="876a0-139">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="876a0-140">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="876a0-140">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="876a0-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="876a0-141">Properties</span></span>
| <span data-ttu-id="876a0-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="876a0-142">Property</span></span>     | <span data-ttu-id="876a0-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="876a0-143">Type</span></span>   |<span data-ttu-id="876a0-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="876a0-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="876a0-145">id</span><span class="sxs-lookup"><span data-stu-id="876a0-145">id</span></span>|<span data-ttu-id="876a0-146">inteiro</span><span class="sxs-lookup"><span data-stu-id="876a0-146">int</span></span>|<span data-ttu-id="876a0-p102">Retorna uma chave exclusiva que identifica a coluna na tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="876a0-p102">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="876a0-149">índice</span><span class="sxs-lookup"><span data-stu-id="876a0-149">index</span></span>|<span data-ttu-id="876a0-150">inteiro</span><span class="sxs-lookup"><span data-stu-id="876a0-150">int</span></span>|<span data-ttu-id="876a0-p103">Retorna o número de índice da coluna na coleção de colunas da tabela. Indexado com zero. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="876a0-p103">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="876a0-154">name</span><span class="sxs-lookup"><span data-stu-id="876a0-154">name</span></span>|<span data-ttu-id="876a0-155">string</span><span class="sxs-lookup"><span data-stu-id="876a0-155">string</span></span>|<span data-ttu-id="876a0-p104">Retorna o nome da coluna da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="876a0-p104">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="876a0-158">values</span><span class="sxs-lookup"><span data-stu-id="876a0-158">values</span></span>|<span data-ttu-id="876a0-159">json</span><span class="sxs-lookup"><span data-stu-id="876a0-159">json</span></span>|<span data-ttu-id="876a0-p105">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="876a0-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="876a0-163">Relações</span><span class="sxs-lookup"><span data-stu-id="876a0-163">Relationships</span></span>
| <span data-ttu-id="876a0-164">Relação</span><span class="sxs-lookup"><span data-stu-id="876a0-164">Relationship</span></span> | <span data-ttu-id="876a0-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="876a0-165">Type</span></span>   |<span data-ttu-id="876a0-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="876a0-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="876a0-167">filtro</span><span class="sxs-lookup"><span data-stu-id="876a0-167">filter</span></span>|[<span data-ttu-id="876a0-168">Filter</span><span class="sxs-lookup"><span data-stu-id="876a0-168">Filter</span></span>](filter.md)|<span data-ttu-id="876a0-p106">Recupera o filtro aplicado à coluna. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="876a0-p106">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="876a0-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="876a0-171">JSON representation</span></span>

<span data-ttu-id="876a0-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="876a0-172">Here is a JSON representation of the resource.</span></span>

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