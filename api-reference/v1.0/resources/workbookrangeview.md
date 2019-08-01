---
title: tipo de recurso rangeView
description: RangeView representa um conjunto de células visíveis do intervalo pai.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d0e30db53ec6e798bf62d5a64aa7d856ddc8f5e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033345"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="1ebfa-103">tipo de recurso rangeView</span><span class="sxs-lookup"><span data-stu-id="1ebfa-103">rangeView resource type</span></span>
<span data-ttu-id="1ebfa-104">RangeView representa um conjunto de células visíveis do intervalo pai.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="1ebfa-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1ebfa-105">Methods</span></span>

| <span data-ttu-id="1ebfa-106">Método</span><span class="sxs-lookup"><span data-stu-id="1ebfa-106">Method</span></span>           | <span data-ttu-id="1ebfa-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1ebfa-107">Return Type</span></span>    |<span data-ttu-id="1ebfa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ebfa-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ebfa-109">List rows</span><span class="sxs-lookup"><span data-stu-id="1ebfa-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="1ebfa-110">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="1ebfa-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="1ebfa-111">Obtenha uma coleção de objetos workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="1ebfa-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="1ebfa-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="1ebfa-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="1ebfa-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="1ebfa-114">Obtenha um item de modo de exibição de intervalo com base no índice.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="1ebfa-115">Range</span><span class="sxs-lookup"><span data-stu-id="1ebfa-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="1ebfa-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="1ebfa-116">workbookRange</span></span>](range.md)|<span data-ttu-id="1ebfa-117">Retorna o objeto de intervalo associado à exibição do intervalo</span><span class="sxs-lookup"><span data-stu-id="1ebfa-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="1ebfa-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ebfa-118">Properties</span></span>
| <span data-ttu-id="1ebfa-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ebfa-119">Property</span></span>     | <span data-ttu-id="1ebfa-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ebfa-120">Type</span></span>   |<span data-ttu-id="1ebfa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ebfa-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ebfa-122">cellAddresses</span><span class="sxs-lookup"><span data-stu-id="1ebfa-122">cellAddresses</span></span>|<span data-ttu-id="1ebfa-123">Json</span><span class="sxs-lookup"><span data-stu-id="1ebfa-123">Json</span></span>|<span data-ttu-id="1ebfa-124">Representa os endereços de célula</span><span class="sxs-lookup"><span data-stu-id="1ebfa-124">Represents the cell addresses</span></span>
|<span data-ttu-id="1ebfa-125">columnCount</span><span class="sxs-lookup"><span data-stu-id="1ebfa-125">columnCount</span></span>|<span data-ttu-id="1ebfa-126">Int32</span><span class="sxs-lookup"><span data-stu-id="1ebfa-126">Int32</span></span>|<span data-ttu-id="1ebfa-p101">Retorna o número de colunas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="1ebfa-129">fórmulas</span><span class="sxs-lookup"><span data-stu-id="1ebfa-129">formulas</span></span>|<span data-ttu-id="1ebfa-130">Json</span><span class="sxs-lookup"><span data-stu-id="1ebfa-130">Json</span></span>|<span data-ttu-id="1ebfa-131">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-131">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="1ebfa-132">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="1ebfa-132">formulasLocal</span></span>|<span data-ttu-id="1ebfa-133">Json</span><span class="sxs-lookup"><span data-stu-id="1ebfa-133">Json</span></span>|<span data-ttu-id="1ebfa-p102">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário. Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="1ebfa-136">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="1ebfa-136">formulasR1C1</span></span>|<span data-ttu-id="1ebfa-137">Json</span><span class="sxs-lookup"><span data-stu-id="1ebfa-137">Json</span></span>|<span data-ttu-id="1ebfa-138">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-138">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="1ebfa-139">índice</span><span class="sxs-lookup"><span data-stu-id="1ebfa-139">index</span></span>|<span data-ttu-id="1ebfa-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1ebfa-140">Int32</span></span>|<span data-ttu-id="1ebfa-141">O índice do intervalo.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-141">Index of the range.</span></span>|
|<span data-ttu-id="1ebfa-142">numberFormat</span><span class="sxs-lookup"><span data-stu-id="1ebfa-142">numberFormat</span></span>|<span data-ttu-id="1ebfa-143">Json</span><span class="sxs-lookup"><span data-stu-id="1ebfa-143">Json</span></span>|<span data-ttu-id="1ebfa-p103">Representa o código de formato de número do Excel para determinada célula. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="1ebfa-146">rowCount</span><span class="sxs-lookup"><span data-stu-id="1ebfa-146">rowCount</span></span>|<span data-ttu-id="1ebfa-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1ebfa-147">Int32</span></span>|<span data-ttu-id="1ebfa-p104">Retorna o número de linhas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="1ebfa-150">texto</span><span class="sxs-lookup"><span data-stu-id="1ebfa-150">text</span></span>|<span data-ttu-id="1ebfa-151">Json</span><span class="sxs-lookup"><span data-stu-id="1ebfa-151">Json</span></span>|<span data-ttu-id="1ebfa-p105">Valores de texto do intervalo especificado. O valor de texto não depende da largura da célula. A substituição pelo sinal #, que ocorre na interface de usuário do Excel, não afeta o valor de texto retornado pela API. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="1ebfa-156">valueTypes</span><span class="sxs-lookup"><span data-stu-id="1ebfa-156">valueTypes</span></span>|<span data-ttu-id="1ebfa-157">Json</span><span class="sxs-lookup"><span data-stu-id="1ebfa-157">Json</span></span>|<span data-ttu-id="1ebfa-158">Representa o tipo de dados de cada célula.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-158">Represents the type of data of each cell.</span></span> <span data-ttu-id="1ebfa-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-159">Read-only.</span></span> <span data-ttu-id="1ebfa-160">Os valores possíveis são: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-160">The possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="1ebfa-161">values</span><span class="sxs-lookup"><span data-stu-id="1ebfa-161">values</span></span>|<span data-ttu-id="1ebfa-162">Json</span><span class="sxs-lookup"><span data-stu-id="1ebfa-162">Json</span></span>|<span data-ttu-id="1ebfa-p107">Representa os valores brutos da exibição do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="1ebfa-166">Relações</span><span class="sxs-lookup"><span data-stu-id="1ebfa-166">Relationships</span></span>
| <span data-ttu-id="1ebfa-167">Relação</span><span class="sxs-lookup"><span data-stu-id="1ebfa-167">Relationship</span></span> | <span data-ttu-id="1ebfa-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ebfa-168">Type</span></span>   |<span data-ttu-id="1ebfa-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ebfa-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ebfa-170">rows</span><span class="sxs-lookup"><span data-stu-id="1ebfa-170">rows</span></span>|<span data-ttu-id="1ebfa-171">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="1ebfa-171">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="1ebfa-p108">Representa uma coleção de exibições de tabelas associadas ao intervalo. Somente leitura.    Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ebfa-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ebfa-175">JSON representation</span></span>
<span data-ttu-id="1ebfa-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ebfa-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
