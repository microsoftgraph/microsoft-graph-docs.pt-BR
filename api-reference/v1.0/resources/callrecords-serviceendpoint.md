---
title: tipo de recurso serviceEndpoint
description: O tipo de serviceEndpoint
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f9120e1b35974a6e921eb269d289dfc82ba9e532
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491942"
---
# <a name="serviceendpoint-resource-type"></a><span data-ttu-id="caf9d-103">tipo de recurso serviceEndpoint</span><span class="sxs-lookup"><span data-stu-id="caf9d-103">serviceEndpoint resource type</span></span>

<span data-ttu-id="caf9d-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="caf9d-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="caf9d-105">Representa um ponto de extremidade de serviço em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="caf9d-105">Represents a service endpoint in a call.</span></span> <span data-ttu-id="caf9d-106">O ponto de extremidade representa um servidor de mídia de chamada ou outra entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="caf9d-106">The endpoint represents a calling media server or other service entity.</span></span> <span data-ttu-id="caf9d-107">Herda de tipo de [ponto de extremidade](callrecords-endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="caf9d-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="caf9d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="caf9d-108">Properties</span></span>

| <span data-ttu-id="caf9d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="caf9d-109">Property</span></span>     | <span data-ttu-id="caf9d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="caf9d-110">Type</span></span>        | <span data-ttu-id="caf9d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="caf9d-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="caf9d-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="caf9d-112">userAgent</span></span>|[<span data-ttu-id="caf9d-113">Microsoft. Graph. callRecords. UserAgent</span><span class="sxs-lookup"><span data-stu-id="caf9d-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="caf9d-114">Agente de usuário relatado por este ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="caf9d-114">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="caf9d-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="caf9d-115">JSON representation</span></span>

<span data-ttu-id="caf9d-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="caf9d-116">The following is a JSON representation of the resource.</span></span>

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