---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9214e8ecde9b2c09e06cfcc6d6145ea5319eace9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531402"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="dd8eb-103">Tipo de recurso FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="dd8eb-103">FilterDatetime resource type</span></span>

<span data-ttu-id="dd8eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd8eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd8eb-105">Indica como filtrar uma data ao filtrar valores.</span><span class="sxs-lookup"><span data-stu-id="dd8eb-105">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="dd8eb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd8eb-106">Properties</span></span>
| <span data-ttu-id="dd8eb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd8eb-107">Property</span></span>     | <span data-ttu-id="dd8eb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd8eb-108">Type</span></span>   |<span data-ttu-id="dd8eb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd8eb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd8eb-110">data</span><span class="sxs-lookup"><span data-stu-id="dd8eb-110">date</span></span>|<span data-ttu-id="dd8eb-111">string</span><span class="sxs-lookup"><span data-stu-id="dd8eb-111">string</span></span>|<span data-ttu-id="dd8eb-112">A data no formato ISO8601 usada para filtrar os dados.</span><span class="sxs-lookup"><span data-stu-id="dd8eb-112">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="dd8eb-113">especificidade</span><span class="sxs-lookup"><span data-stu-id="dd8eb-113">specificity</span></span>|<span data-ttu-id="dd8eb-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd8eb-114">string</span></span>|<span data-ttu-id="dd8eb-115">Como a data específica deve ser usada para manter os dados.</span><span class="sxs-lookup"><span data-stu-id="dd8eb-115">How specific the date should be used to keep data.</span></span> <span data-ttu-id="dd8eb-116">Por exemplo, se a data for 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtragem manterá todas as linhas com uma data do mês de abril de 2009.</span><span class="sxs-lookup"><span data-stu-id="dd8eb-116">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="dd8eb-117">Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="dd8eb-117">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd8eb-118">Relações</span><span class="sxs-lookup"><span data-stu-id="dd8eb-118">Relationships</span></span>
<span data-ttu-id="dd8eb-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd8eb-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dd8eb-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd8eb-120">JSON representation</span></span>

<span data-ttu-id="dd8eb-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd8eb-121">Here is a JSON representation of the resource.</span></span>

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
