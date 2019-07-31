---
author: JeremyKelley
description: calculatedColumn em um recurso columnDefinition indica que os dados da coluna são calculados com base em outras colunas do site.
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8492dcf39cbdee92a998a418599fc00b314078c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013056"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="eea3a-103">Tipo de recurso CalculatedColumn</span><span class="sxs-lookup"><span data-stu-id="eea3a-103">CalculatedColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eea3a-104">**calculatedColumn** em um recurso [columnDefinition](columndefinition.md) indica que os dados da coluna são calculados com base em outras colunas do site.</span><span class="sxs-lookup"><span data-stu-id="eea3a-104">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eea3a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eea3a-105">JSON representation</span></span>

<span data-ttu-id="eea3a-106">Aqui está uma representação JSON de um recurso **calculatedColumn**.</span><span class="sxs-lookup"><span data-stu-id="eea3a-106">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="eea3a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eea3a-107">Properties</span></span>

| <span data-ttu-id="eea3a-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="eea3a-108">Property name</span></span>  | <span data-ttu-id="eea3a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="eea3a-109">Type</span></span>    | <span data-ttu-id="eea3a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eea3a-110">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="eea3a-111">**format**</span><span class="sxs-lookup"><span data-stu-id="eea3a-111">**format**</span></span>     | <span data-ttu-id="eea3a-112">string</span><span class="sxs-lookup"><span data-stu-id="eea3a-112">string</span></span>  | <span data-ttu-id="eea3a-113">Nos tipos de saída `dateTime`, o formato do valor.</span><span class="sxs-lookup"><span data-stu-id="eea3a-113">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="eea3a-114">Deve ser `dateOnly` ou `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="eea3a-114">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="eea3a-115">**formula**</span><span class="sxs-lookup"><span data-stu-id="eea3a-115">**formula**</span></span>    | <span data-ttu-id="eea3a-116">string</span><span class="sxs-lookup"><span data-stu-id="eea3a-116">string</span></span>  | <span data-ttu-id="eea3a-117">A fórmula usada para calcular o valor dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="eea3a-117">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="eea3a-118">**outputType**</span><span class="sxs-lookup"><span data-stu-id="eea3a-118">**outputType**</span></span> | <span data-ttu-id="eea3a-119">string</span><span class="sxs-lookup"><span data-stu-id="eea3a-119">string</span></span>  | <span data-ttu-id="eea3a-120">O tipo de saída usado para formatar valores nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="eea3a-120">The output type used to format values in this column.</span></span> <span data-ttu-id="eea3a-121">Deve ser `boolean`, `currency`, `dateTime`, `number` ou `text`.</span><span class="sxs-lookup"><span data-stu-id="eea3a-121">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="eea3a-122">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="eea3a-122">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="eea3a-123">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="eea3a-123">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": []
}
-->
