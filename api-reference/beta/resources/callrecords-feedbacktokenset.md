---
title: tipo de recurso feedbackTokenSet
description: O tipo feedbackTokenSet
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e3f4b0f58fbe2fcd9a920181ccbfca0c5a8c8dad
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394671"
---
# <a name="feedbacktokenset-resource-type"></a><span data-ttu-id="dedfd-103">tipo de recurso feedbackTokenSet</span><span class="sxs-lookup"><span data-stu-id="dedfd-103">feedbackTokenSet resource type</span></span>

<span data-ttu-id="dedfd-104">Namespace: Microsoft. Graph. callRecords</span><span class="sxs-lookup"><span data-stu-id="dedfd-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dedfd-105">Este é um _tipo aberto_ que representa o conjunto de tokens de comentários fornecidos pelo usuário deste ponto de extremidade para a sessão.</span><span class="sxs-lookup"><span data-stu-id="dedfd-105">This is an _open type_ that represents the set of feedback tokens provided by the user of this endpoint for the Session.</span></span> <span data-ttu-id="dedfd-106">Este é um conjunto de propriedades booleanas.</span><span class="sxs-lookup"><span data-stu-id="dedfd-106">This is a set of Boolean properties.</span></span> <span data-ttu-id="dedfd-107">Os nomes de propriedade não devem ser dependentes, já que eles podem ser alterados, dependendo de quais tokens são oferecidos para o usuário.</span><span class="sxs-lookup"><span data-stu-id="dedfd-107">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>

## <a name="properties"></a><span data-ttu-id="dedfd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dedfd-108">Properties</span></span>

<span data-ttu-id="dedfd-109">Nomes de propriedades explícitas não serão documentados, pois os nomes de token de comentários podem mudar, portanto, este é um [tipo aberto](https://docs.microsoft.com/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span><span class="sxs-lookup"><span data-stu-id="dedfd-109">Explicit property names will not be documented since the feedback token names can change, hence this is an [open type](https://docs.microsoft.com/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span></span>

## <a name="json-representation"></a><span data-ttu-id="dedfd-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dedfd-110">JSON representation</span></span>

<span data-ttu-id="dedfd-111">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dedfd-111">The following is a JSON representation of the resource.</span></span>

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