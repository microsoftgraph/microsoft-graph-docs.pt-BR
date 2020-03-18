---
title: tipo de recurso teleconferenceDeviceMediaQuality
description: Dados de qualidade de mídia do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ab703760246fe08145924fd5d21ce4d02a5090b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763297"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a><span data-ttu-id="c8c80-103">tipo de recurso teleconferenceDeviceMediaQuality</span><span class="sxs-lookup"><span data-stu-id="c8c80-103">teleconferenceDeviceMediaQuality resource type</span></span>

<span data-ttu-id="c8c80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8c80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8c80-105">Representa dados de qualidade de mídia do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="c8c80-105">Represents video teleconferencing device media quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="c8c80-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8c80-106">Properties</span></span>

| <span data-ttu-id="c8c80-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8c80-107">Property</span></span>     | <span data-ttu-id="c8c80-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8c80-108">Type</span></span>        | <span data-ttu-id="c8c80-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8c80-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c8c80-110">averageInboundJitter</span><span class="sxs-lookup"><span data-stu-id="c8c80-110">averageInboundJitter</span></span>|<span data-ttu-id="c8c80-111">Duração</span><span class="sxs-lookup"><span data-stu-id="c8c80-111">Duration</span></span>|<span data-ttu-id="c8c80-112">A tremulação média da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="c8c80-112">The average inbound stream network jitter.</span></span>|
|<span data-ttu-id="c8c80-113">averageInboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="c8c80-113">averageInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="c8c80-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="c8c80-114">Double</span></span>|<span data-ttu-id="c8c80-115">A taxa média de perda de pacote de fluxo de entrada em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="c8c80-115">The average inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="c8c80-116">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="c8c80-116">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="c8c80-117">averageInboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="c8c80-117">averageInboundRoundTripDelay</span></span>|<span data-ttu-id="c8c80-118">Duração</span><span class="sxs-lookup"><span data-stu-id="c8c80-118">Duration</span></span>|<span data-ttu-id="c8c80-119">O intervalo médio de ida e volta da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="c8c80-119">The average inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="c8c80-120">averageOutboundJitter</span><span class="sxs-lookup"><span data-stu-id="c8c80-120">averageOutboundJitter</span></span>|<span data-ttu-id="c8c80-121">Duração</span><span class="sxs-lookup"><span data-stu-id="c8c80-121">Duration</span></span>|<span data-ttu-id="c8c80-122">A tremulação média da rede de fluxo de saída.</span><span class="sxs-lookup"><span data-stu-id="c8c80-122">The average outbound stream network jitter.</span></span>|
|<span data-ttu-id="c8c80-123">averageOutboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="c8c80-123">averageOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="c8c80-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="c8c80-124">Double</span></span>|<span data-ttu-id="c8c80-125">A taxa média de perda de pacotes de fluxo de saída em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="c8c80-125">The average outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="c8c80-126">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="c8c80-126">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="c8c80-127">averageOutboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="c8c80-127">averageOutboundRoundTripDelay</span></span>|<span data-ttu-id="c8c80-128">Duração</span><span class="sxs-lookup"><span data-stu-id="c8c80-128">Duration</span></span>|<span data-ttu-id="c8c80-129">O intervalo médio de ida e volta da rede de fluxo de saída.</span><span class="sxs-lookup"><span data-stu-id="c8c80-129">The average outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="c8c80-130">channelIndex</span><span class="sxs-lookup"><span data-stu-id="c8c80-130">channelIndex</span></span>|<span data-ttu-id="c8c80-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c8c80-131">Int32</span></span>|<span data-ttu-id="c8c80-132">O índice de canal da mídia.</span><span class="sxs-lookup"><span data-stu-id="c8c80-132">The channel index of media.</span></span> <span data-ttu-id="c8c80-133">A indexação começa com 1.</span><span class="sxs-lookup"><span data-stu-id="c8c80-133">Indexing begins with 1.</span></span>  <span data-ttu-id="c8c80-134">Se uma sessão de mídia contiver três modalidades de vídeo, os índices de canal serão 1, 2 e 3.</span><span class="sxs-lookup"><span data-stu-id="c8c80-134">If a media session contains 3 video modalities, channel indexes will be 1, 2, and 3.</span></span>|
|<span data-ttu-id="c8c80-135">inboundPackets</span><span class="sxs-lookup"><span data-stu-id="c8c80-135">inboundPackets</span></span>|<span data-ttu-id="c8c80-136">Int64</span><span class="sxs-lookup"><span data-stu-id="c8c80-136">Int64</span></span>|<span data-ttu-id="c8c80-137">O número total de pacotes de entrada.</span><span class="sxs-lookup"><span data-stu-id="c8c80-137">The total number of the inbound packets.</span></span>|
|<span data-ttu-id="c8c80-138">localIPAddress</span><span class="sxs-lookup"><span data-stu-id="c8c80-138">localIPAddress</span></span>|<span data-ttu-id="c8c80-139">String</span><span class="sxs-lookup"><span data-stu-id="c8c80-139">String</span></span>|<span data-ttu-id="c8c80-140">o endereço IP local da sessão de mídia.</span><span class="sxs-lookup"><span data-stu-id="c8c80-140">the local IP address for the media session.</span></span>|
|<span data-ttu-id="c8c80-141">localPort</span><span class="sxs-lookup"><span data-stu-id="c8c80-141">localPort</span></span>|<span data-ttu-id="c8c80-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c8c80-142">Int32</span></span>|<span data-ttu-id="c8c80-143">A porta de mídia local.</span><span class="sxs-lookup"><span data-stu-id="c8c80-143">The local media port.</span></span>|
|<span data-ttu-id="c8c80-144">maximumInboundJitter</span><span class="sxs-lookup"><span data-stu-id="c8c80-144">maximumInboundJitter</span></span>|<span data-ttu-id="c8c80-145">Duração</span><span class="sxs-lookup"><span data-stu-id="c8c80-145">Duration</span></span>|<span data-ttu-id="c8c80-146">A tremulação máxima da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="c8c80-146">The maximum inbound stream network jitter.</span></span>|
|<span data-ttu-id="c8c80-147">maximumInboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="c8c80-147">maximumInboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="c8c80-148">Duplo</span><span class="sxs-lookup"><span data-stu-id="c8c80-148">Double</span></span>|<span data-ttu-id="c8c80-149">A taxa máxima de perda de pacote de fluxo de entrada em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="c8c80-149">The maximum inbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="c8c80-150">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="c8c80-150">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="c8c80-151">maximumInboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="c8c80-151">maximumInboundRoundTripDelay</span></span>|<span data-ttu-id="c8c80-152">Duração</span><span class="sxs-lookup"><span data-stu-id="c8c80-152">Duration</span></span>|<span data-ttu-id="c8c80-153">O intervalo máximo de ida e volta da rede de fluxo de entrada.</span><span class="sxs-lookup"><span data-stu-id="c8c80-153">The maximum inbound stream network round trip delay.</span></span>|
|<span data-ttu-id="c8c80-154">maximumOutboundJitter</span><span class="sxs-lookup"><span data-stu-id="c8c80-154">maximumOutboundJitter</span></span>|<span data-ttu-id="c8c80-155">Duração</span><span class="sxs-lookup"><span data-stu-id="c8c80-155">Duration</span></span>|<span data-ttu-id="c8c80-156">A tremulação de rede de fluxo de saída máximo.</span><span class="sxs-lookup"><span data-stu-id="c8c80-156">The maximum outbound stream network jitter.</span></span>|
|<span data-ttu-id="c8c80-157">maximumOutboundPacketLossRateInPercentage</span><span class="sxs-lookup"><span data-stu-id="c8c80-157">maximumOutboundPacketLossRateInPercentage</span></span>|<span data-ttu-id="c8c80-158">Duplo</span><span class="sxs-lookup"><span data-stu-id="c8c80-158">Double</span></span>|<span data-ttu-id="c8c80-159">A taxa máxima de perda de pacotes de fluxo de saída em porcentagem (0-100).</span><span class="sxs-lookup"><span data-stu-id="c8c80-159">The maximum outbound stream packet loss rate in percentage (0-100).</span></span> <span data-ttu-id="c8c80-160">Por exemplo, 0, 1 significa 0, 1%.</span><span class="sxs-lookup"><span data-stu-id="c8c80-160">For example, 0.01 means 0.01%.</span></span>|
|<span data-ttu-id="c8c80-161">maximumOutboundRoundTripDelay</span><span class="sxs-lookup"><span data-stu-id="c8c80-161">maximumOutboundRoundTripDelay</span></span>|<span data-ttu-id="c8c80-162">Duração</span><span class="sxs-lookup"><span data-stu-id="c8c80-162">Duration</span></span>|<span data-ttu-id="c8c80-163">O atraso máximo de ida e volta da rede de fluxo de saída.</span><span class="sxs-lookup"><span data-stu-id="c8c80-163">The maximum outbound stream network round trip delay.</span></span>|
|<span data-ttu-id="c8c80-164">mediaDuration</span><span class="sxs-lookup"><span data-stu-id="c8c80-164">mediaDuration</span></span>|<span data-ttu-id="c8c80-165">Duração</span><span class="sxs-lookup"><span data-stu-id="c8c80-165">Duration</span></span>|<span data-ttu-id="c8c80-166">A duração da modalidade total.</span><span class="sxs-lookup"><span data-stu-id="c8c80-166">The total modality duration.</span></span> <span data-ttu-id="c8c80-167">Se a mídia habilitada e desabilitada várias vezes, MediaDuration será a soma de todas as durações.</span><span class="sxs-lookup"><span data-stu-id="c8c80-167">If the media enabled and disabled multiple times, MediaDuration will the summation of all of the durations.</span></span>|
|<span data-ttu-id="c8c80-168">networkLinkSpeedInBytes</span><span class="sxs-lookup"><span data-stu-id="c8c80-168">networkLinkSpeedInBytes</span></span>|<span data-ttu-id="c8c80-169">Int64</span><span class="sxs-lookup"><span data-stu-id="c8c80-169">Int64</span></span>|<span data-ttu-id="c8c80-170">A velocidade do link de rede em bytes</span><span class="sxs-lookup"><span data-stu-id="c8c80-170">The network link speed in bytes</span></span>|
|<span data-ttu-id="c8c80-171">outboundPackets</span><span class="sxs-lookup"><span data-stu-id="c8c80-171">outboundPackets</span></span>|<span data-ttu-id="c8c80-172">Int64</span><span class="sxs-lookup"><span data-stu-id="c8c80-172">Int64</span></span>|<span data-ttu-id="c8c80-173">O número total dos pacotes de saída.</span><span class="sxs-lookup"><span data-stu-id="c8c80-173">The total number of the outbound packets.</span></span>|
|<span data-ttu-id="c8c80-174">remoteIPAddress</span><span class="sxs-lookup"><span data-stu-id="c8c80-174">remoteIPAddress</span></span>|<span data-ttu-id="c8c80-175">String</span><span class="sxs-lookup"><span data-stu-id="c8c80-175">String</span></span>|<span data-ttu-id="c8c80-176">O endereço IP remoto da sessão de mídia.</span><span class="sxs-lookup"><span data-stu-id="c8c80-176">The remote IP address for the media session.</span></span>|
|<span data-ttu-id="c8c80-177">remotePort</span><span class="sxs-lookup"><span data-stu-id="c8c80-177">remotePort</span></span>|<span data-ttu-id="c8c80-178">Int32</span><span class="sxs-lookup"><span data-stu-id="c8c80-178">Int32</span></span>|<span data-ttu-id="c8c80-179">A porta de mídia remota.</span><span class="sxs-lookup"><span data-stu-id="c8c80-179">The remote media port.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8c80-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8c80-180">JSON representation</span></span>

<span data-ttu-id="c8c80-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8c80-181">The following is a JSON representation of the resource.</span></span>

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
