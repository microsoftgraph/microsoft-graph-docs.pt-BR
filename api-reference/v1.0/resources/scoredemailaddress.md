---
title: tipo de recurso scoredEmailAddress
description: Representa um endereço de email pontuado.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b8cdcd7a0192bdd97bc096ce06514e75a7184f63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034591"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="01bc9-103">tipo de recurso scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="01bc9-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="01bc9-104">Representa um endereço de email pontuado.</span><span class="sxs-lookup"><span data-stu-id="01bc9-104">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="01bc9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01bc9-105">Properties</span></span>
| <span data-ttu-id="01bc9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01bc9-106">Property</span></span>     | <span data-ttu-id="01bc9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="01bc9-107">Type</span></span>   |<span data-ttu-id="01bc9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="01bc9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01bc9-109">address</span><span class="sxs-lookup"><span data-stu-id="01bc9-109">address</span></span>|<span data-ttu-id="01bc9-110">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01bc9-110">string</span></span>|<span data-ttu-id="01bc9-111">O endereço de email.</span><span class="sxs-lookup"><span data-stu-id="01bc9-111">The email address.</span></span>|
|<span data-ttu-id="01bc9-112">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="01bc9-112">relevanceScore</span></span>|<span data-ttu-id="01bc9-113">double</span><span class="sxs-lookup"><span data-stu-id="01bc9-113">double</span></span>|<span data-ttu-id="01bc9-p101">A pontuação de relevância do endereço de email. Uma pontuação de relevância é usada como uma chave de classificação em relação aos outros resultados retornados. Um valor mais alto de pontuação de relevância corresponde a um resultado mais relevante. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="01bc9-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="01bc9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01bc9-118">JSON representation</span></span>

<span data-ttu-id="01bc9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01bc9-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
