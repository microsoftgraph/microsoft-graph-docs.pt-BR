---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
localization_priority: Normal
ms.openlocfilehash: ad4341e13eadc911377ec7b9859d6a31305fadf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507548"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="1d170-103">Tipo de recurso FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="1d170-103">FilterDatetime resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d170-104">Indica como filtrar uma data ao filtrar valores.</span><span class="sxs-lookup"><span data-stu-id="1d170-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="1d170-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d170-105">Properties</span></span>
| <span data-ttu-id="1d170-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d170-106">Property</span></span>     | <span data-ttu-id="1d170-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d170-107">Type</span></span>   |<span data-ttu-id="1d170-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d170-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d170-109">data</span><span class="sxs-lookup"><span data-stu-id="1d170-109">date</span></span>|<span data-ttu-id="1d170-110">string</span><span class="sxs-lookup"><span data-stu-id="1d170-110">string</span></span>|<span data-ttu-id="1d170-111">A data no formato ISO8601 usada para filtrar os dados.</span><span class="sxs-lookup"><span data-stu-id="1d170-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="1d170-112">especificidade</span><span class="sxs-lookup"><span data-stu-id="1d170-112">specificity</span></span>|<span data-ttu-id="1d170-113">string</span><span class="sxs-lookup"><span data-stu-id="1d170-113">string</span></span>|<span data-ttu-id="1d170-p101">Como a data específica deve ser usada para manter os dados. Por exemplo, se a data for 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtragem manterá todas as linhas com uma data do mês de abril de 2009. Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute` e `Second`.</span><span class="sxs-lookup"><span data-stu-id="1d170-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d170-117">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="1d170-117">Relationships</span></span>
<span data-ttu-id="1d170-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d170-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1d170-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d170-119">JSON representation</span></span>

<span data-ttu-id="1d170-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d170-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filterdatetime.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
