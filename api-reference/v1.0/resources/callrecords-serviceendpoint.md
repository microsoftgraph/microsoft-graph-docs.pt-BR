---
title: tipo de recurso serviceEndpoint
description: O tipo de serviceEndpoint
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e51d8998ffe332426c617e1b17abd6a6362da77e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069320"
---
# <a name="serviceendpoint-resource-type"></a><span data-ttu-id="531e6-103">tipo de recurso serviceEndpoint</span><span class="sxs-lookup"><span data-stu-id="531e6-103">serviceEndpoint resource type</span></span>

<span data-ttu-id="531e6-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="531e6-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="531e6-105">Representa um ponto de extremidade de serviço em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="531e6-105">Represents a service endpoint in a call.</span></span> <span data-ttu-id="531e6-106">O ponto de extremidade representa um servidor de mídia de chamada ou outra entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="531e6-106">The endpoint represents a calling media server or other service entity.</span></span> <span data-ttu-id="531e6-107">Herda de tipo de [ponto de extremidade](callrecords-endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="531e6-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="531e6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="531e6-108">Properties</span></span>

| <span data-ttu-id="531e6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="531e6-109">Property</span></span>     | <span data-ttu-id="531e6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="531e6-110">Type</span></span>        | <span data-ttu-id="531e6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="531e6-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="531e6-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="531e6-112">userAgent</span></span>|[<span data-ttu-id="531e6-113">Microsoft. Graph. callRecords. UserAgent</span><span class="sxs-lookup"><span data-stu-id="531e6-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="531e6-114">Agente de usuário relatado por este ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="531e6-114">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="531e6-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="531e6-115">JSON representation</span></span>

<span data-ttu-id="531e6-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="531e6-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.serviceEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
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
  "description": "serviceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
