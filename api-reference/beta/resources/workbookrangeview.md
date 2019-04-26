---
title: tipo de recurso workbookRangeView
description: RangeView representa um conjunto de células visíveis do intervalo pai.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fdc09b4c88e3105624f322697784cfa4e654ee96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345824"
---
# <a name="workbookrangeview-resource-type"></a><span data-ttu-id="fbf0e-103">tipo de recurso workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="fbf0e-103">workbookRangeView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbf0e-104">RangeView representa um conjunto de células visíveis do intervalo pai.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="fbf0e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fbf0e-105">Methods</span></span>

| <span data-ttu-id="fbf0e-106">Método</span><span class="sxs-lookup"><span data-stu-id="fbf0e-106">Method</span></span>           | <span data-ttu-id="fbf0e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fbf0e-107">Return Type</span></span>    |<span data-ttu-id="fbf0e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbf0e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbf0e-109">List rows</span><span class="sxs-lookup"><span data-stu-id="fbf0e-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="fbf0e-110">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="fbf0e-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="fbf0e-111">Obtenha uma coleção de objetos workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="fbf0e-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="fbf0e-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="fbf0e-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="fbf0e-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="fbf0e-114">Obtenha um item de modo de exibição de intervalo com base no índice.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="fbf0e-115">Range</span><span class="sxs-lookup"><span data-stu-id="fbf0e-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="fbf0e-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="fbf0e-116">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="fbf0e-117">Retorna o objeto de intervalo associado à exibição do intervalo</span><span class="sxs-lookup"><span data-stu-id="fbf0e-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="fbf0e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbf0e-118">Properties</span></span>
| <span data-ttu-id="fbf0e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbf0e-119">Property</span></span>     | <span data-ttu-id="fbf0e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbf0e-120">Type</span></span>   |<span data-ttu-id="fbf0e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbf0e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbf0e-122">columnCount</span><span class="sxs-lookup"><span data-stu-id="fbf0e-122">columnCount</span></span>|<span data-ttu-id="fbf0e-123">Int32</span><span class="sxs-lookup"><span data-stu-id="fbf0e-123">Int32</span></span>|<span data-ttu-id="fbf0e-p101">Retorna o número de colunas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="fbf0e-126">formulas</span><span class="sxs-lookup"><span data-stu-id="fbf0e-126">formulas</span></span>|<span data-ttu-id="fbf0e-127">Json</span><span class="sxs-lookup"><span data-stu-id="fbf0e-127">Json</span></span>|<span data-ttu-id="fbf0e-128">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-128">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="fbf0e-129">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="fbf0e-129">formulasLocal</span></span>|<span data-ttu-id="fbf0e-130">Json</span><span class="sxs-lookup"><span data-stu-id="fbf0e-130">Json</span></span>|<span data-ttu-id="fbf0e-p102">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário. Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="fbf0e-133">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="fbf0e-133">formulasR1C1</span></span>|<span data-ttu-id="fbf0e-134">Json</span><span class="sxs-lookup"><span data-stu-id="fbf0e-134">Json</span></span>|<span data-ttu-id="fbf0e-135">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-135">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="fbf0e-136">índice</span><span class="sxs-lookup"><span data-stu-id="fbf0e-136">index</span></span>|<span data-ttu-id="fbf0e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="fbf0e-137">Int32</span></span>|<span data-ttu-id="fbf0e-138">O índice do intervalo.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-138">Index of the range.</span></span>|
|<span data-ttu-id="fbf0e-139">numberFormat</span><span class="sxs-lookup"><span data-stu-id="fbf0e-139">numberFormat</span></span>|<span data-ttu-id="fbf0e-140">Json</span><span class="sxs-lookup"><span data-stu-id="fbf0e-140">Json</span></span>|<span data-ttu-id="fbf0e-p103">Representa o código de formato de número do Excel para determinada célula. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="fbf0e-143">rowCount</span><span class="sxs-lookup"><span data-stu-id="fbf0e-143">rowCount</span></span>|<span data-ttu-id="fbf0e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fbf0e-144">Int32</span></span>|<span data-ttu-id="fbf0e-p104">Retorna o número de linhas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="fbf0e-147">text</span><span class="sxs-lookup"><span data-stu-id="fbf0e-147">text</span></span>|<span data-ttu-id="fbf0e-148">Json</span><span class="sxs-lookup"><span data-stu-id="fbf0e-148">Json</span></span>|<span data-ttu-id="fbf0e-p105">Valores de texto do intervalo especificado. O valor de texto não depende da largura da célula. A substituição pelo sinal #, que ocorre na interface de usuário do Excel, não afeta o valor de texto retornado pela API. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="fbf0e-153">valueTypes</span><span class="sxs-lookup"><span data-stu-id="fbf0e-153">valueTypes</span></span>|<span data-ttu-id="fbf0e-154">Json</span><span class="sxs-lookup"><span data-stu-id="fbf0e-154">Json</span></span>|<span data-ttu-id="fbf0e-p106">Representa o tipo de dados de cada célula. Somente leitura. Os valores possíveis são: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="fbf0e-158">values</span><span class="sxs-lookup"><span data-stu-id="fbf0e-158">values</span></span>|<span data-ttu-id="fbf0e-159">Json</span><span class="sxs-lookup"><span data-stu-id="fbf0e-159">Json</span></span>|<span data-ttu-id="fbf0e-p107">Representa os valores brutos da exibição do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="fbf0e-163">Relações</span><span class="sxs-lookup"><span data-stu-id="fbf0e-163">Relationships</span></span>
| <span data-ttu-id="fbf0e-164">Relação</span><span class="sxs-lookup"><span data-stu-id="fbf0e-164">Relationship</span></span> | <span data-ttu-id="fbf0e-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbf0e-165">Type</span></span>   |<span data-ttu-id="fbf0e-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbf0e-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbf0e-167">rows</span><span class="sxs-lookup"><span data-stu-id="fbf0e-167">rows</span></span>|<span data-ttu-id="fbf0e-168">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="fbf0e-168">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="fbf0e-p108">Representa uma coleção de exibições de tabelas associadas ao intervalo. Somente leitura.    Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbf0e-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbf0e-172">JSON representation</span></span>
<span data-ttu-id="fbf0e-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbf0e-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
