---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
ms.openlocfilehash: 8156b9f5779dd8d70ff3a839d8a6ef4f5753bacd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003573"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="4d380-103">Tipo de recurso FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="4d380-103">FilterDatetime resource type</span></span>

<span data-ttu-id="4d380-104">Indica como filtrar uma data ao filtrar valores.</span><span class="sxs-lookup"><span data-stu-id="4d380-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="4d380-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d380-105">Properties</span></span>
| <span data-ttu-id="4d380-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d380-106">Property</span></span>     | <span data-ttu-id="4d380-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d380-107">Type</span></span>   |<span data-ttu-id="4d380-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d380-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d380-109">data</span><span class="sxs-lookup"><span data-stu-id="4d380-109">date</span></span>|<span data-ttu-id="4d380-110">string</span><span class="sxs-lookup"><span data-stu-id="4d380-110">string</span></span>|<span data-ttu-id="4d380-111">A data no formato ISO8601 usada para filtrar os dados.</span><span class="sxs-lookup"><span data-stu-id="4d380-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="4d380-112">especificidade</span><span class="sxs-lookup"><span data-stu-id="4d380-112">specificity</span></span>|<span data-ttu-id="4d380-113">string</span><span class="sxs-lookup"><span data-stu-id="4d380-113">string</span></span>|<span data-ttu-id="4d380-114">Específico como a data deve ser usada para manter os dados.</span><span class="sxs-lookup"><span data-stu-id="4d380-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="4d380-115">Por exemplo, se a data é 2005-04-02 e o specifity estiver definido como "mês", a operação de filtro manterá todas as linhas com uma data no mês de abril de 2009.</span><span class="sxs-lookup"><span data-stu-id="4d380-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="4d380-116">Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="4d380-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d380-117">Relações</span><span class="sxs-lookup"><span data-stu-id="4d380-117">Relationships</span></span>
<span data-ttu-id="4d380-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4d380-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4d380-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d380-119">JSON representation</span></span>

<span data-ttu-id="4d380-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d380-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->