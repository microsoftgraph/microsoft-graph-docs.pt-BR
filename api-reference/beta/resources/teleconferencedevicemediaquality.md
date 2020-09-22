---
title: tipo de recurso teleconferenceDeviceMediaQuality
description: Dados de qualidade de mídia do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a01dd135c85288fd511975cce8781912f2975f4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046305"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a><span data-ttu-id="1d5f0-103">tipo de recurso teleconferenceDeviceMediaQuality</span><span class="sxs-lookup"><span data-stu-id="1d5f0-103">teleconferenceDeviceMediaQuality resource type</span></span>

<span data-ttu-id="1d5f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d5f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d5f0-105">Representa dados de qualidade de mídia do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-105">Represents video teleconferencing device media quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="1d5f0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d5f0-106">Properties</span></span>

| <span data-ttu-id="1d5f0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d5f0-107">Property</span></span>     | <span data-ttu-id="1d5f0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d5f0-108">Type</span></span>        | <span data-ttu-id="1d5f0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d5f0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d5f0-110">averageInboundJitter</span><span class="sxs-lookup"><span data-stu-id="1d5f0-110">averageInboundJitter</span></span>|<span data-ttu-id="1d5f0-111">Duração</span><span class="sxs-lookup"><span data-stu-id="1d5f0-111">Duration</span></span>|<span data-ttu-id="1d5f0-112">A tremulação média da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-112">The average inbound stream network jitter.</span></span>|
|<span data-ttu-id="1d5f0-113">averageInboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="1d5f0-113">averageInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="1d5f0-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="1d5f0-114">Double</span></span>|<span data-ttu-id="1d5f0-115">A taxa média de perda de pacote de fluxo de entrada em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="1d5f0-115">The average inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="1d5f0-116">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-116">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="1d5f0-117">averageInboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="1d5f0-117">averageInboundRoundTripDelay</span></span>|<span data-ttu-id="1d5f0-118">Duração</span><span class="sxs-lookup"><span data-stu-id="1d5f0-118">Duration</span></span>|<span data-ttu-id="1d5f0-119">O intervalo médio de ida e volta da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-119">The average inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="1d5f0-120">averageOutboundJitter</span><span class="sxs-lookup"><span data-stu-id="1d5f0-120">averageOutboundJitter</span></span>|<span data-ttu-id="1d5f0-121">Duração</span><span class="sxs-lookup"><span data-stu-id="1d5f0-121">Duration</span></span>|<span data-ttu-id="1d5f0-122">A tremulação média da rede de fluxo de saída.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-122">The average outbound stream network jitter.</span></span>|
|<span data-ttu-id="1d5f0-123">averageOutboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="1d5f0-123">averageOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="1d5f0-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="1d5f0-124">Double</span></span>|<span data-ttu-id="1d5f0-125">A taxa média de perda de pacotes de fluxo de saída em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="1d5f0-125">The average outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="1d5f0-126">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-126">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="1d5f0-127">averageOutboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="1d5f0-127">averageOutboundRoundTripDelay</span></span>|<span data-ttu-id="1d5f0-128">Duração</span><span class="sxs-lookup"><span data-stu-id="1d5f0-128">Duration</span></span>|<span data-ttu-id="1d5f0-129">O intervalo médio de ida e volta da rede de fluxo de saída.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-129">The average outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="1d5f0-130">channelIndex</span><span class="sxs-lookup"><span data-stu-id="1d5f0-130">channelIndex</span></span>|<span data-ttu-id="1d5f0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="1d5f0-131">Int32</span></span>|<span data-ttu-id="1d5f0-132">O índice de canal da mídia.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-132">The channel index of media.</span></span> <span data-ttu-id="1d5f0-133">A indexação começa com 1.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-133">Indexing begins with 1.</span></span>  <span data-ttu-id="1d5f0-134">Se uma sessão de mídia contiver três modalidades de vídeo, os índices de canal serão 1, 2 e 3.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-134">If a media session contains 3 video modalities, channel indexes will be 1, 2, and 3.</span></span>|
|<span data-ttu-id="1d5f0-135">inboundPackets</span><span class="sxs-lookup"><span data-stu-id="1d5f0-135">inboundPackets</span></span>|<span data-ttu-id="1d5f0-136">Int64</span><span class="sxs-lookup"><span data-stu-id="1d5f0-136">Int64</span></span>|<span data-ttu-id="1d5f0-137">O número total de pacotes de entrada.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-137">The total number of the inbound packets.</span></span>|
|<span data-ttu-id="1d5f0-138">localIPAddress</span><span class="sxs-lookup"><span data-stu-id="1d5f0-138">localIPAddress</span></span>|<span data-ttu-id="1d5f0-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d5f0-139">String</span></span>|<span data-ttu-id="1d5f0-140">o endereço IP local da sessão de mídia.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-140">the local IP address for the media session.</span></span>|
|<span data-ttu-id="1d5f0-141">localPort</span><span class="sxs-lookup"><span data-stu-id="1d5f0-141">localPort</span></span>|<span data-ttu-id="1d5f0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1d5f0-142">Int32</span></span>|<span data-ttu-id="1d5f0-143">A porta de mídia local.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-143">The local media port.</span></span>|
|<span data-ttu-id="1d5f0-144">maximumInboundJitter</span><span class="sxs-lookup"><span data-stu-id="1d5f0-144">maximumInboundJitter</span></span>|<span data-ttu-id="1d5f0-145">Duração</span><span class="sxs-lookup"><span data-stu-id="1d5f0-145">Duration</span></span>|<span data-ttu-id="1d5f0-146">A tremulação máxima da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-146">The maximum inbound stream network jitter.</span></span>|
|<span data-ttu-id="1d5f0-147">maximumInboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="1d5f0-147">maximumInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="1d5f0-148">Duplo</span><span class="sxs-lookup"><span data-stu-id="1d5f0-148">Double</span></span>|<span data-ttu-id="1d5f0-149">A taxa máxima de perda de pacote de fluxo de entrada em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="1d5f0-149">The maximum inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="1d5f0-150">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-150">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="1d5f0-151">maximumInboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="1d5f0-151">maximumInboundRoundTripDelay</span></span>|<span data-ttu-id="1d5f0-152">Duração</span><span class="sxs-lookup"><span data-stu-id="1d5f0-152">Duration</span></span>|<span data-ttu-id="1d5f0-153">O intervalo máximo de ida e volta da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-153">The maximum inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="1d5f0-154">maximumOutboundJitter</span><span class="sxs-lookup"><span data-stu-id="1d5f0-154">maximumOutboundJitter</span></span>|<span data-ttu-id="1d5f0-155">Duração</span><span class="sxs-lookup"><span data-stu-id="1d5f0-155">Duration</span></span>|<span data-ttu-id="1d5f0-156">A tremulação de rede de fluxo de saída máximo.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-156">The maximum outbound stream network jitter.</span></span>|
|<span data-ttu-id="1d5f0-157">maximumOutboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="1d5f0-157">maximumOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="1d5f0-158">Duplo</span><span class="sxs-lookup"><span data-stu-id="1d5f0-158">Double</span></span>|<span data-ttu-id="1d5f0-159">A taxa máxima de perda de pacotes de fluxo de saída em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="1d5f0-159">The maximum outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="1d5f0-160">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-160">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="1d5f0-161">maximumOutboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="1d5f0-161">maximumOutboundRoundTripDelay</span></span>|<span data-ttu-id="1d5f0-162">Duração</span><span class="sxs-lookup"><span data-stu-id="1d5f0-162">Duration</span></span>|<span data-ttu-id="1d5f0-163">O atraso máximo de ida e volta da rede de fluxo de saída.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-163">The maximum outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="1d5f0-164">mediaDuration</span><span class="sxs-lookup"><span data-stu-id="1d5f0-164">mediaDuration</span></span>|<span data-ttu-id="1d5f0-165">Duração</span><span class="sxs-lookup"><span data-stu-id="1d5f0-165">Duration</span></span>|<span data-ttu-id="1d5f0-166">A duração da modalidade total.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-166">The total modality duration.</span></span> <span data-ttu-id="1d5f0-167">Se a mídia habilitada e desabilitada várias vezes, MediaDuration será a soma de todas as durações.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-167">If the media enabled and disabled multiple times, MediaDuration will the summation of all of the durations.</span></span>|
|<span data-ttu-id="1d5f0-168">networkLinkSpeedInBytes</span><span class="sxs-lookup"><span data-stu-id="1d5f0-168">networkLinkSpeedInBytes</span></span>|<span data-ttu-id="1d5f0-169">Int64</span><span class="sxs-lookup"><span data-stu-id="1d5f0-169">Int64</span></span>|<span data-ttu-id="1d5f0-170">A velocidade do link de rede em bytes</span><span class="sxs-lookup"><span data-stu-id="1d5f0-170">The network link speed in bytes</span></span>|
|<span data-ttu-id="1d5f0-171">outboundPackets</span><span class="sxs-lookup"><span data-stu-id="1d5f0-171">outboundPackets</span></span>|<span data-ttu-id="1d5f0-172">Int64</span><span class="sxs-lookup"><span data-stu-id="1d5f0-172">Int64</span></span>|<span data-ttu-id="1d5f0-173">O número total dos pacotes de saída.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-173">The total number of the outbound packets.</span></span>|
|<span data-ttu-id="1d5f0-174">remoteIPAddress</span><span class="sxs-lookup"><span data-stu-id="1d5f0-174">remoteIPAddress</span></span>|<span data-ttu-id="1d5f0-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d5f0-175">String</span></span>|<span data-ttu-id="1d5f0-176">O endereço IP remoto da sessão de mídia.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-176">The remote IP address for the media session.</span></span>|
|<span data-ttu-id="1d5f0-177">remotePort</span><span class="sxs-lookup"><span data-stu-id="1d5f0-177">remotePort</span></span>|<span data-ttu-id="1d5f0-178">Int32</span><span class="sxs-lookup"><span data-stu-id="1d5f0-178">Int32</span></span>|<span data-ttu-id="1d5f0-179">A porta de mídia remota.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-179">The remote media port.</span></span>|

### <a name="derived-types"></a><span data-ttu-id="1d5f0-180">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="1d5f0-180">Derived types</span></span>

| <span data-ttu-id="1d5f0-181">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d5f0-181">Type</span></span>                                                 | <span data-ttu-id="1d5f0-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d5f0-182">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="1d5f0-183">teleconferenceDeviceAudioQuality</span><span class="sxs-lookup"><span data-stu-id="1d5f0-183">teleconferenceDeviceAudioQuality</span></span>](teleconferencedeviceaudioquality.md)    | <span data-ttu-id="1d5f0-184">Dados de qualidade de áudio do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-184">Video teleconferencing device audio quality data.</span></span>                          |
| [<span data-ttu-id="1d5f0-185">teleconferenceDeviceVideoQuality</span><span class="sxs-lookup"><span data-stu-id="1d5f0-185">teleconferenceDeviceVideoQuality</span></span>](teleconferencedevicevideoquality.md)    | <span data-ttu-id="1d5f0-186">Dados de qualidade de vídeo do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-186">Video teleconferencing device video quality data.</span></span>                          |
| [<span data-ttu-id="1d5f0-187">teleconferenceDeviceScreenSharingQuality</span><span class="sxs-lookup"><span data-stu-id="1d5f0-187">teleconferenceDeviceScreenSharingQuality</span></span>](teleconferencedevicescreensharingquality.md)    | <span data-ttu-id="1d5f0-188">Dados de qualidade de compartilhamento de tela do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-188">Video teleconferencing device screen-sharing quality data.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1d5f0-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d5f0-189">JSON representation</span></span>

<span data-ttu-id="1d5f0-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d5f0-190">The following is a JSON representation of the resource.</span></span>

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


