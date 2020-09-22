---
title: tipo de recurso de ponto de extremidade
description: O tipo de ponto de extremidade
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c4719632f7d3e2944f1dda81134acc11aa014c06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071514"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="8d948-103">tipo de recurso de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="8d948-103">endpoint resource type</span></span>

<span data-ttu-id="8d948-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="8d948-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d948-105">Representa um ponto de extremidade em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="8d948-105">Represents an endpoint in a call.</span></span> <span data-ttu-id="8d948-106">O ponto de extremidade pode ser o dispositivo de um usuário, uma reunião, um aplicativo/bot, etc. Os tipos [participantEndpoint](callrecords-participantendpoint.md) e [serviceEndpoint](callrecords-serviceendpoint.md) herdam desse tipo.</span><span class="sxs-lookup"><span data-stu-id="8d948-106">The endpoint could be a user's device, a meeting, an application/bot, etc. The [participantEndpoint](callrecords-participantendpoint.md) and [serviceEndpoint](callrecords-serviceendpoint.md) types inherit from this type.</span></span>

## <a name="properties"></a><span data-ttu-id="8d948-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d948-107">Properties</span></span>

| <span data-ttu-id="8d948-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d948-108">Property</span></span>     | <span data-ttu-id="8d948-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d948-109">Type</span></span>        | <span data-ttu-id="8d948-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d948-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d948-111">userAgent</span><span class="sxs-lookup"><span data-stu-id="8d948-111">userAgent</span></span>|[<span data-ttu-id="8d948-112">Microsoft. Graph. callRecords. UserAgent</span><span class="sxs-lookup"><span data-stu-id="8d948-112">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="8d948-113">Agente de usuário relatado por este ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="8d948-113">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d948-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d948-114">JSON representation</span></span>

<span data-ttu-id="8d948-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d948-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.endpoint",
  "baseType": null
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

