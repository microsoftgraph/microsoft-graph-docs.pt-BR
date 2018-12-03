---
title: tipo de recurso rangeView
description: RangeView representa um conjunto de células visíveis do intervalo pai.
ms.openlocfilehash: 84ff9d315a6bfa8c4b03fad1b8f05670cb2b155c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039945"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="b7a39-103">tipo de recurso rangeView</span><span class="sxs-lookup"><span data-stu-id="b7a39-103">rangeView resource type</span></span>

> <span data-ttu-id="b7a39-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b7a39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7a39-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b7a39-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7a39-106">RangeView representa um conjunto de células visíveis do intervalo pai.</span><span class="sxs-lookup"><span data-stu-id="b7a39-106">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="b7a39-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b7a39-107">Methods</span></span>

| <span data-ttu-id="b7a39-108">Método</span><span class="sxs-lookup"><span data-stu-id="b7a39-108">Method</span></span>           | <span data-ttu-id="b7a39-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b7a39-109">Return Type</span></span>    |<span data-ttu-id="b7a39-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7a39-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b7a39-111">List rows</span><span class="sxs-lookup"><span data-stu-id="b7a39-111">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="b7a39-112">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="b7a39-112">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="b7a39-113">Obtenha uma coleção de objetos workbookRangeView.</span><span class="sxs-lookup"><span data-stu-id="b7a39-113">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="b7a39-114">Itemat</span><span class="sxs-lookup"><span data-stu-id="b7a39-114">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="b7a39-115">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="b7a39-115">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="b7a39-116">Obtenha um item de modo de exibição de intervalo com base no índice.</span><span class="sxs-lookup"><span data-stu-id="b7a39-116">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="b7a39-117">Range</span><span class="sxs-lookup"><span data-stu-id="b7a39-117">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="b7a39-118">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b7a39-118">workbookRange</span></span>](range.md)|<span data-ttu-id="b7a39-119">Retorna o objeto de intervalo associado à exibição do intervalo</span><span class="sxs-lookup"><span data-stu-id="b7a39-119">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="b7a39-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7a39-120">Properties</span></span>
| <span data-ttu-id="b7a39-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7a39-121">Property</span></span>     | <span data-ttu-id="b7a39-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7a39-122">Type</span></span>   |<span data-ttu-id="b7a39-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7a39-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7a39-124">columnCount</span><span class="sxs-lookup"><span data-stu-id="b7a39-124">columnCount</span></span>|<span data-ttu-id="b7a39-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b7a39-125">Int32</span></span>|<span data-ttu-id="b7a39-p102">Retorna o número de colunas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b7a39-p102">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="b7a39-128">formulas</span><span class="sxs-lookup"><span data-stu-id="b7a39-128">formulas</span></span>|<span data-ttu-id="b7a39-129">Json</span><span class="sxs-lookup"><span data-stu-id="b7a39-129">Json</span></span>|<span data-ttu-id="b7a39-130">Representa a fórmula em notação A1.</span><span class="sxs-lookup"><span data-stu-id="b7a39-130">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="b7a39-131">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="b7a39-131">formulasLocal</span></span>|<span data-ttu-id="b7a39-132">Json</span><span class="sxs-lookup"><span data-stu-id="b7a39-132">Json</span></span>|<span data-ttu-id="b7a39-p103">Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário. Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.</span><span class="sxs-lookup"><span data-stu-id="b7a39-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="b7a39-135">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="b7a39-135">formulasR1C1</span></span>|<span data-ttu-id="b7a39-136">Json</span><span class="sxs-lookup"><span data-stu-id="b7a39-136">Json</span></span>|<span data-ttu-id="b7a39-137">Representa a fórmula em notação no estilo L1C1.</span><span class="sxs-lookup"><span data-stu-id="b7a39-137">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="b7a39-138">índice</span><span class="sxs-lookup"><span data-stu-id="b7a39-138">index</span></span>|<span data-ttu-id="b7a39-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b7a39-139">Int32</span></span>|<span data-ttu-id="b7a39-140">O índice do intervalo.</span><span class="sxs-lookup"><span data-stu-id="b7a39-140">Index of the range.</span></span>|
|<span data-ttu-id="b7a39-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="b7a39-141">numberFormat</span></span>|<span data-ttu-id="b7a39-142">Json</span><span class="sxs-lookup"><span data-stu-id="b7a39-142">Json</span></span>|<span data-ttu-id="b7a39-p104">Representa o código de formato de número do Excel para determinada célula. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b7a39-p104">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="b7a39-145">rowCount</span><span class="sxs-lookup"><span data-stu-id="b7a39-145">rowCount</span></span>|<span data-ttu-id="b7a39-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b7a39-146">Int32</span></span>|<span data-ttu-id="b7a39-p105">Retorna o número de linhas visíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b7a39-p105">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="b7a39-149">text</span><span class="sxs-lookup"><span data-stu-id="b7a39-149">text</span></span>|<span data-ttu-id="b7a39-150">Json</span><span class="sxs-lookup"><span data-stu-id="b7a39-150">Json</span></span>|<span data-ttu-id="b7a39-p106">Valores de texto do intervalo especificado. O valor de texto não depende da largura da célula. A substituição pelo sinal #, que ocorre na interface de usuário do Excel, não afeta o valor de texto retornado pela API. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b7a39-p106">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="b7a39-155">valueTypes</span><span class="sxs-lookup"><span data-stu-id="b7a39-155">valueTypes</span></span>|<span data-ttu-id="b7a39-156">Json</span><span class="sxs-lookup"><span data-stu-id="b7a39-156">Json</span></span>|<span data-ttu-id="b7a39-p107">Representa o tipo de dados de cada célula. Somente leitura. Os valores possíveis são: Unknown, Empty, String, Integer, Double, Boolean, Error.</span><span class="sxs-lookup"><span data-stu-id="b7a39-p107">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="b7a39-160">values</span><span class="sxs-lookup"><span data-stu-id="b7a39-160">values</span></span>|<span data-ttu-id="b7a39-161">Json</span><span class="sxs-lookup"><span data-stu-id="b7a39-161">Json</span></span>|<span data-ttu-id="b7a39-p108">Representa os valores brutos da exibição do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="b7a39-p108">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="b7a39-165">Relações</span><span class="sxs-lookup"><span data-stu-id="b7a39-165">Relationships</span></span>
| <span data-ttu-id="b7a39-166">Relação</span><span class="sxs-lookup"><span data-stu-id="b7a39-166">Relationship</span></span> | <span data-ttu-id="b7a39-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7a39-167">Type</span></span>   |<span data-ttu-id="b7a39-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7a39-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7a39-169">rows</span><span class="sxs-lookup"><span data-stu-id="b7a39-169">rows</span></span>|<span data-ttu-id="b7a39-170">Coleção [workbookRangeView](workbookrangeview.md)</span><span class="sxs-lookup"><span data-stu-id="b7a39-170">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="b7a39-p109">Representa uma coleção de exibições de tabelas associadas ao intervalo. Somente leitura.    Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b7a39-p109">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7a39-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7a39-174">JSON representation</span></span>
<span data-ttu-id="b7a39-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7a39-175">Here is a JSON representation of the resource.</span></span>
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