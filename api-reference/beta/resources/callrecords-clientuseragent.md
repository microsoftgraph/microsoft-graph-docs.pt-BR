---
title: tipo de recurso clientUserAgent
description: O tipo clientUserAgent
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1833972fc97559cf10dac75e08ab11b5fe633a81
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071530"
---
# <a name="clientuseragent-resource-type"></a><span data-ttu-id="7aa48-103">tipo de recurso clientUserAgent</span><span class="sxs-lookup"><span data-stu-id="7aa48-103">clientUserAgent resource type</span></span>

<span data-ttu-id="7aa48-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="7aa48-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aa48-105">Representa um agente de usuário do cliente de um ponto de extremidade em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="7aa48-105">Represents a client user agent of an endpoint in a call.</span></span> <span data-ttu-id="7aa48-106">Herda do tipo [UserAgent](callrecords-useragent.md) .</span><span class="sxs-lookup"><span data-stu-id="7aa48-106">Inherits from the [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="7aa48-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7aa48-107">Properties</span></span>

| <span data-ttu-id="7aa48-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7aa48-108">Property</span></span>     | <span data-ttu-id="7aa48-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aa48-109">Type</span></span>        | <span data-ttu-id="7aa48-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aa48-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7aa48-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="7aa48-111">applicationVersion</span></span>|<span data-ttu-id="7aa48-112">String</span><span class="sxs-lookup"><span data-stu-id="7aa48-112">String</span></span>|<span data-ttu-id="7aa48-113">Identifica a versão do software do aplicativo usado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="7aa48-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="7aa48-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="7aa48-114">headerValue</span></span>|<span data-ttu-id="7aa48-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7aa48-115">String</span></span>|<span data-ttu-id="7aa48-116">Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="7aa48-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="7aa48-117">plataforma</span><span class="sxs-lookup"><span data-stu-id="7aa48-117">platform</span></span>|<span data-ttu-id="7aa48-118">Microsoft. Graph. callRecords. clientPlatform</span><span class="sxs-lookup"><span data-stu-id="7aa48-118">microsoft.graph.callRecords.clientPlatform</span></span>|<span data-ttu-id="7aa48-119">Identifica a plataforma usada por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="7aa48-119">Identifies the platform used by this endpoint.</span></span> <span data-ttu-id="7aa48-120">Os valores possíveis são: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7aa48-120">Possible values are: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7aa48-121">productFamily</span><span class="sxs-lookup"><span data-stu-id="7aa48-121">productFamily</span></span>|<span data-ttu-id="7aa48-122">Microsoft. Graph. callRecords. productFamily</span><span class="sxs-lookup"><span data-stu-id="7aa48-122">microsoft.graph.callRecords.productFamily</span></span>|<span data-ttu-id="7aa48-123">Identifica a família de software de aplicativo usada por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="7aa48-123">Identifies the family of application software used by this endpoint.</span></span> <span data-ttu-id="7aa48-124">Os valores possíveis são: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7aa48-124">Possible values are: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7aa48-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7aa48-125">JSON representation</span></span>

<span data-ttu-id="7aa48-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7aa48-126">The following is a JSON representation of the resource.</span></span>

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

