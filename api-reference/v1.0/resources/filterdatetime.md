---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd8d7c01b94306245708df8290a44ffb936ac4d6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018288"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="22a23-103">Tipo de recurso FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="22a23-103">FilterDatetime resource type</span></span>

<span data-ttu-id="22a23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22a23-105">Indica como filtrar uma data ao filtrar valores.</span><span class="sxs-lookup"><span data-stu-id="22a23-105">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="22a23-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22a23-106">Properties</span></span>
| <span data-ttu-id="22a23-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22a23-107">Property</span></span>     | <span data-ttu-id="22a23-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a23-108">Type</span></span>   |<span data-ttu-id="22a23-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a23-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22a23-110">data</span><span class="sxs-lookup"><span data-stu-id="22a23-110">date</span></span>|<span data-ttu-id="22a23-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22a23-111">string</span></span>|<span data-ttu-id="22a23-112">A data no formato ISO8601 usada para filtrar os dados.</span><span class="sxs-lookup"><span data-stu-id="22a23-112">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="22a23-113">especificidade</span><span class="sxs-lookup"><span data-stu-id="22a23-113">specificity</span></span>|<span data-ttu-id="22a23-114">string</span><span class="sxs-lookup"><span data-stu-id="22a23-114">string</span></span>|<span data-ttu-id="22a23-115">Como a data específica deve ser usada para manter os dados.</span><span class="sxs-lookup"><span data-stu-id="22a23-115">How specific the date should be used to keep data.</span></span> <span data-ttu-id="22a23-116">Por exemplo, se a data for 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtragem manterá todas as linhas com uma data do mês de abril de 2009.</span><span class="sxs-lookup"><span data-stu-id="22a23-116">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="22a23-117">Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="22a23-117">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22a23-118">Relações</span><span class="sxs-lookup"><span data-stu-id="22a23-118">Relationships</span></span>
<span data-ttu-id="22a23-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22a23-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="22a23-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22a23-120">JSON representation</span></span>

<span data-ttu-id="22a23-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22a23-121">Here is a JSON representation of the resource.</span></span>

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

