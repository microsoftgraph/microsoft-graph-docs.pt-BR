---
title: tipo de recurso feedbackTokenSet
description: O tipo feedbackTokenSet
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0e978bc25615d3fe0f4f39e0e1c5f50d3d5b2ffb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601332"
---
# <a name="feedbacktokenset-resource-type"></a><span data-ttu-id="cf28f-103">tipo de recurso feedbackTokenSet</span><span class="sxs-lookup"><span data-stu-id="cf28f-103">feedbackTokenSet resource type</span></span>

<span data-ttu-id="cf28f-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="cf28f-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="cf28f-105">Este é um _tipo aberto_ que representa o conjunto de tokens de comentários fornecidos pelo usuário deste ponto de extremidade para a sessão.</span><span class="sxs-lookup"><span data-stu-id="cf28f-105">This is an _open type_ that represents the set of feedback tokens provided by the user of this endpoint for the Session.</span></span> <span data-ttu-id="cf28f-106">Este é um conjunto de propriedades booleanas.</span><span class="sxs-lookup"><span data-stu-id="cf28f-106">This is a set of Boolean properties.</span></span> <span data-ttu-id="cf28f-107">Os nomes de propriedade não devem ser dependentes, já que eles podem ser alterados, dependendo de quais tokens são oferecidos para o usuário.</span><span class="sxs-lookup"><span data-stu-id="cf28f-107">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>

## <a name="properties"></a><span data-ttu-id="cf28f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf28f-108">Properties</span></span>

<span data-ttu-id="cf28f-109">Nomes de propriedades explícitas não serão documentados, pois os nomes de token de comentários podem mudar, portanto, este é um [tipo aberto](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span><span class="sxs-lookup"><span data-stu-id="cf28f-109">Explicit property names will not be documented since the feedback token names can change, hence this is an [open type](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf28f-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf28f-110">JSON representation</span></span>

<span data-ttu-id="cf28f-111">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf28f-111">The following is a JSON representation of the resource.</span></span>

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