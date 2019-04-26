---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
localization_priority: Normal
ms.openlocfilehash: 49587bf34c90e9a42145fade30177f03c49ed0b6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333761"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="3f7ed-103">Tipo de recurso FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="3f7ed-103">FilterDatetime resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f7ed-104">Indica como filtrar uma data ao filtrar valores.</span><span class="sxs-lookup"><span data-stu-id="3f7ed-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="3f7ed-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f7ed-105">Properties</span></span>
| <span data-ttu-id="3f7ed-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f7ed-106">Property</span></span>     | <span data-ttu-id="3f7ed-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f7ed-107">Type</span></span>   |<span data-ttu-id="3f7ed-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f7ed-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f7ed-109">data</span><span class="sxs-lookup"><span data-stu-id="3f7ed-109">date</span></span>|<span data-ttu-id="3f7ed-110">string</span><span class="sxs-lookup"><span data-stu-id="3f7ed-110">string</span></span>|<span data-ttu-id="3f7ed-111">A data no formato ISO8601 usada para filtrar os dados.</span><span class="sxs-lookup"><span data-stu-id="3f7ed-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="3f7ed-112">especificidade</span><span class="sxs-lookup"><span data-stu-id="3f7ed-112">specificity</span></span>|<span data-ttu-id="3f7ed-113">string</span><span class="sxs-lookup"><span data-stu-id="3f7ed-113">string</span></span>|<span data-ttu-id="3f7ed-p101">Como a data específica deve ser usada para manter os dados. Por exemplo, se a data for 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtragem manterá todas as linhas com uma data do mês de abril de 2009. Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute` e `Second`.</span><span class="sxs-lookup"><span data-stu-id="3f7ed-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f7ed-117">Relações</span><span class="sxs-lookup"><span data-stu-id="3f7ed-117">Relationships</span></span>
<span data-ttu-id="3f7ed-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f7ed-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3f7ed-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f7ed-119">JSON representation</span></span>

<span data-ttu-id="3f7ed-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f7ed-120">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
