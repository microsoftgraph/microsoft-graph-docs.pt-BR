---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: b3a0d76a236cc4bce53bf476a90e8f37757ae003
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512623"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="12b2f-102">Tipo de recurso CalculatedColumn</span><span class="sxs-lookup"><span data-stu-id="12b2f-102">CalculatedColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12b2f-103">**calculatedColumn** em um recurso [columnDefinition](columndefinition.md) indica que os dados da coluna são calculados com base em outras colunas do site.</span><span class="sxs-lookup"><span data-stu-id="12b2f-103">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12b2f-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12b2f-104">JSON representation</span></span>

<span data-ttu-id="12b2f-105">Aqui está uma representação JSON de um recurso **calculatedColumn**.</span><span class="sxs-lookup"><span data-stu-id="12b2f-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="12b2f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12b2f-106">Properties</span></span>

| <span data-ttu-id="12b2f-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="12b2f-107">Property name</span></span>  | <span data-ttu-id="12b2f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="12b2f-108">Type</span></span>    | <span data-ttu-id="12b2f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="12b2f-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="12b2f-110">**format**</span><span class="sxs-lookup"><span data-stu-id="12b2f-110">**format**</span></span>     | <span data-ttu-id="12b2f-111">string</span><span class="sxs-lookup"><span data-stu-id="12b2f-111">string</span></span>  | <span data-ttu-id="12b2f-112">Nos tipos de saída `dateTime`, o formato do valor.</span><span class="sxs-lookup"><span data-stu-id="12b2f-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="12b2f-113">Deve ser `dateOnly` ou `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="12b2f-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="12b2f-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="12b2f-114">**formula**</span></span>    | <span data-ttu-id="12b2f-115">string</span><span class="sxs-lookup"><span data-stu-id="12b2f-115">string</span></span>  | <span data-ttu-id="12b2f-116">A fórmula usada para calcular o valor dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="12b2f-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="12b2f-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="12b2f-117">**outputType**</span></span> | <span data-ttu-id="12b2f-118">string</span><span class="sxs-lookup"><span data-stu-id="12b2f-118">string</span></span>  | <span data-ttu-id="12b2f-119">O tipo de saída usado para formatar valores nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="12b2f-119">The output type used to format values in this column.</span></span> <span data-ttu-id="12b2f-120">Deve ser `boolean`, `currency`, `dateTime`, `number` ou `text`.</span><span class="sxs-lookup"><span data-stu-id="12b2f-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="12b2f-121">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="12b2f-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="12b2f-122">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="12b2f-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/calculatedColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
