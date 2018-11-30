---
title: tipo de recurso de rankedEmailAddress
description: Representa um endereço de email classificados.
ms.openlocfilehash: 9234f527ecba6dc83f2e4f80911442d4a083503a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039977"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="06c8b-103">tipo de recurso de rankedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="06c8b-103">rankedEmailAddress resource type</span></span>

> <span data-ttu-id="06c8b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06c8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06c8b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06c8b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06c8b-106">Representa um endereço de email classificados.</span><span class="sxs-lookup"><span data-stu-id="06c8b-106">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="06c8b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06c8b-107">Properties</span></span>
| <span data-ttu-id="06c8b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06c8b-108">Property</span></span>     | <span data-ttu-id="06c8b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="06c8b-109">Type</span></span>   |<span data-ttu-id="06c8b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06c8b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06c8b-111">address</span><span class="sxs-lookup"><span data-stu-id="06c8b-111">address</span></span>|<span data-ttu-id="06c8b-112">string</span><span class="sxs-lookup"><span data-stu-id="06c8b-112">string</span></span>|<span data-ttu-id="06c8b-113">O endereço de email.</span><span class="sxs-lookup"><span data-stu-id="06c8b-113">The email address.</span></span>|
|<span data-ttu-id="06c8b-114">rank</span><span class="sxs-lookup"><span data-stu-id="06c8b-114">rank</span></span>|<span data-ttu-id="06c8b-115">double</span><span class="sxs-lookup"><span data-stu-id="06c8b-115">double</span></span>|<span data-ttu-id="06c8b-116">A classificação do endereço de email.</span><span class="sxs-lookup"><span data-stu-id="06c8b-116">The rank of the email address.</span></span> <span data-ttu-id="06c8b-117">Uma classificação é usada como uma chave de classificação, em relação as outros resultados retornados.</span><span class="sxs-lookup"><span data-stu-id="06c8b-117">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="06c8b-118">Um valor de classificação mais alto corresponde a um resultado mais relevante.</span><span class="sxs-lookup"><span data-stu-id="06c8b-118">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="06c8b-119">A relevância é determinada por sinais de comunicação, colaboração e relacionamento comercial.</span><span class="sxs-lookup"><span data-stu-id="06c8b-119">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06c8b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06c8b-120">JSON representation</span></span>

<span data-ttu-id="06c8b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06c8b-121">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
