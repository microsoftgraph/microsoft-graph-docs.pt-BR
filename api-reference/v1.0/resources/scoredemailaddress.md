---
title: tipo de recurso scoredEmailAddress
description: Representa um endereço de email pontuado.
localization_priority: Normal
ms.openlocfilehash: 740173e7d5f93dc875c08508bf73100727fdf415
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819471"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="16afd-103">tipo de recurso scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="16afd-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="16afd-104">Representa um endereço de email pontuado.</span><span class="sxs-lookup"><span data-stu-id="16afd-104">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="16afd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16afd-105">Properties</span></span>
| <span data-ttu-id="16afd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16afd-106">Property</span></span>     | <span data-ttu-id="16afd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="16afd-107">Type</span></span>   |<span data-ttu-id="16afd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="16afd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16afd-109">address</span><span class="sxs-lookup"><span data-stu-id="16afd-109">address</span></span>|<span data-ttu-id="16afd-110">string</span><span class="sxs-lookup"><span data-stu-id="16afd-110">string</span></span>|<span data-ttu-id="16afd-111">O endereço de email.</span><span class="sxs-lookup"><span data-stu-id="16afd-111">The email address.</span></span>|
|<span data-ttu-id="16afd-112">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="16afd-112">relevanceScore</span></span>|<span data-ttu-id="16afd-113">double</span><span class="sxs-lookup"><span data-stu-id="16afd-113">double</span></span>|<span data-ttu-id="16afd-p101">A pontuação de relevância do endereço de email. Uma pontuação de relevância é usada como uma chave de classificação em relação aos outros resultados retornados. Um valor mais alto de pontuação de relevância corresponde a um resultado mais relevante. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="16afd-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16afd-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16afd-118">JSON representation</span></span>

<span data-ttu-id="16afd-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16afd-119">Here is a JSON representation of the resource.</span></span>

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
