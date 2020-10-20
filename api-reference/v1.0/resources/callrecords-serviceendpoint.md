---
title: tipo de recurso serviceEndpoint
description: O tipo de serviceEndpoint
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b650b2f105a9feb2d33327a0ceef9add18716d00
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601563"
---
# <a name="serviceendpoint-resource-type"></a><span data-ttu-id="bff07-103">tipo de recurso serviceEndpoint</span><span class="sxs-lookup"><span data-stu-id="bff07-103">serviceEndpoint resource type</span></span>

<span data-ttu-id="bff07-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="bff07-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="bff07-105">Representa um ponto de extremidade de serviço em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="bff07-105">Represents a service endpoint in a call.</span></span> <span data-ttu-id="bff07-106">O ponto de extremidade representa um servidor de mídia de chamada ou outra entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="bff07-106">The endpoint represents a calling media server or other service entity.</span></span> <span data-ttu-id="bff07-107">Herda de tipo de [ponto de extremidade](callrecords-endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="bff07-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="bff07-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bff07-108">Properties</span></span>

| <span data-ttu-id="bff07-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bff07-109">Property</span></span>     | <span data-ttu-id="bff07-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bff07-110">Type</span></span>        | <span data-ttu-id="bff07-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bff07-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bff07-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="bff07-112">userAgent</span></span>|[<span data-ttu-id="bff07-113">Microsoft. Graph. callRecords. UserAgent</span><span class="sxs-lookup"><span data-stu-id="bff07-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="bff07-114">Agente de usuário relatado por este ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="bff07-114">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bff07-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bff07-115">JSON representation</span></span>

<span data-ttu-id="bff07-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bff07-116">The following is a JSON representation of the resource.</span></span>

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
