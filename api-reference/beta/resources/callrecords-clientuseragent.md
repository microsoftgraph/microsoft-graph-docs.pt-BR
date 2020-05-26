---
title: tipo de recurso clientUserAgent
description: O tipo clientUserAgent
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6e985d99c1fb86c71b862d0f055af96eba2c2a66
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353620"
---
# <a name="clientuseragent-resource-type"></a><span data-ttu-id="1d1ae-103">tipo de recurso clientUserAgent</span><span class="sxs-lookup"><span data-stu-id="1d1ae-103">clientUserAgent resource type</span></span>

<span data-ttu-id="1d1ae-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="1d1ae-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d1ae-105">Representa um agente de usuário do cliente de um ponto de extremidade em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="1d1ae-105">Represents a client user agent of an endpoint in a call.</span></span> <span data-ttu-id="1d1ae-106">Herda do tipo [UserAgent](callrecords-useragent.md) .</span><span class="sxs-lookup"><span data-stu-id="1d1ae-106">Inherits from the [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="1d1ae-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d1ae-107">Properties</span></span>

| <span data-ttu-id="1d1ae-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d1ae-108">Property</span></span>     | <span data-ttu-id="1d1ae-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d1ae-109">Type</span></span>        | <span data-ttu-id="1d1ae-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d1ae-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d1ae-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="1d1ae-111">applicationVersion</span></span>|<span data-ttu-id="1d1ae-112">String</span><span class="sxs-lookup"><span data-stu-id="1d1ae-112">String</span></span>|<span data-ttu-id="1d1ae-113">Identifica a versão do software do aplicativo usado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="1d1ae-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="1d1ae-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="1d1ae-114">headerValue</span></span>|<span data-ttu-id="1d1ae-115">String</span><span class="sxs-lookup"><span data-stu-id="1d1ae-115">String</span></span>|<span data-ttu-id="1d1ae-116">Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="1d1ae-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="1d1ae-117">platform</span><span class="sxs-lookup"><span data-stu-id="1d1ae-117">platform</span></span>|<span data-ttu-id="1d1ae-118">Microsoft. Graph. callRecords. clientPlatform</span><span class="sxs-lookup"><span data-stu-id="1d1ae-118">microsoft.graph.callRecords.clientPlatform</span></span>|<span data-ttu-id="1d1ae-119">Identifica a plataforma usada por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="1d1ae-119">Identifies the platform used by this endpoint.</span></span> <span data-ttu-id="1d1ae-120">Os valores possíveis são: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1d1ae-120">Possible values are: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1d1ae-121">productFamily</span><span class="sxs-lookup"><span data-stu-id="1d1ae-121">productFamily</span></span>|<span data-ttu-id="1d1ae-122">Microsoft. Graph. callRecords. productFamily</span><span class="sxs-lookup"><span data-stu-id="1d1ae-122">microsoft.graph.callRecords.productFamily</span></span>|<span data-ttu-id="1d1ae-123">Identifica a família de software de aplicativo usada por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="1d1ae-123">Identifies the family of application software used by this endpoint.</span></span> <span data-ttu-id="1d1ae-124">Os valores possíveis são: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1d1ae-124">Possible values are: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d1ae-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d1ae-125">JSON representation</span></span>

<span data-ttu-id="1d1ae-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d1ae-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.clientUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "platform": "String",
  "productFamily": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "clientUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->