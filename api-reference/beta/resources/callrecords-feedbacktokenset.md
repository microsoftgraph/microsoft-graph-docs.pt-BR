---
title: tipo de recurso feedbackTokenSet
description: O tipo feedbackTokenSet
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cbf09c70e1df854f1ccba8cb4f8a5fa61c0c24aa
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405601"
---
# <a name="feedbacktokenset-resource-type"></a><span data-ttu-id="0b250-103">tipo de recurso feedbackTokenSet</span><span class="sxs-lookup"><span data-stu-id="0b250-103">feedbackTokenSet resource type</span></span>

<span data-ttu-id="0b250-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="0b250-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b250-105">Este é um _tipo aberto_ que representa o conjunto de tokens de comentários fornecidos pelo usuário deste ponto de extremidade para a sessão.</span><span class="sxs-lookup"><span data-stu-id="0b250-105">This is an _open type_ that represents the set of feedback tokens provided by the user of this endpoint for the Session.</span></span> <span data-ttu-id="0b250-106">Este é um conjunto de propriedades booleanas.</span><span class="sxs-lookup"><span data-stu-id="0b250-106">This is a set of Boolean properties.</span></span> <span data-ttu-id="0b250-107">Os nomes de propriedade não devem ser dependentes, já que eles podem ser alterados, dependendo de quais tokens são oferecidos para o usuário.</span><span class="sxs-lookup"><span data-stu-id="0b250-107">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>

## <a name="properties"></a><span data-ttu-id="0b250-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b250-108">Properties</span></span>

<span data-ttu-id="0b250-109">Nomes de propriedades explícitas não serão documentados, pois os nomes de token de comentários podem mudar, portanto, este é um [tipo aberto](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span><span class="sxs-lookup"><span data-stu-id="0b250-109">Explicit property names will not be documented since the feedback token names can change, hence this is an [open type](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b250-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b250-110">JSON representation</span></span>

<span data-ttu-id="0b250-111">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b250-111">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.feedbackTokenSet",
  "baseType": null
}-->

```json
{
  "DistortedSpeech": true,
  "ElectronicFeedback": false,
  "BackgroundNoise": true,
  "MuffledSpeech": true,
  "Echo": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "feedbackTokenSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->