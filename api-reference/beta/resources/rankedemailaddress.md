---
title: tipo de recurso rankedEmailAddress
description: Representa um endereço de email classificado.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: 36215d545bb6d24fae4ef8cbca35a1c5210976bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026401"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="b7603-103">tipo de recurso rankedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b7603-103">rankedEmailAddress resource type</span></span>

<span data-ttu-id="b7603-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7603-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7603-105">Representa um endereço de email classificado.</span><span class="sxs-lookup"><span data-stu-id="b7603-105">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="b7603-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7603-106">Properties</span></span>
| <span data-ttu-id="b7603-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7603-107">Property</span></span>     | <span data-ttu-id="b7603-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7603-108">Type</span></span>   |<span data-ttu-id="b7603-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7603-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7603-110">address</span><span class="sxs-lookup"><span data-stu-id="b7603-110">address</span></span>|<span data-ttu-id="b7603-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7603-111">string</span></span>|<span data-ttu-id="b7603-112">O endereço de email.</span><span class="sxs-lookup"><span data-stu-id="b7603-112">The email address.</span></span>|
|<span data-ttu-id="b7603-113">classificação</span><span class="sxs-lookup"><span data-stu-id="b7603-113">rank</span></span>|<span data-ttu-id="b7603-114">double</span><span class="sxs-lookup"><span data-stu-id="b7603-114">double</span></span>|<span data-ttu-id="b7603-115">A classificação do endereço de email.</span><span class="sxs-lookup"><span data-stu-id="b7603-115">The rank of the email address.</span></span> <span data-ttu-id="b7603-116">Uma classificação é usada como uma chave de classificação, em relação aos outros resultados retornados.</span><span class="sxs-lookup"><span data-stu-id="b7603-116">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="b7603-117">Um valor de classificação mais alto corresponde a um resultado mais relevante.</span><span class="sxs-lookup"><span data-stu-id="b7603-117">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="b7603-118">A relevância é determinada por sinais de comunicação, colaboração e relacionamento comercial.</span><span class="sxs-lookup"><span data-stu-id="b7603-118">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7603-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7603-119">JSON representation</span></span>

<span data-ttu-id="b7603-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7603-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


