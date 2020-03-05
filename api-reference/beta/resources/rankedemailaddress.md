---
title: tipo de recurso rankedEmailAddress
description: Representa um endereço de email classificado.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bdba5af83357737c77e3b5c441703e404f971587
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521275"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="2c0ca-103">tipo de recurso rankedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2c0ca-103">rankedEmailAddress resource type</span></span>

<span data-ttu-id="2c0ca-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2c0ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c0ca-105">Representa um endereço de email classificado.</span><span class="sxs-lookup"><span data-stu-id="2c0ca-105">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="2c0ca-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c0ca-106">Properties</span></span>
| <span data-ttu-id="2c0ca-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c0ca-107">Property</span></span>     | <span data-ttu-id="2c0ca-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c0ca-108">Type</span></span>   |<span data-ttu-id="2c0ca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c0ca-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c0ca-110">address</span><span class="sxs-lookup"><span data-stu-id="2c0ca-110">address</span></span>|<span data-ttu-id="2c0ca-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c0ca-111">string</span></span>|<span data-ttu-id="2c0ca-112">O endereço de email.</span><span class="sxs-lookup"><span data-stu-id="2c0ca-112">The email address.</span></span>|
|<span data-ttu-id="2c0ca-113">classificação</span><span class="sxs-lookup"><span data-stu-id="2c0ca-113">rank</span></span>|<span data-ttu-id="2c0ca-114">double</span><span class="sxs-lookup"><span data-stu-id="2c0ca-114">double</span></span>|<span data-ttu-id="2c0ca-115">A classificação do endereço de email.</span><span class="sxs-lookup"><span data-stu-id="2c0ca-115">The rank of the email address.</span></span> <span data-ttu-id="2c0ca-116">Uma classificação é usada como uma chave de classificação, em relação aos outros resultados retornados.</span><span class="sxs-lookup"><span data-stu-id="2c0ca-116">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="2c0ca-117">Um valor de classificação mais alto corresponde a um resultado mais relevante.</span><span class="sxs-lookup"><span data-stu-id="2c0ca-117">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="2c0ca-118">A relevância é determinada por sinais de comunicação, colaboração e relacionamento comercial.</span><span class="sxs-lookup"><span data-stu-id="2c0ca-118">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c0ca-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c0ca-119">JSON representation</span></span>

<span data-ttu-id="2c0ca-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c0ca-120">Here is a JSON representation of the resource.</span></span>

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
