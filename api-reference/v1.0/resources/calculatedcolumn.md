---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 66fbc59fa9fe4880c023086c9bd334e04650bc73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569365"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="e41c5-102">Tipo de recurso CalculatedColumn</span><span class="sxs-lookup"><span data-stu-id="e41c5-102">CalculatedColumn resource type</span></span>

<span data-ttu-id="e41c5-103">**calculatedColumn** em um recurso [columnDefinition](columndefinition.md) indica que os dados da coluna são calculados com base em outras colunas do site.</span><span class="sxs-lookup"><span data-stu-id="e41c5-103">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e41c5-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e41c5-104">JSON representation</span></span>

<span data-ttu-id="e41c5-105">Aqui está uma representação JSON de um recurso **calculatedColumn**.</span><span class="sxs-lookup"><span data-stu-id="e41c5-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="e41c5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e41c5-106">Properties</span></span>

| <span data-ttu-id="e41c5-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e41c5-107">Property name</span></span>  | <span data-ttu-id="e41c5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e41c5-108">Type</span></span>    | <span data-ttu-id="e41c5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e41c5-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="e41c5-110">**format**</span><span class="sxs-lookup"><span data-stu-id="e41c5-110">**format**</span></span>     | <span data-ttu-id="e41c5-111">string</span><span class="sxs-lookup"><span data-stu-id="e41c5-111">string</span></span>  | <span data-ttu-id="e41c5-112">Nos tipos de saída `dateTime`, o formato do valor.</span><span class="sxs-lookup"><span data-stu-id="e41c5-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="e41c5-113">Deve ser `dateOnly` ou `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="e41c5-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="e41c5-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="e41c5-114">**formula**</span></span>    | <span data-ttu-id="e41c5-115">string</span><span class="sxs-lookup"><span data-stu-id="e41c5-115">string</span></span>  | <span data-ttu-id="e41c5-116">A fórmula usada para calcular o valor dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="e41c5-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="e41c5-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="e41c5-117">**outputType**</span></span> | <span data-ttu-id="e41c5-118">string</span><span class="sxs-lookup"><span data-stu-id="e41c5-118">string</span></span>  | <span data-ttu-id="e41c5-119">O tipo de saída usado para formatar valores nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="e41c5-119">The output type used to format values in this column.</span></span> <span data-ttu-id="e41c5-120">Deve ser `boolean`, `currency`, `dateTime`, `number` ou `text`.</span><span class="sxs-lookup"><span data-stu-id="e41c5-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="e41c5-121">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="e41c5-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="e41c5-122">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e41c5-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

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
