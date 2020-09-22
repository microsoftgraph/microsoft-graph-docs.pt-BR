---
title: tipo de recurso participantEndpoint
description: O tipo participantEndpoint
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e2b05ce7e5921c5436d47aeb6b93a99f68a579e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071380"
---
# <a name="participantendpoint-resource-type"></a><span data-ttu-id="7bb6b-103">tipo de recurso participantEndpoint</span><span class="sxs-lookup"><span data-stu-id="7bb6b-103">participantEndpoint resource type</span></span>

<span data-ttu-id="7bb6b-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="7bb6b-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bb6b-105">Representa um ponto de extremidade de participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="7bb6b-105">Represents an participant endpoint in a call.</span></span> <span data-ttu-id="7bb6b-106">O ponto de extremidade representa uma entidade de usuário ou semelhante a um usuário.</span><span class="sxs-lookup"><span data-stu-id="7bb6b-106">The endpoint represents a user or user-like entity.</span></span> <span data-ttu-id="7bb6b-107">Herda de tipo de [ponto de extremidade](callrecords-endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="7bb6b-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="7bb6b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bb6b-108">Properties</span></span>

| <span data-ttu-id="7bb6b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bb6b-109">Property</span></span>     | <span data-ttu-id="7bb6b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bb6b-110">Type</span></span>        | <span data-ttu-id="7bb6b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bb6b-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7bb6b-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="7bb6b-112">userAgent</span></span>|[<span data-ttu-id="7bb6b-113">Microsoft. Graph. callRecords. UserAgent</span><span class="sxs-lookup"><span data-stu-id="7bb6b-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="7bb6b-114">Agente de usuário relatado por este ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="7bb6b-114">User-agent reported by this endpoint.</span></span>|
|<span data-ttu-id="7bb6b-115">comentários</span><span class="sxs-lookup"><span data-stu-id="7bb6b-115">feedback</span></span>|[<span data-ttu-id="7bb6b-116">Microsoft. Graph. callRecords. userfeedback</span><span class="sxs-lookup"><span data-stu-id="7bb6b-116">microsoft.graph.callRecords.userFeedback</span></span>](callrecords-userfeedback.md)|<span data-ttu-id="7bb6b-117">Os comentários fornecidos pelo usuário deste ponto de extremidade sobre a qualidade da sessão.</span><span class="sxs-lookup"><span data-stu-id="7bb6b-117">The feedback provided by the user of this endpoint about the quality of the session.</span></span>|
|<span data-ttu-id="7bb6b-118">ladrões</span><span class="sxs-lookup"><span data-stu-id="7bb6b-118">identity</span></span>|[<span data-ttu-id="7bb6b-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="7bb6b-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="7bb6b-120">Identidade associada ao ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="7bb6b-120">Identity associated with the endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bb6b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bb6b-121">JSON representation</span></span>

<span data-ttu-id="7bb6b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bb6b-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.participantEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"},
  "feedback": {"@odata.type": "microsoft.graph.callRecords.userFeedback"},
  "identity": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

