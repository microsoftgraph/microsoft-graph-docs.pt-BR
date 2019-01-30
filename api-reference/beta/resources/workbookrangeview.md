---
title: tipo de recurso rangeView
description: RangeView representa um conjunto de células visíveis do intervalo pai.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ace424d12e38e4bb907923ea542ebd7330130d06
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643976"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="6fd5b-103">tipo de recurso rangeView</span><span class="sxs-lookup"><span data-stu-id="6fd5b-103">rangeView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fd5b-104">RangeView representa um conjunto de células visíveis do intervalo pai.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="6fd5b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="6fd5b-105">Methods</span></span>

| <span data-ttu-id="6fd5b-106">Método</span><span class="sxs-lookup"><span data-stu-id="6fd5b-106">Method</span></span>           | <span data-ttu-id="6fd5b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6fd5b-107">Return Type</span></span>    |<span data-ttu-id="6fd5b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fd5b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6fd5b-109">List rows</span><span class="sxs-lookup"><span data-stu-id="6fd5b-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="6fd5b-110">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="6fd5b-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="6fd5b-111">Obtenha uma coleção de objetos workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="6fd5b-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="6fd5b-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="6fd5b-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="6fd5b-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="6fd5b-114">Obtenha um item de modo de exibição de intervalo com base no índice.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="6fd5b-115">Range</span><span class="sxs-lookup"><span data-stu-id="6fd5b-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="6fd5b-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="6fd5b-116">workbookRange</span></span>](range.md)|<span data-ttu-id="6fd5b-117">Retorna o objeto de intervalo associado à exibição do intervalo</span><span class="sxs-lookup"><span data-stu-id="6fd5b-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="6fd5b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fd5b-118">Properties</span></span>
| <span data-ttu-id="6fd5b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fd5b-119">Property</span></span>     | <span data-ttu-id="6fd5b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fd5b-120">Type</span></span>   |<span data-ttu-id="6fd5b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fd5b-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fd5b-122">columnCount</span><span class="sxs-lookup"><span data-stu-id="6fd5b-122">columnCount</span></span>|<span data-ttu-id="6fd5b-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6fd5b-123">Int32</span></span>|<span data-ttu-id="6fd5b-p101">Retorna o número de colunas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="6fd5b-126">formulas</span><span class="sxs-lookup"><span data-stu-id="6fd5b-126">formulas</span></span>|<span data-ttu-id="6fd5b-127">Json</span><span class="sxs-lookup"><span data-stu-id="6fd5b-127">Json</span></span>|<span data-ttu-id="6fd5b-128">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-128">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="6fd5b-129">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="6fd5b-129">formulasLocal</span></span>|<span data-ttu-id="6fd5b-130">Json</span><span class="sxs-lookup"><span data-stu-id="6fd5b-130">Json</span></span>|<span data-ttu-id="6fd5b-p102">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário. Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="6fd5b-133">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="6fd5b-133">formulasR1C1</span></span>|<span data-ttu-id="6fd5b-134">Json</span><span class="sxs-lookup"><span data-stu-id="6fd5b-134">Json</span></span>|<span data-ttu-id="6fd5b-135">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-135">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="6fd5b-136">índice</span><span class="sxs-lookup"><span data-stu-id="6fd5b-136">index</span></span>|<span data-ttu-id="6fd5b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6fd5b-137">Int32</span></span>|<span data-ttu-id="6fd5b-138">O índice do intervalo.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-138">Index of the range.</span></span>|
|<span data-ttu-id="6fd5b-139">numberFormat</span><span class="sxs-lookup"><span data-stu-id="6fd5b-139">numberFormat</span></span>|<span data-ttu-id="6fd5b-140">Json</span><span class="sxs-lookup"><span data-stu-id="6fd5b-140">Json</span></span>|<span data-ttu-id="6fd5b-p103">Representa o código de formato de número do Excel para determinada célula. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="6fd5b-143">rowCount</span><span class="sxs-lookup"><span data-stu-id="6fd5b-143">rowCount</span></span>|<span data-ttu-id="6fd5b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="6fd5b-144">Int32</span></span>|<span data-ttu-id="6fd5b-p104">Retorna o número de linhas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="6fd5b-147">text</span><span class="sxs-lookup"><span data-stu-id="6fd5b-147">text</span></span>|<span data-ttu-id="6fd5b-148">Json</span><span class="sxs-lookup"><span data-stu-id="6fd5b-148">Json</span></span>|<span data-ttu-id="6fd5b-p105">Valores de texto do intervalo especificado. O valor de texto não depende da largura da célula. A substituição pelo sinal #, que ocorre na interface de usuário do Excel, não afeta o valor de texto retornado pela API. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="6fd5b-153">valueTypes</span><span class="sxs-lookup"><span data-stu-id="6fd5b-153">valueTypes</span></span>|<span data-ttu-id="6fd5b-154">Json</span><span class="sxs-lookup"><span data-stu-id="6fd5b-154">Json</span></span>|<span data-ttu-id="6fd5b-p106">Representa o tipo de dados de cada célula. Somente leitura. Os valores possíveis são: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="6fd5b-158">values</span><span class="sxs-lookup"><span data-stu-id="6fd5b-158">values</span></span>|<span data-ttu-id="6fd5b-159">Json</span><span class="sxs-lookup"><span data-stu-id="6fd5b-159">Json</span></span>|<span data-ttu-id="6fd5b-p107">Representa os valores brutos da exibição do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="6fd5b-163">Relações</span><span class="sxs-lookup"><span data-stu-id="6fd5b-163">Relationships</span></span>
| <span data-ttu-id="6fd5b-164">Relação</span><span class="sxs-lookup"><span data-stu-id="6fd5b-164">Relationship</span></span> | <span data-ttu-id="6fd5b-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fd5b-165">Type</span></span>   |<span data-ttu-id="6fd5b-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fd5b-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fd5b-167">rows</span><span class="sxs-lookup"><span data-stu-id="6fd5b-167">rows</span></span>|<span data-ttu-id="6fd5b-168">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="6fd5b-168">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="6fd5b-p108">Representa uma coleção de exibições de tabelas associadas ao intervalo. Somente leitura.    Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fd5b-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fd5b-172">JSON representation</span></span>
<span data-ttu-id="6fd5b-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fd5b-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookrangeview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
