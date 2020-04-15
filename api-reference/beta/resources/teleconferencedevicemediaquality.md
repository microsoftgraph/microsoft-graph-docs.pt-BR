---
title: tipo de recurso teleconferenceDeviceMediaQuality
description: Dados de qualidade de mídia do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6fa0bc09f2f6038dd49c8c804420ce042bd5ec93
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510580"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a><span data-ttu-id="ab463-103">tipo de recurso teleconferenceDeviceMediaQuality</span><span class="sxs-lookup"><span data-stu-id="ab463-103">teleconferenceDeviceMediaQuality resource type</span></span>

<span data-ttu-id="ab463-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab463-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab463-105">Representa dados de qualidade de mídia do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="ab463-105">Represents video teleconferencing device media quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="ab463-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab463-106">Properties</span></span>

| <span data-ttu-id="ab463-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab463-107">Property</span></span>     | <span data-ttu-id="ab463-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab463-108">Type</span></span>        | <span data-ttu-id="ab463-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab463-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ab463-110">averageInboundJitter</span><span class="sxs-lookup"><span data-stu-id="ab463-110">averageInboundJitter</span></span>|<span data-ttu-id="ab463-111">Duração</span><span class="sxs-lookup"><span data-stu-id="ab463-111">Duration</span></span>|<span data-ttu-id="ab463-112">A tremulação média da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="ab463-112">The average inbound stream network jitter.</span></span>|
|<span data-ttu-id="ab463-113">averageInboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="ab463-113">averageInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="ab463-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="ab463-114">Double</span></span>|<span data-ttu-id="ab463-115">A taxa média de perda de pacote de fluxo de entrada em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="ab463-115">The average inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="ab463-116">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="ab463-116">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="ab463-117">averageInboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="ab463-117">averageInboundRoundTripDelay</span></span>|<span data-ttu-id="ab463-118">Duração</span><span class="sxs-lookup"><span data-stu-id="ab463-118">Duration</span></span>|<span data-ttu-id="ab463-119">O intervalo médio de ida e volta da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="ab463-119">The average inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="ab463-120">averageOutboundJitter</span><span class="sxs-lookup"><span data-stu-id="ab463-120">averageOutboundJitter</span></span>|<span data-ttu-id="ab463-121">Duração</span><span class="sxs-lookup"><span data-stu-id="ab463-121">Duration</span></span>|<span data-ttu-id="ab463-122">A tremulação média da rede de fluxo de saída.</span><span class="sxs-lookup"><span data-stu-id="ab463-122">The average outbound stream network jitter.</span></span>|
|<span data-ttu-id="ab463-123">averageOutboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="ab463-123">averageOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="ab463-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="ab463-124">Double</span></span>|<span data-ttu-id="ab463-125">A taxa média de perda de pacotes de fluxo de saída em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="ab463-125">The average outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="ab463-126">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="ab463-126">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="ab463-127">averageOutboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="ab463-127">averageOutboundRoundTripDelay</span></span>|<span data-ttu-id="ab463-128">Duração</span><span class="sxs-lookup"><span data-stu-id="ab463-128">Duration</span></span>|<span data-ttu-id="ab463-129">O intervalo médio de ida e volta da rede de fluxo de saída.</span><span class="sxs-lookup"><span data-stu-id="ab463-129">The average outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="ab463-130">channelIndex</span><span class="sxs-lookup"><span data-stu-id="ab463-130">channelIndex</span></span>|<span data-ttu-id="ab463-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ab463-131">Int32</span></span>|<span data-ttu-id="ab463-132">O índice de canal da mídia.</span><span class="sxs-lookup"><span data-stu-id="ab463-132">The channel index of media.</span></span> <span data-ttu-id="ab463-133">A indexação começa com 1.</span><span class="sxs-lookup"><span data-stu-id="ab463-133">Indexing begins with 1.</span></span>  <span data-ttu-id="ab463-134">Se uma sessão de mídia contiver três modalidades de vídeo, os índices de canal serão 1, 2 e 3.</span><span class="sxs-lookup"><span data-stu-id="ab463-134">If a media session contains 3 video modalities, channel indexes will be 1, 2, and 3.</span></span>|
|<span data-ttu-id="ab463-135">inboundPackets</span><span class="sxs-lookup"><span data-stu-id="ab463-135">inboundPackets</span></span>|<span data-ttu-id="ab463-136">Int64</span><span class="sxs-lookup"><span data-stu-id="ab463-136">Int64</span></span>|<span data-ttu-id="ab463-137">O número total de pacotes de entrada.</span><span class="sxs-lookup"><span data-stu-id="ab463-137">The total number of the inbound packets.</span></span>|
|<span data-ttu-id="ab463-138">localIPAddress</span><span class="sxs-lookup"><span data-stu-id="ab463-138">localIPAddress</span></span>|<span data-ttu-id="ab463-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab463-139">String</span></span>|<span data-ttu-id="ab463-140">o endereço IP local da sessão de mídia.</span><span class="sxs-lookup"><span data-stu-id="ab463-140">the local IP address for the media session.</span></span>|
|<span data-ttu-id="ab463-141">localPort</span><span class="sxs-lookup"><span data-stu-id="ab463-141">localPort</span></span>|<span data-ttu-id="ab463-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ab463-142">Int32</span></span>|<span data-ttu-id="ab463-143">A porta de mídia local.</span><span class="sxs-lookup"><span data-stu-id="ab463-143">The local media port.</span></span>|
|<span data-ttu-id="ab463-144">maximumInboundJitter</span><span class="sxs-lookup"><span data-stu-id="ab463-144">maximumInboundJitter</span></span>|<span data-ttu-id="ab463-145">Duração</span><span class="sxs-lookup"><span data-stu-id="ab463-145">Duration</span></span>|<span data-ttu-id="ab463-146">A tremulação máxima da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="ab463-146">The maximum inbound stream network jitter.</span></span>|
|<span data-ttu-id="ab463-147">maximumInboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="ab463-147">maximumInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="ab463-148">Duplo</span><span class="sxs-lookup"><span data-stu-id="ab463-148">Double</span></span>|<span data-ttu-id="ab463-149">A taxa máxima de perda de pacote de fluxo de entrada em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="ab463-149">The maximum inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="ab463-150">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="ab463-150">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="ab463-151">maximumInboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="ab463-151">maximumInboundRoundTripDelay</span></span>|<span data-ttu-id="ab463-152">Duração</span><span class="sxs-lookup"><span data-stu-id="ab463-152">Duration</span></span>|<span data-ttu-id="ab463-153">O intervalo máximo de ida e volta da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="ab463-153">The maximum inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="ab463-154">maximumOutboundJitter</span><span class="sxs-lookup"><span data-stu-id="ab463-154">maximumOutboundJitter</span></span>|<span data-ttu-id="ab463-155">Duração</span><span class="sxs-lookup"><span data-stu-id="ab463-155">Duration</span></span>|<span data-ttu-id="ab463-156">A tremulação de rede de fluxo de saída máximo.</span><span class="sxs-lookup"><span data-stu-id="ab463-156">The maximum outbound stream network jitter.</span></span>|
|<span data-ttu-id="ab463-157">maximumOutboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="ab463-157">maximumOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="ab463-158">Duplo</span><span class="sxs-lookup"><span data-stu-id="ab463-158">Double</span></span>|<span data-ttu-id="ab463-159">A taxa máxima de perda de pacotes de fluxo de saída em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="ab463-159">The maximum outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="ab463-160">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="ab463-160">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="ab463-161">maximumOutboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="ab463-161">maximumOutboundRoundTripDelay</span></span>|<span data-ttu-id="ab463-162">Duração</span><span class="sxs-lookup"><span data-stu-id="ab463-162">Duration</span></span>|<span data-ttu-id="ab463-163">O atraso máximo de ida e volta da rede de fluxo de saída.</span><span class="sxs-lookup"><span data-stu-id="ab463-163">The maximum outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="ab463-164">mediaDuration</span><span class="sxs-lookup"><span data-stu-id="ab463-164">mediaDuration</span></span>|<span data-ttu-id="ab463-165">Duração</span><span class="sxs-lookup"><span data-stu-id="ab463-165">Duration</span></span>|<span data-ttu-id="ab463-166">A duração da modalidade total.</span><span class="sxs-lookup"><span data-stu-id="ab463-166">The total modality duration.</span></span> <span data-ttu-id="ab463-167">Se a mídia habilitada e desabilitada várias vezes, MediaDuration será a soma de todas as durações.</span><span class="sxs-lookup"><span data-stu-id="ab463-167">If the media enabled and disabled multiple times, MediaDuration will the summation of all of the durations.</span></span>|
|<span data-ttu-id="ab463-168">networkLinkSpeedInBytes</span><span class="sxs-lookup"><span data-stu-id="ab463-168">networkLinkSpeedInBytes</span></span>|<span data-ttu-id="ab463-169">Int64</span><span class="sxs-lookup"><span data-stu-id="ab463-169">Int64</span></span>|<span data-ttu-id="ab463-170">A velocidade do link de rede em bytes</span><span class="sxs-lookup"><span data-stu-id="ab463-170">The network link speed in bytes</span></span>|
|<span data-ttu-id="ab463-171">outboundPackets</span><span class="sxs-lookup"><span data-stu-id="ab463-171">outboundPackets</span></span>|<span data-ttu-id="ab463-172">Int64</span><span class="sxs-lookup"><span data-stu-id="ab463-172">Int64</span></span>|<span data-ttu-id="ab463-173">O número total dos pacotes de saída.</span><span class="sxs-lookup"><span data-stu-id="ab463-173">The total number of the outbound packets.</span></span>|
|<span data-ttu-id="ab463-174">remoteIPAddress</span><span class="sxs-lookup"><span data-stu-id="ab463-174">remoteIPAddress</span></span>|<span data-ttu-id="ab463-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab463-175">String</span></span>|<span data-ttu-id="ab463-176">O endereço IP remoto da sessão de mídia.</span><span class="sxs-lookup"><span data-stu-id="ab463-176">The remote IP address for the media session.</span></span>|
|<span data-ttu-id="ab463-177">remotePort</span><span class="sxs-lookup"><span data-stu-id="ab463-177">remotePort</span></span>|<span data-ttu-id="ab463-178">Int32</span><span class="sxs-lookup"><span data-stu-id="ab463-178">Int32</span></span>|<span data-ttu-id="ab463-179">A porta de mídia remota.</span><span class="sxs-lookup"><span data-stu-id="ab463-179">The remote media port.</span></span>|

### <a name="derived-types"></a><span data-ttu-id="ab463-180">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="ab463-180">Derived types</span></span>

| <span data-ttu-id="ab463-181">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab463-181">Type</span></span>                                                 | <span data-ttu-id="ab463-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab463-182">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="ab463-183">teleconferenceDeviceAudioQuality</span><span class="sxs-lookup"><span data-stu-id="ab463-183">teleconferenceDeviceAudioQuality</span></span>](teleconferencedeviceaudioquality.md)    | <span data-ttu-id="ab463-184">Dados de qualidade de áudio do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="ab463-184">Video teleconferencing device audio quality data.</span></span>                          |
| [<span data-ttu-id="ab463-185">teleconferenceDeviceVideoQuality</span><span class="sxs-lookup"><span data-stu-id="ab463-185">teleconferenceDeviceVideoQuality</span></span>](teleconferencedevicevideoquality.md)    | <span data-ttu-id="ab463-186">Dados de qualidade de vídeo do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="ab463-186">Video teleconferencing device video quality data.</span></span>                          |
| [<span data-ttu-id="ab463-187">teleconferenceDeviceScreenSharingQuality</span><span class="sxs-lookup"><span data-stu-id="ab463-187">teleconferenceDeviceScreenSharingQuality</span></span>](teleconferencedevicescreensharingquality.md)    | <span data-ttu-id="ab463-188">Dados de qualidade de compartilhamento de tela do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="ab463-188">Video teleconferencing device screen-sharing quality data.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab463-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab463-189">JSON representation</span></span>

<span data-ttu-id="ab463-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab463-190">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality",
  "baseType": null
}-->

```json
{
  "averageInboundJitter": "String (ISO 8601 duration)",
  "averageInboundPacketLossRateInPercentage": 10,
  "averageInboundRoundTripDelay": "String (ISO 8601 duration)",
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
  "description": "teleconferenceDeviceMediaQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
