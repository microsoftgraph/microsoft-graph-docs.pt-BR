---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
localization_priority: Normal
ms.openlocfilehash: 26d42b45a2e9b9cdd279f33330a877a64ea1c8d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564243"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="b4967-103">Tipo de recurso FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="b4967-103">FilterDatetime resource type</span></span>

<span data-ttu-id="b4967-104">Indica como filtrar uma data ao filtrar valores.</span><span class="sxs-lookup"><span data-stu-id="b4967-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="b4967-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4967-105">Properties</span></span>
| <span data-ttu-id="b4967-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4967-106">Property</span></span>     | <span data-ttu-id="b4967-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4967-107">Type</span></span>   |<span data-ttu-id="b4967-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4967-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4967-109">data</span><span class="sxs-lookup"><span data-stu-id="b4967-109">date</span></span>|<span data-ttu-id="b4967-110">string</span><span class="sxs-lookup"><span data-stu-id="b4967-110">string</span></span>|<span data-ttu-id="b4967-111">A data no formato ISO8601 usada para filtrar os dados.</span><span class="sxs-lookup"><span data-stu-id="b4967-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="b4967-112">especificidade</span><span class="sxs-lookup"><span data-stu-id="b4967-112">specificity</span></span>|<span data-ttu-id="b4967-113">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4967-113">string</span></span>|<span data-ttu-id="b4967-114">Como a data específica deve ser usada para manter os dados.</span><span class="sxs-lookup"><span data-stu-id="b4967-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="b4967-115">Por exemplo, se a data for 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtragem manterá todas as linhas com uma data do mês de abril de 2009.</span><span class="sxs-lookup"><span data-stu-id="b4967-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="b4967-116">Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="b4967-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4967-117">Relações</span><span class="sxs-lookup"><span data-stu-id="b4967-117">Relationships</span></span>
<span data-ttu-id="b4967-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4967-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b4967-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4967-119">JSON representation</span></span>

<span data-ttu-id="b4967-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4967-120">Here is a JSON representation of the resource.</span></span>

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
