---
title: tipo de recurso rankedEmailAddress
description: Representa um endereço de email classificado.
localization_priority: Normal
ms.openlocfilehash: 0c92f46c587b4f615b640e47b8d82a33aefc5e50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344079"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="b733d-103">tipo de recurso rankedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b733d-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b733d-104">Representa um endereço de email classificado.</span><span class="sxs-lookup"><span data-stu-id="b733d-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="b733d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b733d-105">Properties</span></span>
| <span data-ttu-id="b733d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b733d-106">Property</span></span>     | <span data-ttu-id="b733d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b733d-107">Type</span></span>   |<span data-ttu-id="b733d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b733d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b733d-109">address</span><span class="sxs-lookup"><span data-stu-id="b733d-109">address</span></span>|<span data-ttu-id="b733d-110">string</span><span class="sxs-lookup"><span data-stu-id="b733d-110">string</span></span>|<span data-ttu-id="b733d-111">O endereço de email.</span><span class="sxs-lookup"><span data-stu-id="b733d-111">The email address.</span></span>|
|<span data-ttu-id="b733d-112">classificação</span><span class="sxs-lookup"><span data-stu-id="b733d-112">rank</span></span>|<span data-ttu-id="b733d-113">double</span><span class="sxs-lookup"><span data-stu-id="b733d-113">double</span></span>|<span data-ttu-id="b733d-114">A classificação do endereço de email.</span><span class="sxs-lookup"><span data-stu-id="b733d-114">The rank of the email address.</span></span> <span data-ttu-id="b733d-115">Uma classificação é usada como uma chave de classificação, em relação aos outros resultados retornados.</span><span class="sxs-lookup"><span data-stu-id="b733d-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="b733d-116">Um valor de classificação mais alto corresponde a um resultado mais relevante.</span><span class="sxs-lookup"><span data-stu-id="b733d-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="b733d-117">A relevância é determinada por sinais de comunicação, colaboração e relacionamento comercial.</span><span class="sxs-lookup"><span data-stu-id="b733d-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b733d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b733d-118">JSON representation</span></span>

<span data-ttu-id="b733d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b733d-119">Here is a JSON representation of the resource.</span></span>

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
