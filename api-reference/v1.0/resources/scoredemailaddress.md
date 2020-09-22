---
title: tipo de recurso scoredEmailAddress
description: Representa um endereço de email pontuado.
localization_priority: Normal
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 11efd8331cf8fca844b912703fa927b627624611
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984135"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="d8f0a-103">tipo de recurso scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d8f0a-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="d8f0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8f0a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8f0a-105">Representa um endereço de email pontuado.</span><span class="sxs-lookup"><span data-stu-id="d8f0a-105">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="d8f0a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8f0a-106">Properties</span></span>
| <span data-ttu-id="d8f0a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8f0a-107">Property</span></span>     | <span data-ttu-id="d8f0a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8f0a-108">Type</span></span>   |<span data-ttu-id="d8f0a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8f0a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8f0a-110">address</span><span class="sxs-lookup"><span data-stu-id="d8f0a-110">address</span></span>|<span data-ttu-id="d8f0a-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8f0a-111">string</span></span>|<span data-ttu-id="d8f0a-112">O endereço de email.</span><span class="sxs-lookup"><span data-stu-id="d8f0a-112">The email address.</span></span>|
|<span data-ttu-id="d8f0a-113">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="d8f0a-113">relevanceScore</span></span>|<span data-ttu-id="d8f0a-114">double</span><span class="sxs-lookup"><span data-stu-id="d8f0a-114">double</span></span>|<span data-ttu-id="d8f0a-p101">A pontuação de relevância do endereço de email. Uma pontuação de relevância é usada como uma chave de classificação em relação aos outros resultados retornados. Um valor mais alto de pontuação de relevância corresponde a um resultado mais relevante. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8f0a-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8f0a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8f0a-119">JSON representation</span></span>

<span data-ttu-id="d8f0a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8f0a-120">Here is a JSON representation of the resource.</span></span>

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

