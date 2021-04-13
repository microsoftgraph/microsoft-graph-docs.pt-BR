---
title: Tipo de recurso channelIdentity
description: Representa a identidade de um canal no Microsoft Teams.
author: Kanaka
doc_type: resourcePageType
localization_priority: Normal
ms.prod: teamwork
ms.openlocfilehash: eae8533f549ba0064d9d392fcf60a5baa6479e2c
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697913"
---
# <a name="channelidentity-resource-type"></a><span data-ttu-id="3fb7d-103">Tipo de recurso channelIdentity</span><span class="sxs-lookup"><span data-stu-id="3fb7d-103">channelIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="3fb7d-104">Contém informações básicas de identificação sobre um canal no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3fb7d-104">Contains basic identification information about a channel in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="3fb7d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3fb7d-105">Properties</span></span>

| <span data-ttu-id="3fb7d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fb7d-106">Property</span></span>   | <span data-ttu-id="3fb7d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fb7d-107">Type</span></span> |<span data-ttu-id="3fb7d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fb7d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fb7d-109">channelId</span><span class="sxs-lookup"><span data-stu-id="3fb7d-109">channelId</span></span>|<span data-ttu-id="3fb7d-110">string</span><span class="sxs-lookup"><span data-stu-id="3fb7d-110">string</span></span>|  <span data-ttu-id="3fb7d-111">A identidade do canal no qual a mensagem foi postada.</span><span class="sxs-lookup"><span data-stu-id="3fb7d-111">The identity of the channel in which the message was posted.</span></span>|
|<span data-ttu-id="3fb7d-112">teamId</span><span class="sxs-lookup"><span data-stu-id="3fb7d-112">teamId</span></span>|<span data-ttu-id="3fb7d-113">string</span><span class="sxs-lookup"><span data-stu-id="3fb7d-113">string</span></span>|  <span data-ttu-id="3fb7d-114">A identidade da equipe na qual a mensagem foi postada.</span><span class="sxs-lookup"><span data-stu-id="3fb7d-114">The identity of the team in which the message was posted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fb7d-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3fb7d-115">JSON representation</span></span>

<span data-ttu-id="3fb7d-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3fb7d-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "@odata.type": "microsoft.graph.channelIdentity"
}-->

```json
{
   "channelId":"string",
   "teamId":"string"
}
```

<!-- uuid: 4DFA000D-1A5F-4299-B3DD-835E4DD2F3BF
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel identity  resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
