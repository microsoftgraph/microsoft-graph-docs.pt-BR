---
title: tipo de recurso teleconferenceDeviceVideoQuality
description: Representa dados de qualidade de vídeo do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8f892fe059828cd7fd71ec19914b5b5db0b9e3cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086225"
---
# <a name="teleconferencedevicevideoquality-resource-type"></a><span data-ttu-id="85697-103">tipo de recurso teleconferenceDeviceVideoQuality</span><span class="sxs-lookup"><span data-stu-id="85697-103">teleconferenceDeviceVideoQuality resource type</span></span>

<span data-ttu-id="85697-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85697-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85697-105">Representa dados de qualidade de vídeo do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="85697-105">Represents video teleconferencing device video quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="85697-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85697-106">Properties</span></span>

<span data-ttu-id="85697-107">O recurso **teleconferenceDeviceVideoQuality** herda as propriedades de [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)e inclui as seguintes propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="85697-107">The **teleconferenceDeviceVideoQuality** resource inherits the properties from [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md), and includes the following additional properties.</span></span>

| <span data-ttu-id="85697-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85697-108">Property</span></span>     | <span data-ttu-id="85697-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="85697-109">Type</span></span>        | <span data-ttu-id="85697-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="85697-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="85697-111">averageInboundBitRate</span><span class="sxs-lookup"><span data-stu-id="85697-111">averageInboundBitRate</span></span>|<span data-ttu-id="85697-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="85697-112">Double</span></span>|<span data-ttu-id="85697-113">A taxa média de bits de vídeo de fluxo de entrada por segundo.</span><span class="sxs-lookup"><span data-stu-id="85697-113">The average inbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="85697-114">averageInboundFrameRate</span><span class="sxs-lookup"><span data-stu-id="85697-114">averageInboundFrameRate</span></span>|<span data-ttu-id="85697-115">Duplo</span><span class="sxs-lookup"><span data-stu-id="85697-115">Double</span></span>|<span data-ttu-id="85697-116">A taxa média de quadros de vídeo de fluxo de entrada por segundo.</span><span class="sxs-lookup"><span data-stu-id="85697-116">The average inbound stream video frame rate per second.</span></span>|
|<span data-ttu-id="85697-117">averageOutboundBitRate</span><span class="sxs-lookup"><span data-stu-id="85697-117">averageOutboundBitRate</span></span>|<span data-ttu-id="85697-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="85697-118">Double</span></span>|<span data-ttu-id="85697-119">A taxa média de bits de vídeo de fluxo de saída por segundo.</span><span class="sxs-lookup"><span data-stu-id="85697-119">The average outbound stream video bit rate per second.</span></span>|
|<span data-ttu-id="85697-120">averageOutboundFrameRate</span><span class="sxs-lookup"><span data-stu-id="85697-120">averageOutboundFrameRate</span></span>|<span data-ttu-id="85697-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="85697-121">Double</span></span>|<span data-ttu-id="85697-122">A taxa média de quadros de vídeo de fluxo de saída por segundo.</span><span class="sxs-lookup"><span data-stu-id="85697-122">The average outbound stream video frame rate per second.</span></span>|

### <a name="derived-types"></a><span data-ttu-id="85697-123">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="85697-123">Derived types</span></span>

| <span data-ttu-id="85697-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="85697-124">Type</span></span>                                                 | <span data-ttu-id="85697-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="85697-125">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="85697-126">teleconferenceDeviceScreenSharingQuality</span><span class="sxs-lookup"><span data-stu-id="85697-126">teleconferenceDeviceScreenSharingQuality</span></span>](teleconferencedevicescreensharingquality.md)    | <span data-ttu-id="85697-127">Dados de qualidade de compartilhamento de tela do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="85697-127">Video teleconferencing device screen-sharing quality data.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85697-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85697-128">JSON representation</span></span>

<span data-ttu-id="85697-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85697-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceVideoQuality",
  "baseType": "microsoft.graph.teleconferenceDeviceMediaQuality"
}-->

```json
{
  "averageInboundBitRate": 1024,
  "averageInboundFrameRate": 1024,
  "averageInboundJitter": "String (ISO 8601 duration)",
  "averageInboundPacketLossRateInPercentage": 10,
  "averageInboundRoundTripDelay": "String (ISO 8601 duration)",
  "averageOutboundBitRate": 1024,
  "averageOutboundFrameRate": 1024,
  "averageOutboundJitter": "String (ISO 8601 duration)",
  "averageOutboundPacketLossRateInPercentage": 10,
  "averageOutboundRoundTripDelay": "String (ISO 8601 duration)",
  "channelIndex": 1,
  "inboundPackets": 1024,
  "localIPAddress": "String",
  "localPort": 2000,
  "maximumInboundJitter": "String (ISO 8601 duration)",
  "maximumInboundPacketLossRateInPercentage": 12,
  "maximumInboundRoundTripDelay": "String (ISO 8601 duration)",
  "maximumOutboundJitter": "String (ISO 8601 duration)",
  "maximumOutboundPacketLossRateInPercentage": 12,
  "maximumOutboundRoundTripDelay": "String (ISO 8601 duration)",
  "mediaDuration": "String (ISO 8601 duration)",
  "networkLinkSpeedInBytes": 1000000,
  "outboundPackets": 1024,
  "remoteIPAddress": "String",
  "remotePort": 3000
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceVideoQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

