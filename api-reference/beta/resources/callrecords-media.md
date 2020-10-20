---
title: tipo de recurso de mídia
description: O tipo de mídia
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9245d9c030c15d17b286338aa7887333b26f2678
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601164"
---
# <a name="media-resource-type"></a><span data-ttu-id="261b0-103">tipo de recurso de mídia</span><span class="sxs-lookup"><span data-stu-id="261b0-103">media resource type</span></span>

<span data-ttu-id="261b0-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="261b0-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="261b0-105">Representa a mídia (áudio, vídeo, compartilhamento de tela baseado em vídeo, etc.) usada em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="261b0-105">Represents the media (audio, video, video-based screen-sharing, etc.) used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="261b0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="261b0-106">Properties</span></span>

| <span data-ttu-id="261b0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="261b0-107">Property</span></span>     | <span data-ttu-id="261b0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="261b0-108">Type</span></span>        | <span data-ttu-id="261b0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="261b0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="261b0-110">rótulo</span><span class="sxs-lookup"><span data-stu-id="261b0-110">label</span></span>|<span data-ttu-id="261b0-111">String</span><span class="sxs-lookup"><span data-stu-id="261b0-111">String</span></span>|<span data-ttu-id="261b0-112">Como a mídia foi identificada durante o estágio de negociação de mídia.</span><span class="sxs-lookup"><span data-stu-id="261b0-112">How the media was identified during media negotiation stage.</span></span>|
|<span data-ttu-id="261b0-113">callerDevice</span><span class="sxs-lookup"><span data-stu-id="261b0-113">callerDevice</span></span>|[<span data-ttu-id="261b0-114">Microsoft. Graph. callRecords. deviceInfo</span><span class="sxs-lookup"><span data-stu-id="261b0-114">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="261b0-115">Informações do dispositivo associadas ao ponto de extremidade do chamador desta mídia.</span><span class="sxs-lookup"><span data-stu-id="261b0-115">Device information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="261b0-116">callerNetwork</span><span class="sxs-lookup"><span data-stu-id="261b0-116">callerNetwork</span></span>|[<span data-ttu-id="261b0-117">Microsoft. Graph. callRecords. networkInfo</span><span class="sxs-lookup"><span data-stu-id="261b0-117">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="261b0-118">Informações de rede associadas ao ponto de extremidade do chamador desta mídia.</span><span class="sxs-lookup"><span data-stu-id="261b0-118">Network information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="261b0-119">calleeDevice</span><span class="sxs-lookup"><span data-stu-id="261b0-119">calleeDevice</span></span>|[<span data-ttu-id="261b0-120">Microsoft. Graph. callRecords. deviceInfo</span><span class="sxs-lookup"><span data-stu-id="261b0-120">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="261b0-121">Informações do dispositivo associadas ao ponto de extremidade do receptor desta mídia.</span><span class="sxs-lookup"><span data-stu-id="261b0-121">Device information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="261b0-122">calleeNetwork</span><span class="sxs-lookup"><span data-stu-id="261b0-122">calleeNetwork</span></span>|[<span data-ttu-id="261b0-123">Microsoft. Graph. callRecords. networkInfo</span><span class="sxs-lookup"><span data-stu-id="261b0-123">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="261b0-124">Informações de rede associadas ao ponto de extremidade chamado desta mídia.</span><span class="sxs-lookup"><span data-stu-id="261b0-124">Network information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="261b0-125">streaming</span><span class="sxs-lookup"><span data-stu-id="261b0-125">streams</span></span>|<span data-ttu-id="261b0-126">coleção [Microsoft. Graph. callRecords. mediaStream](callrecords-mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="261b0-126">[microsoft.graph.callRecords.mediaStream](callrecords-mediastream.md) collection</span></span>|<span data-ttu-id="261b0-127">Fluxos de rede associados a essa mídia.</span><span class="sxs-lookup"><span data-stu-id="261b0-127">Network streams associated with this media.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="261b0-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="261b0-128">JSON representation</span></span>

<span data-ttu-id="261b0-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="261b0-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.media",
  "baseType": null
}-->

```json
{
  "label": "String",
  "callerDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "callerNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "calleeDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "calleeNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "streams": [{"@odata.type": "microsoft.graph.callRecords.mediaStream"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "media resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

