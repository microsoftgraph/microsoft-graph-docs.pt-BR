---
author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
description: calculatedColumn em um recurso columnDefinition indica que os dados da coluna são calculados com base em outras colunas do site.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a75db3ea7a3973d57a3d09aa6cba2cb85a66ce11
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239076"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="7a689-103">Tipo de recurso CalculatedColumn</span><span class="sxs-lookup"><span data-stu-id="7a689-103">CalculatedColumn resource type</span></span>

<span data-ttu-id="7a689-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a689-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a689-105">**calculatedColumn** em um recurso [columnDefinition](columndefinition.md) indica que os dados da coluna são calculados com base em outras colunas do site.</span><span class="sxs-lookup"><span data-stu-id="7a689-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a689-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a689-106">JSON representation</span></span>

<span data-ttu-id="7a689-107">Aqui está uma representação JSON de um recurso **calculatedColumn**.</span><span class="sxs-lookup"><span data-stu-id="7a689-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="7a689-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a689-108">Properties</span></span>

| <span data-ttu-id="7a689-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7a689-109">Property name</span></span>  | <span data-ttu-id="7a689-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a689-110">Type</span></span>    | <span data-ttu-id="7a689-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a689-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="7a689-112">**format**</span><span class="sxs-lookup"><span data-stu-id="7a689-112">**format**</span></span>     | <span data-ttu-id="7a689-113">string</span><span class="sxs-lookup"><span data-stu-id="7a689-113">string</span></span>  | <span data-ttu-id="7a689-114">Nos tipos de saída `dateTime`, o formato do valor.</span><span class="sxs-lookup"><span data-stu-id="7a689-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="7a689-115">Deve ser `dateOnly` ou `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="7a689-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="7a689-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="7a689-116">**formula**</span></span>    | <span data-ttu-id="7a689-117">string</span><span class="sxs-lookup"><span data-stu-id="7a689-117">string</span></span>  | <span data-ttu-id="7a689-118">A fórmula usada para calcular o valor dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="7a689-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="7a689-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="7a689-119">**outputType**</span></span> | <span data-ttu-id="7a689-120">string</span><span class="sxs-lookup"><span data-stu-id="7a689-120">string</span></span>  | <span data-ttu-id="7a689-121">O tipo de saída usado para formatar valores nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="7a689-121">The output type used to format values in this column.</span></span> <span data-ttu-id="7a689-122">Deve ser `boolean`, `currency`, `dateTime`, `number` ou `text`.</span><span class="sxs-lookup"><span data-stu-id="7a689-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="7a689-123">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="7a689-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="7a689-124">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="7a689-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(boolean,currency,dateTime,number,text) are in resource, but () are in table"
  ],
  "tocPath": "Resources/CalculatedColumn"
} -->

