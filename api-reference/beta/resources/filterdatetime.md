---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 27dafb0583380af299a4f5d8632c60a7e8af1a54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973552"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="f3fa8-103">Tipo de recurso FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="f3fa8-103">FilterDatetime resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3fa8-104">Indica como filtrar uma data ao filtrar valores.</span><span class="sxs-lookup"><span data-stu-id="f3fa8-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="f3fa8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3fa8-105">Properties</span></span>
| <span data-ttu-id="f3fa8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3fa8-106">Property</span></span>     | <span data-ttu-id="f3fa8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3fa8-107">Type</span></span>   |<span data-ttu-id="f3fa8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3fa8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3fa8-109">data</span><span class="sxs-lookup"><span data-stu-id="f3fa8-109">date</span></span>|<span data-ttu-id="f3fa8-110">string</span><span class="sxs-lookup"><span data-stu-id="f3fa8-110">string</span></span>|<span data-ttu-id="f3fa8-111">A data no formato ISO8601 usada para filtrar os dados.</span><span class="sxs-lookup"><span data-stu-id="f3fa8-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="f3fa8-112">especificidade</span><span class="sxs-lookup"><span data-stu-id="f3fa8-112">specificity</span></span>|<span data-ttu-id="f3fa8-113">string</span><span class="sxs-lookup"><span data-stu-id="f3fa8-113">string</span></span>|<span data-ttu-id="f3fa8-p101">Como a data específica deve ser usada para manter os dados. Por exemplo, se a data for 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtragem manterá todas as linhas com uma data do mês de abril de 2009. Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute` e `Second`.</span><span class="sxs-lookup"><span data-stu-id="f3fa8-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3fa8-117">Relações</span><span class="sxs-lookup"><span data-stu-id="f3fa8-117">Relationships</span></span>
<span data-ttu-id="f3fa8-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3fa8-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f3fa8-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3fa8-119">JSON representation</span></span>

<span data-ttu-id="f3fa8-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3fa8-120">Here is a JSON representation of the resource.</span></span>

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
