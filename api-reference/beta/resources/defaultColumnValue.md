---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
ms.openlocfilehash: ad94cadaa26d0fab72236d4037ceffd09a52c561
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514275"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="261f4-102">Tipo de recurso DefaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="261f4-102">DefaultColumnValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="261f4-103">**defaultColumnValue** em um recurso [columnDefinition](columndefinition.md) especifica o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="261f4-103">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="261f4-104">O valor padrão pode ser especificado tanto diretamente ou como uma fórmula.</span><span class="sxs-lookup"><span data-stu-id="261f4-104">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="261f4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="261f4-105">JSON representation</span></span>

<span data-ttu-id="261f4-106">Aqui está uma representação JSON de um recurso **defaultColumnValue**.</span><span class="sxs-lookup"><span data-stu-id="261f4-106">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="261f4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="261f4-107">Properties</span></span>

| <span data-ttu-id="261f4-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="261f4-108">Property name</span></span> | <span data-ttu-id="261f4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="261f4-109">Type</span></span>   | <span data-ttu-id="261f4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="261f4-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="261f4-111">**formula**</span><span class="sxs-lookup"><span data-stu-id="261f4-111">**formula**</span></span>   | <span data-ttu-id="261f4-112">string</span><span class="sxs-lookup"><span data-stu-id="261f4-112">string</span></span> | <span data-ttu-id="261f4-113">A fórmula usada para calcular o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="261f4-113">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="261f4-114">**value**</span><span class="sxs-lookup"><span data-stu-id="261f4-114">**value**</span></span>     | <span data-ttu-id="261f4-115">string</span><span class="sxs-lookup"><span data-stu-id="261f4-115">string</span></span> | <span data-ttu-id="261f4-116">O valor direto para usar como o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="261f4-116">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="261f4-117">Somente uma **fórmula** ou um **valor** pode ser especificado por vez.</span><span class="sxs-lookup"><span data-stu-id="261f4-117">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="261f4-118">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="261f4-118">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="261f4-119">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="261f4-119">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue",
  "suppressions": [
    "Error: /api-reference/beta/resources/defaultColumnValue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
