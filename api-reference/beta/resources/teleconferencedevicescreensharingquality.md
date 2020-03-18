---
title: tipo de recurso teleconferenceDeviceScreenSharingQuality
description: Representa os dados de qualidade de compartilhamento de tela do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 86f692a235bc065a93fe00a87bae3139b64f669e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763302"
---
# <a name="teleconferencedevicescreensharingquality-resource-type"></a><span data-ttu-id="ac020-103">tipo de recurso teleconferenceDeviceScreenSharingQuality</span><span class="sxs-lookup"><span data-stu-id="ac020-103">teleconferenceDeviceScreenSharingQuality resource type</span></span>

<span data-ttu-id="ac020-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac020-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac020-105">Representa os dados de qualidade de compartilhamento de tela do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="ac020-105">Represents video teleconferencing device screen-sharing quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="ac020-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac020-106">Properties</span></span>

<span data-ttu-id="ac020-107">O **teleconferenceDeviceScreenSharingQuality** herda todas as propriedades de [teleconferenceDeviceVideoQuality](teleconferencedevicevideoquality.md).</span><span class="sxs-lookup"><span data-stu-id="ac020-107">The **teleconferenceDeviceScreenSharingQuality** inherits all the properties from [teleconferenceDeviceVideoQuality](teleconferencedevicevideoquality.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac020-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac020-108">JSON representation</span></span>

<span data-ttu-id="ac020-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac020-109">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceScreenSharingQuality",
  "baseType": "microsoft.graph.teleconferenceDeviceVideoQuality"
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
  "description": "teleconferenceDeviceScreenSharingQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
