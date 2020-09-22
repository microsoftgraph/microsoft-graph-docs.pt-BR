---
title: tipo de recurso mediaStream
description: O tipo mediaStream
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0f0181a94743cadf770355d6be349e0d482a387f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071413"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="79219-103">tipo de recurso mediaStream</span><span class="sxs-lookup"><span data-stu-id="79219-103">mediaStream resource type</span></span>

<span data-ttu-id="79219-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="79219-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79219-105">Representa informações sobre um fluxo de mídia entre dois pontos de extremidade em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="79219-105">Represents information about a media stream between two endpoints in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="79219-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79219-106">Properties</span></span>

| <span data-ttu-id="79219-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79219-107">Property</span></span>     | <span data-ttu-id="79219-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="79219-108">Type</span></span>        | <span data-ttu-id="79219-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="79219-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79219-110">averageAudioDegradation</span><span class="sxs-lookup"><span data-stu-id="79219-110">averageAudioDegradation</span></span>|<span data-ttu-id="79219-111">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-111">Double</span></span>|<span data-ttu-id="79219-112">Média da redução da pontuação média de opinião de rede para o Stream.</span><span class="sxs-lookup"><span data-stu-id="79219-112">Average Network Mean Opinion Score degradation for stream.</span></span> <span data-ttu-id="79219-113">Representa o quanto a perda e a tremulação da rede impactaram a qualidade do áudio recebido.</span><span class="sxs-lookup"><span data-stu-id="79219-113">Represents how much the network loss and jitter has impacted the quality of received audio.</span></span>|
|<span data-ttu-id="79219-114">averageAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="79219-114">averageAudioNetworkJitter</span></span>|<span data-ttu-id="79219-115">Duração</span><span class="sxs-lookup"><span data-stu-id="79219-115">Duration</span></span>|<span data-ttu-id="79219-116">Variação média do fluxo calculado conforme especificado em [RFC 3550][], indicado no formato [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="79219-116">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="79219-117">Por exemplo, 1 segundo é indicado como `'PT1S'` , em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.</span><span class="sxs-lookup"><span data-stu-id="79219-117">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="79219-118">averageBandwidthEstimate</span><span class="sxs-lookup"><span data-stu-id="79219-118">averageBandwidthEstimate</span></span>|<span data-ttu-id="79219-119">Int64</span><span class="sxs-lookup"><span data-stu-id="79219-119">Int64</span></span>|<span data-ttu-id="79219-120">Largura de banda estimada média disponível entre dois pontos de extremidade em bits por segundo.</span><span class="sxs-lookup"><span data-stu-id="79219-120">Average estimated bandwidth available between two endpoints in bits per second.</span></span>|
|<span data-ttu-id="79219-121">averageJitter</span><span class="sxs-lookup"><span data-stu-id="79219-121">averageJitter</span></span>|<span data-ttu-id="79219-122">Duração</span><span class="sxs-lookup"><span data-stu-id="79219-122">Duration</span></span>|<span data-ttu-id="79219-123">Variação média do fluxo calculado conforme especificado em [RFC 3550][], indicado no formato [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="79219-123">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="79219-124">Por exemplo, 1 segundo é indicado como `'PT1S'` , em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.</span><span class="sxs-lookup"><span data-stu-id="79219-124">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="79219-125">averagePacketLossRate</span><span class="sxs-lookup"><span data-stu-id="79219-125">averagePacketLossRate</span></span>|<span data-ttu-id="79219-126">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-126">Double</span></span>|<span data-ttu-id="79219-127">Taxa média de perda de pacotes para Stream.</span><span class="sxs-lookup"><span data-stu-id="79219-127">Average packet loss rate for stream.</span></span>|
|<span data-ttu-id="79219-128">averageRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="79219-128">averageRatioOfConcealedSamples</span></span>|<span data-ttu-id="79219-129">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-129">Double</span></span>|<span data-ttu-id="79219-130">Taxa do número de quadros de áudio com amostras geradas por ocultação de perda de pacotes para o número total de quadros de áudio.</span><span class="sxs-lookup"><span data-stu-id="79219-130">Ratio of the number of audio frames with samples generated by packet loss concealment to the total number of audio frames.</span></span>|
|<span data-ttu-id="79219-131">averageReceivedFrameRate</span><span class="sxs-lookup"><span data-stu-id="79219-131">averageReceivedFrameRate</span></span>|<span data-ttu-id="79219-132">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-132">Double</span></span>|<span data-ttu-id="79219-133">Média de quadros por segundo recebidos para todos os fluxos de vídeo calculados durante a sessão.</span><span class="sxs-lookup"><span data-stu-id="79219-133">Average frames per second received for all video streams computed over the duration of the session.</span></span>|
|<span data-ttu-id="79219-134">averageRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="79219-134">averageRoundTripTime</span></span>|<span data-ttu-id="79219-135">Duração</span><span class="sxs-lookup"><span data-stu-id="79219-135">Duration</span></span>|<span data-ttu-id="79219-136">Tempo médio de ida e volta da propagação de rede calculado conforme especificado na [RFC 3550][], indicado no formato [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="79219-136">Average network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="79219-137">Por exemplo, 1 segundo é indicado como `'PT1S'` , em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.</span><span class="sxs-lookup"><span data-stu-id="79219-137">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="79219-138">averageVideoFrameLossPercentage</span><span class="sxs-lookup"><span data-stu-id="79219-138">averageVideoFrameLossPercentage</span></span>|<span data-ttu-id="79219-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-139">Double</span></span>|<span data-ttu-id="79219-140">Porcentagem média de quadros de vídeo perdidos, conforme exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="79219-140">Average percentage of video frames lost as displayed to the user.</span></span>|
|<span data-ttu-id="79219-141">averageVideoFrameRate</span><span class="sxs-lookup"><span data-stu-id="79219-141">averageVideoFrameRate</span></span>|<span data-ttu-id="79219-142">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-142">Double</span></span>|<span data-ttu-id="79219-143">Média de quadros por segundo recebidos para um fluxo de vídeo, calculado sobre a duração da sessão.</span><span class="sxs-lookup"><span data-stu-id="79219-143">Average frames per second received for a video stream, computed over the duration of the session.</span></span>|
|<span data-ttu-id="79219-144">averageVideoPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="79219-144">averageVideoPacketLossRate</span></span>|<span data-ttu-id="79219-145">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-145">Double</span></span>|<span data-ttu-id="79219-146">Fração média de pacotes perdidos, conforme especificado em [RFC 3550][], calculado durante a sessão.</span><span class="sxs-lookup"><span data-stu-id="79219-146">Average fraction of packets lost, as specified in [RFC 3550][], computed over the duration of the session.</span></span>|
|<span data-ttu-id="79219-147">endDateTime</span><span class="sxs-lookup"><span data-stu-id="79219-147">endDateTime</span></span>|<span data-ttu-id="79219-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79219-148">DateTimeOffset</span></span>|<span data-ttu-id="79219-149">Hora UTC em que o Stream terminou.</span><span class="sxs-lookup"><span data-stu-id="79219-149">UTC time when the stream ended.</span></span> <span data-ttu-id="79219-150">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="79219-150">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="79219-151">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="79219-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="79219-152">lowFrameRateRatio</span><span class="sxs-lookup"><span data-stu-id="79219-152">lowFrameRateRatio</span></span>|<span data-ttu-id="79219-153">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-153">Double</span></span>|<span data-ttu-id="79219-154">Fração da chamada em que a taxa de quadros é menor que 7,5 quadros por segundo.</span><span class="sxs-lookup"><span data-stu-id="79219-154">Fraction of the call where frame rate is less than 7.5 frames per second.</span></span>|
|<span data-ttu-id="79219-155">lowVideoProcessingCapabilityRatio</span><span class="sxs-lookup"><span data-stu-id="79219-155">lowVideoProcessingCapabilityRatio</span></span>|<span data-ttu-id="79219-156">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-156">Double</span></span>|<span data-ttu-id="79219-157">Fração da chamada em que o cliente está executando menos de 70% da capacidade de processamento de vídeo esperada.</span><span class="sxs-lookup"><span data-stu-id="79219-157">Fraction of the call that the client is running less than 70% expected video processing capability.</span></span>|
|<span data-ttu-id="79219-158">maxAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="79219-158">maxAudioNetworkJitter</span></span>|<span data-ttu-id="79219-159">Duração</span><span class="sxs-lookup"><span data-stu-id="79219-159">Duration</span></span>|<span data-ttu-id="79219-160">Máximo de tremulação de rede de áudio calculada sobre cada uma das 20 segundos janelas durante a sessão, indicada no formato [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="79219-160">Maximum of audio network jitter computed over each of the 20 second windows during the session, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="79219-161">Por exemplo, 1 segundo é indicado como `'PT1S'` , em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.</span><span class="sxs-lookup"><span data-stu-id="79219-161">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="79219-162">maxJitter</span><span class="sxs-lookup"><span data-stu-id="79219-162">maxJitter</span></span>|<span data-ttu-id="79219-163">Duração</span><span class="sxs-lookup"><span data-stu-id="79219-163">Duration</span></span>|<span data-ttu-id="79219-164">Variação máxima do Stream computada conforme especificado em RFC 3550, indicado no formato [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="79219-164">Maximum jitter for the stream computed as specified in RFC 3550, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="79219-165">Por exemplo, 1 segundo é indicado como `'PT1S'` , em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.</span><span class="sxs-lookup"><span data-stu-id="79219-165">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="79219-166">maxPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="79219-166">maxPacketLossRate</span></span>|<span data-ttu-id="79219-167">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-167">Double</span></span>|<span data-ttu-id="79219-168">Taxa máxima de perda de pacotes para o fluxo.</span><span class="sxs-lookup"><span data-stu-id="79219-168">Maximum packet loss rate for the stream.</span></span>|
|<span data-ttu-id="79219-169">maxRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="79219-169">maxRatioOfConcealedSamples</span></span>|<span data-ttu-id="79219-170">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-170">Double</span></span>|<span data-ttu-id="79219-171">Taxa máxima de pacotes ocultos pelo reparo.</span><span class="sxs-lookup"><span data-stu-id="79219-171">Maximum ratio of packets concealed by the healer.</span></span>|
|<span data-ttu-id="79219-172">maxRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="79219-172">maxRoundTripTime</span></span>|<span data-ttu-id="79219-173">Duração</span><span class="sxs-lookup"><span data-stu-id="79219-173">Duration</span></span>|<span data-ttu-id="79219-174">Tempo máximo de ida e volta da propagação de rede calculado conforme especificado na [RFC 3550][], indicado no formato [ISO 8601][] .</span><span class="sxs-lookup"><span data-stu-id="79219-174">Maximum network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="79219-175">Por exemplo, 1 segundo é indicado como `'PT1S'` , em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.</span><span class="sxs-lookup"><span data-stu-id="79219-175">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="79219-176">packetUtilization</span><span class="sxs-lookup"><span data-stu-id="79219-176">packetUtilization</span></span>|<span data-ttu-id="79219-177">Int64</span><span class="sxs-lookup"><span data-stu-id="79219-177">Int64</span></span>|<span data-ttu-id="79219-178">Contagem de pacotes para o Stream.</span><span class="sxs-lookup"><span data-stu-id="79219-178">Packet count for the stream.</span></span>|
|<span data-ttu-id="79219-179">postForwardErrorCorrectionPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="79219-179">postForwardErrorCorrectionPacketLossRate</span></span>|<span data-ttu-id="79219-180">Duplo</span><span class="sxs-lookup"><span data-stu-id="79219-180">Double</span></span>|<span data-ttu-id="79219-181">Taxa de perda de pacotes após o FEC ter sido aplicado em todos os fluxos de vídeo e codecs.</span><span class="sxs-lookup"><span data-stu-id="79219-181">Packet loss rate after FEC has been applied aggregated across all video streams and codecs.</span></span>|
|<span data-ttu-id="79219-182">startDateTime</span><span class="sxs-lookup"><span data-stu-id="79219-182">startDateTime</span></span>|<span data-ttu-id="79219-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79219-183">DateTimeOffset</span></span>|<span data-ttu-id="79219-184">Hora UTC quando o fluxo é iniciado.</span><span class="sxs-lookup"><span data-stu-id="79219-184">UTC time when the stream started.</span></span> <span data-ttu-id="79219-185">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="79219-185">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="79219-186">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="79219-186">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="79219-187">streamDirection</span><span class="sxs-lookup"><span data-stu-id="79219-187">streamDirection</span></span>|<span data-ttu-id="79219-188">Microsoft. Graph. callRecords. mediaStreamDirection</span><span class="sxs-lookup"><span data-stu-id="79219-188">microsoft.graph.callRecords.mediaStreamDirection</span></span>|<span data-ttu-id="79219-189">Indica a direção do fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="79219-189">Indicates the direction of the media stream.</span></span> <span data-ttu-id="79219-190">Os valores possíveis são: `callerToCallee` e `calleeToCaller`.</span><span class="sxs-lookup"><span data-stu-id="79219-190">Possible values are: `callerToCallee`, `calleeToCaller`.</span></span>|
|<span data-ttu-id="79219-191">streamid</span><span class="sxs-lookup"><span data-stu-id="79219-191">streamId</span></span>|<span data-ttu-id="79219-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79219-192">String</span></span>|<span data-ttu-id="79219-193">Identificador exclusivo do Stream.</span><span class="sxs-lookup"><span data-stu-id="79219-193">Unique identifier for the stream.</span></span>|
|<span data-ttu-id="79219-194">wasMediaBypassed</span><span class="sxs-lookup"><span data-stu-id="79219-194">wasMediaBypassed</span></span>|<span data-ttu-id="79219-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="79219-195">Boolean</span></span>|<span data-ttu-id="79219-196">True se o fluxo de mídia ignorar o servidor de mediação e passou diretamente entre o cliente e gateway PSTN/PBX; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="79219-196">True if the media stream bypassed the Mediation Server and went straight between client and PSTN Gateway/PBX, false otherwise.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="79219-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79219-197">JSON representation</span></span>

<span data-ttu-id="79219-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79219-198">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.mediaStream",
  "baseType": null
}-->

```json
{
  "averageAudioDegradation": "Double",
  "averageAudioNetworkJitter": "String (duration)",
  "averageBandwidthEstimate": 1024,
  "averageJitter": "String (duration)",
  "averagePacketLossRate": "Double",
  "averageRatioOfConcealedSamples": "Double",
  "averageReceivedFrameRate": "Double",
  "averageRoundTripTime": "String (duration)",
  "averageVideoFrameLossPercentage": "Double",
  "averageVideoFrameRate": "Double",
  "averageVideoPacketLossRate": "Double",
  "endDateTime": "String (timestamp)",
  "lowFrameRateRatio": "Double",
  "lowVideoProcessingCapabilityRatio": "Double",
  "maxAudioNetworkJitter": "String (duration)",
  "maxJitter": "String (duration)",
  "maxPacketLossRate": "Double",
  "maxRatioOfConcealedSamples": "Double",
  "maxRoundTripTime": "String (duration)",
  "packetUtilization": 1024,
  "postForwardErrorCorrectionPacketLossRate": "Double",
  "startDateTime": "String (timestamp)",
  "streamDirection": "String",
  "streamId": "String",
  "wasMediaBypassed": true
}
```

[ISO 8601]: https://www.iso.org/iso/iso8601
[RFC 3550]: https://tools.ietf.org/html/rfc3550

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

