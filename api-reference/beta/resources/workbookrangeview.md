---
title: tipo de recurso rangeView
description: RangeView representa um conjunto de células visíveis do intervalo pai.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c356c737946dc70c6718b71c1c9aa7081069fd96
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858999"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="d3b7c-103">tipo de recurso rangeView</span><span class="sxs-lookup"><span data-stu-id="d3b7c-103">rangeView resource type</span></span>

> <span data-ttu-id="d3b7c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3b7c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3b7c-106">RangeView representa um conjunto de células visíveis do intervalo pai.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-106">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="d3b7c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d3b7c-107">Methods</span></span>

| <span data-ttu-id="d3b7c-108">Método</span><span class="sxs-lookup"><span data-stu-id="d3b7c-108">Method</span></span>           | <span data-ttu-id="d3b7c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d3b7c-109">Return Type</span></span>    |<span data-ttu-id="d3b7c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3b7c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3b7c-111">List rows</span><span class="sxs-lookup"><span data-stu-id="d3b7c-111">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="d3b7c-112">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="d3b7c-112">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="d3b7c-113">Obtenha uma coleção de objetos workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-113">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="d3b7c-114">Itemat</span><span class="sxs-lookup"><span data-stu-id="d3b7c-114">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="d3b7c-115">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="d3b7c-115">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="d3b7c-116">Obtenha um item de modo de exibição de intervalo com base no índice.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-116">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="d3b7c-117">Range</span><span class="sxs-lookup"><span data-stu-id="d3b7c-117">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="d3b7c-118">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d3b7c-118">workbookRange</span></span>](range.md)|<span data-ttu-id="d3b7c-119">Retorna o objeto de intervalo associado à exibição do intervalo</span><span class="sxs-lookup"><span data-stu-id="d3b7c-119">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="d3b7c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3b7c-120">Properties</span></span>
| <span data-ttu-id="d3b7c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3b7c-121">Property</span></span>     | <span data-ttu-id="d3b7c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3b7c-122">Type</span></span>   |<span data-ttu-id="d3b7c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3b7c-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3b7c-124">columnCount</span><span class="sxs-lookup"><span data-stu-id="d3b7c-124">columnCount</span></span>|<span data-ttu-id="d3b7c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d3b7c-125">Int32</span></span>|<span data-ttu-id="d3b7c-p102">Retorna o número de colunas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-p102">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="d3b7c-128">formulas</span><span class="sxs-lookup"><span data-stu-id="d3b7c-128">formulas</span></span>|<span data-ttu-id="d3b7c-129">Json</span><span class="sxs-lookup"><span data-stu-id="d3b7c-129">Json</span></span>|<span data-ttu-id="d3b7c-130">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-130">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="d3b7c-131">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="d3b7c-131">formulasLocal</span></span>|<span data-ttu-id="d3b7c-132">Json</span><span class="sxs-lookup"><span data-stu-id="d3b7c-132">Json</span></span>|<span data-ttu-id="d3b7c-p103">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário. Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="d3b7c-135">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="d3b7c-135">formulasR1C1</span></span>|<span data-ttu-id="d3b7c-136">Json</span><span class="sxs-lookup"><span data-stu-id="d3b7c-136">Json</span></span>|<span data-ttu-id="d3b7c-137">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-137">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="d3b7c-138">índice</span><span class="sxs-lookup"><span data-stu-id="d3b7c-138">index</span></span>|<span data-ttu-id="d3b7c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d3b7c-139">Int32</span></span>|<span data-ttu-id="d3b7c-140">O índice do intervalo.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-140">Index of the range.</span></span>|
|<span data-ttu-id="d3b7c-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="d3b7c-141">numberFormat</span></span>|<span data-ttu-id="d3b7c-142">Json</span><span class="sxs-lookup"><span data-stu-id="d3b7c-142">Json</span></span>|<span data-ttu-id="d3b7c-p104">Representa o código de formato de número do Excel para determinada célula. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-p104">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="d3b7c-145">rowCount</span><span class="sxs-lookup"><span data-stu-id="d3b7c-145">rowCount</span></span>|<span data-ttu-id="d3b7c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d3b7c-146">Int32</span></span>|<span data-ttu-id="d3b7c-p105">Retorna o número de linhas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-p105">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="d3b7c-149">text</span><span class="sxs-lookup"><span data-stu-id="d3b7c-149">text</span></span>|<span data-ttu-id="d3b7c-150">Json</span><span class="sxs-lookup"><span data-stu-id="d3b7c-150">Json</span></span>|<span data-ttu-id="d3b7c-p106">Valores de texto do intervalo especificado. O valor de texto não depende da largura da célula. A substituição pelo sinal #, que ocorre na interface de usuário do Excel, não afeta o valor de texto retornado pela API. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-p106">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="d3b7c-155">valueTypes</span><span class="sxs-lookup"><span data-stu-id="d3b7c-155">valueTypes</span></span>|<span data-ttu-id="d3b7c-156">Json</span><span class="sxs-lookup"><span data-stu-id="d3b7c-156">Json</span></span>|<span data-ttu-id="d3b7c-p107">Representa o tipo de dados de cada célula. Somente leitura. Os valores possíveis são: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-p107">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="d3b7c-160">values</span><span class="sxs-lookup"><span data-stu-id="d3b7c-160">values</span></span>|<span data-ttu-id="d3b7c-161">Json</span><span class="sxs-lookup"><span data-stu-id="d3b7c-161">Json</span></span>|<span data-ttu-id="d3b7c-p108">Representa os valores brutos da exibição do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-p108">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="d3b7c-165">Relações</span><span class="sxs-lookup"><span data-stu-id="d3b7c-165">Relationships</span></span>
| <span data-ttu-id="d3b7c-166">Relação</span><span class="sxs-lookup"><span data-stu-id="d3b7c-166">Relationship</span></span> | <span data-ttu-id="d3b7c-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3b7c-167">Type</span></span>   |<span data-ttu-id="d3b7c-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3b7c-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3b7c-169">rows</span><span class="sxs-lookup"><span data-stu-id="d3b7c-169">rows</span></span>|<span data-ttu-id="d3b7c-170">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="d3b7c-170">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="d3b7c-p109">Representa uma coleção de exibições de tabelas associadas ao intervalo. Somente leitura.    Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-p109">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3b7c-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3b7c-174">JSON representation</span></span>
<span data-ttu-id="d3b7c-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3b7c-175">Here is a JSON representation of the resource.</span></span>
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
