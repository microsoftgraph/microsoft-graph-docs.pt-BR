---
title: tipo de recurso workbookRangeView
description: RangeView representa um conjunto de células visíveis do intervalo pai.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: da469982ba0f5adf8c6387057d21f31b6d977baa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046171"
---
# <a name="workbookrangeview-resource-type"></a><span data-ttu-id="a2451-103">tipo de recurso workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="a2451-103">workbookRangeView resource type</span></span>

<span data-ttu-id="a2451-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2451-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2451-105">RangeView representa um conjunto de células visíveis do intervalo pai.</span><span class="sxs-lookup"><span data-stu-id="a2451-105">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="a2451-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a2451-106">Methods</span></span>

| <span data-ttu-id="a2451-107">Método</span><span class="sxs-lookup"><span data-stu-id="a2451-107">Method</span></span>           | <span data-ttu-id="a2451-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2451-108">Return Type</span></span>    |<span data-ttu-id="a2451-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2451-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2451-110">List rows</span><span class="sxs-lookup"><span data-stu-id="a2451-110">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="a2451-111">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="a2451-111">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="a2451-112">Obtenha uma coleção de objetos workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="a2451-112">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="a2451-113">Itemat</span><span class="sxs-lookup"><span data-stu-id="a2451-113">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="a2451-114">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="a2451-114">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="a2451-115">Obtenha um item de modo de exibição de intervalo com base no índice.</span><span class="sxs-lookup"><span data-stu-id="a2451-115">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="a2451-116">Range</span><span class="sxs-lookup"><span data-stu-id="a2451-116">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="a2451-117">workbookRange</span><span class="sxs-lookup"><span data-stu-id="a2451-117">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="a2451-118">Retorna o objeto de intervalo associado à exibição do intervalo</span><span class="sxs-lookup"><span data-stu-id="a2451-118">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="a2451-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2451-119">Properties</span></span>
| <span data-ttu-id="a2451-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2451-120">Property</span></span>     | <span data-ttu-id="a2451-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2451-121">Type</span></span>   |<span data-ttu-id="a2451-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2451-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2451-123">columnCount</span><span class="sxs-lookup"><span data-stu-id="a2451-123">columnCount</span></span>|<span data-ttu-id="a2451-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a2451-124">Int32</span></span>|<span data-ttu-id="a2451-p101">Retorna o número de colunas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2451-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="a2451-127">fórmulas</span><span class="sxs-lookup"><span data-stu-id="a2451-127">formulas</span></span>|<span data-ttu-id="a2451-128">Json</span><span class="sxs-lookup"><span data-stu-id="a2451-128">Json</span></span>|<span data-ttu-id="a2451-129">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="a2451-129">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="a2451-130">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="a2451-130">formulasLocal</span></span>|<span data-ttu-id="a2451-131">Json</span><span class="sxs-lookup"><span data-stu-id="a2451-131">Json</span></span>|<span data-ttu-id="a2451-p102">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário. Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="a2451-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="a2451-134">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="a2451-134">formulasR1C1</span></span>|<span data-ttu-id="a2451-135">Json</span><span class="sxs-lookup"><span data-stu-id="a2451-135">Json</span></span>|<span data-ttu-id="a2451-136">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="a2451-136">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="a2451-137">índice</span><span class="sxs-lookup"><span data-stu-id="a2451-137">index</span></span>|<span data-ttu-id="a2451-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a2451-138">Int32</span></span>|<span data-ttu-id="a2451-139">O índice do intervalo.</span><span class="sxs-lookup"><span data-stu-id="a2451-139">Index of the range.</span></span>|
|<span data-ttu-id="a2451-140">numberFormat</span><span class="sxs-lookup"><span data-stu-id="a2451-140">numberFormat</span></span>|<span data-ttu-id="a2451-141">Json</span><span class="sxs-lookup"><span data-stu-id="a2451-141">Json</span></span>|<span data-ttu-id="a2451-p103">Representa o código de formato de número do Excel para determinada célula. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2451-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="a2451-144">rowCount</span><span class="sxs-lookup"><span data-stu-id="a2451-144">rowCount</span></span>|<span data-ttu-id="a2451-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a2451-145">Int32</span></span>|<span data-ttu-id="a2451-p104">Retorna o número de linhas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2451-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="a2451-148">texto</span><span class="sxs-lookup"><span data-stu-id="a2451-148">text</span></span>|<span data-ttu-id="a2451-149">Json</span><span class="sxs-lookup"><span data-stu-id="a2451-149">Json</span></span>|<span data-ttu-id="a2451-p105">Valores de texto do intervalo especificado. O valor de texto não depende da largura da célula. A substituição pelo sinal #, que ocorre na interface de usuário do Excel, não afeta o valor de texto retornado pela API. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2451-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="a2451-154">valueTypes</span><span class="sxs-lookup"><span data-stu-id="a2451-154">valueTypes</span></span>|<span data-ttu-id="a2451-155">Json</span><span class="sxs-lookup"><span data-stu-id="a2451-155">Json</span></span>|<span data-ttu-id="a2451-p106">Representa o tipo de dados de cada célula. Somente leitura. Os valores possíveis são: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="a2451-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="a2451-159">values</span><span class="sxs-lookup"><span data-stu-id="a2451-159">values</span></span>|<span data-ttu-id="a2451-160">Json</span><span class="sxs-lookup"><span data-stu-id="a2451-160">Json</span></span>|<span data-ttu-id="a2451-p107">Representa os valores brutos da exibição do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="a2451-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="a2451-164">Relações</span><span class="sxs-lookup"><span data-stu-id="a2451-164">Relationships</span></span>
| <span data-ttu-id="a2451-165">Relação</span><span class="sxs-lookup"><span data-stu-id="a2451-165">Relationship</span></span> | <span data-ttu-id="a2451-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2451-166">Type</span></span>   |<span data-ttu-id="a2451-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2451-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2451-168">rows</span><span class="sxs-lookup"><span data-stu-id="a2451-168">rows</span></span>|<span data-ttu-id="a2451-169">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="a2451-169">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="a2451-p108">Representa uma coleção de exibições de tabelas associadas ao intervalo. Somente leitura.    Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2451-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2451-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2451-173">JSON representation</span></span>
<span data-ttu-id="a2451-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2451-174">Here is a JSON representation of the resource.</span></span>
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


