---
title: tipo de recurso participantEndpoint
description: O tipo participantEndpoint
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ff590acb76d50da9d0772bdaece805a1db0cd26a
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491966"
---
# <a name="participantendpoint-resource-type"></a><span data-ttu-id="3a677-103">tipo de recurso participantEndpoint</span><span class="sxs-lookup"><span data-stu-id="3a677-103">participantEndpoint resource type</span></span>

<span data-ttu-id="3a677-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="3a677-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="3a677-105">Representa um ponto de extremidade de participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="3a677-105">Represents an participant endpoint in a call.</span></span> <span data-ttu-id="3a677-106">O ponto de extremidade representa uma entidade de usuário ou semelhante a um usuário.</span><span class="sxs-lookup"><span data-stu-id="3a677-106">The endpoint represents a user or user-like entity.</span></span> <span data-ttu-id="3a677-107">Herda de tipo de [ponto de extremidade](callrecords-endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="3a677-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="3a677-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a677-108">Properties</span></span>

| <span data-ttu-id="3a677-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a677-109">Property</span></span>     | <span data-ttu-id="3a677-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a677-110">Type</span></span>        | <span data-ttu-id="3a677-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a677-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a677-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="3a677-112">userAgent</span></span>|[<span data-ttu-id="3a677-113">Microsoft. Graph. callRecords. UserAgent</span><span class="sxs-lookup"><span data-stu-id="3a677-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="3a677-114">Agente de usuário relatado por este ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="3a677-114">User-agent reported by this endpoint.</span></span>|
|<span data-ttu-id="3a677-115">comentários</span><span class="sxs-lookup"><span data-stu-id="3a677-115">feedback</span></span>|[<span data-ttu-id="3a677-116">Microsoft. Graph. callRecords. userfeedback</span><span class="sxs-lookup"><span data-stu-id="3a677-116">microsoft.graph.callRecords.userFeedback</span></span>](callrecords-userfeedback.md)|<span data-ttu-id="3a677-117">Os comentários fornecidos pelo usuário deste ponto de extremidade sobre a qualidade da sessão.</span><span class="sxs-lookup"><span data-stu-id="3a677-117">The feedback provided by the user of this endpoint about the quality of the session.</span></span>|
|<span data-ttu-id="3a677-118">ladrões</span><span class="sxs-lookup"><span data-stu-id="3a677-118">identity</span></span>|[<span data-ttu-id="3a677-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="3a677-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="3a677-120">Identidade associada ao ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="3a677-120">Identity associated with the endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a677-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a677-121">JSON representation</span></span>

<span data-ttu-id="3a677-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a677-122">The following is a JSON representation of the resource.</span></span>

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