---
title: Tipo de recurso mediaStream
description: O tipo mediaStream
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 69555033ddacc9244c910b5094449ca60d1a9633
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720246"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="86025-103">Tipo de recurso mediaStream</span><span class="sxs-lookup"><span data-stu-id="86025-103">mediaStream resource type</span></span>

<span data-ttu-id="86025-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="86025-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86025-105">Representa informações sobre um fluxo de mídia entre dois pontos de extremidade em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="86025-105">Represents information about a media stream between two endpoints in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="86025-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86025-106">Properties</span></span>

| <span data-ttu-id="86025-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86025-107">Property</span></span>     | <span data-ttu-id="86025-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="86025-108">Type</span></span>        | <span data-ttu-id="86025-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="86025-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86025-110">averageAudioDegradation</span><span class="sxs-lookup"><span data-stu-id="86025-110">averageAudioDegradation</span></span>|<span data-ttu-id="86025-111">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-111">Double</span></span>|<span data-ttu-id="86025-112">Degradação média de pontuação de opinião de rede para fluxo.</span><span class="sxs-lookup"><span data-stu-id="86025-112">Average Network Mean Opinion Score degradation for stream.</span></span> <span data-ttu-id="86025-113">Representa o quanto a perda de rede e a tremedeira afetaram a qualidade do áudio recebido.</span><span class="sxs-lookup"><span data-stu-id="86025-113">Represents how much the network loss and jitter has impacted the quality of received audio.</span></span>|
|<span data-ttu-id="86025-114">averageAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="86025-114">averageAudioNetworkJitter</span></span>|<span data-ttu-id="86025-115">Duration</span><span class="sxs-lookup"><span data-stu-id="86025-115">Duration</span></span>|<span data-ttu-id="86025-116">Tremido médio para o fluxo calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="86025-116">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="86025-117">Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.</span><span class="sxs-lookup"><span data-stu-id="86025-117">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="86025-118">averageBandwidthEstimate</span><span class="sxs-lookup"><span data-stu-id="86025-118">averageBandwidthEstimate</span></span>|<span data-ttu-id="86025-119">Int64</span><span class="sxs-lookup"><span data-stu-id="86025-119">Int64</span></span>|<span data-ttu-id="86025-120">Largura de banda estimada média disponível entre dois pontos de extremidade em bits por segundo.</span><span class="sxs-lookup"><span data-stu-id="86025-120">Average estimated bandwidth available between two endpoints in bits per second.</span></span>|
|<span data-ttu-id="86025-121">averageJitter</span><span class="sxs-lookup"><span data-stu-id="86025-121">averageJitter</span></span>|<span data-ttu-id="86025-122">Duration</span><span class="sxs-lookup"><span data-stu-id="86025-122">Duration</span></span>|<span data-ttu-id="86025-123">Tremido médio para o fluxo calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="86025-123">Average jitter for the stream computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="86025-124">Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.</span><span class="sxs-lookup"><span data-stu-id="86025-124">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="86025-125">averagePacketLossRate</span><span class="sxs-lookup"><span data-stu-id="86025-125">averagePacketLossRate</span></span>|<span data-ttu-id="86025-126">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-126">Double</span></span>|<span data-ttu-id="86025-127">Taxa média de perda de pacotes para fluxo.</span><span class="sxs-lookup"><span data-stu-id="86025-127">Average packet loss rate for stream.</span></span>|
|<span data-ttu-id="86025-128">averageRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="86025-128">averageRatioOfConcealedSamples</span></span>|<span data-ttu-id="86025-129">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-129">Double</span></span>|<span data-ttu-id="86025-130">Taxa do número de quadros de áudio com exemplos gerados pela ocultação de perda de pacotes para o número total de quadros de áudio.</span><span class="sxs-lookup"><span data-stu-id="86025-130">Ratio of the number of audio frames with samples generated by packet loss concealment to the total number of audio frames.</span></span>|
|<span data-ttu-id="86025-131">averageReceivedFrameRate</span><span class="sxs-lookup"><span data-stu-id="86025-131">averageReceivedFrameRate</span></span>|<span data-ttu-id="86025-132">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-132">Double</span></span>|<span data-ttu-id="86025-133">Média de quadros por segundo recebidos para todos os fluxos de vídeo calculados durante a sessão.</span><span class="sxs-lookup"><span data-stu-id="86025-133">Average frames per second received for all video streams computed over the duration of the session.</span></span>|
|<span data-ttu-id="86025-134">averageRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="86025-134">averageRoundTripTime</span></span>|<span data-ttu-id="86025-135">Duration</span><span class="sxs-lookup"><span data-stu-id="86025-135">Duration</span></span>|<span data-ttu-id="86025-136">Tempo médio de propagação de rede calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="86025-136">Average network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="86025-137">Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.</span><span class="sxs-lookup"><span data-stu-id="86025-137">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="86025-138">averageVideoFrameLossPercentage</span><span class="sxs-lookup"><span data-stu-id="86025-138">averageVideoFrameLossPercentage</span></span>|<span data-ttu-id="86025-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-139">Double</span></span>|<span data-ttu-id="86025-140">Porcentagem média de quadros de vídeo perdidos conforme exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="86025-140">Average percentage of video frames lost as displayed to the user.</span></span>|
|<span data-ttu-id="86025-141">averageVideoFrameRate</span><span class="sxs-lookup"><span data-stu-id="86025-141">averageVideoFrameRate</span></span>|<span data-ttu-id="86025-142">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-142">Double</span></span>|<span data-ttu-id="86025-143">Quadros médios por segundo recebidos para um fluxo de vídeo, calculados durante a duração da sessão.</span><span class="sxs-lookup"><span data-stu-id="86025-143">Average frames per second received for a video stream, computed over the duration of the session.</span></span>|
|<span data-ttu-id="86025-144">averageVideoPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="86025-144">averageVideoPacketLossRate</span></span>|<span data-ttu-id="86025-145">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-145">Double</span></span>|<span data-ttu-id="86025-146">Fração média de pacotes perdidos, conforme especificado em [RFC 3550][], calculado durante a duração da sessão.</span><span class="sxs-lookup"><span data-stu-id="86025-146">Average fraction of packets lost, as specified in [RFC 3550][], computed over the duration of the session.</span></span>|
|<span data-ttu-id="86025-147">endDateTime</span><span class="sxs-lookup"><span data-stu-id="86025-147">endDateTime</span></span>|<span data-ttu-id="86025-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86025-148">DateTimeOffset</span></span>|<span data-ttu-id="86025-149">Hora UTC quando o fluxo terminou.</span><span class="sxs-lookup"><span data-stu-id="86025-149">UTC time when the stream ended.</span></span> <span data-ttu-id="86025-150">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="86025-150">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="86025-151">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="86025-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="86025-152">lowFrameRateRatio</span><span class="sxs-lookup"><span data-stu-id="86025-152">lowFrameRateRatio</span></span>|<span data-ttu-id="86025-153">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-153">Double</span></span>|<span data-ttu-id="86025-154">Fração da chamada em que a taxa de quadros é inferior a 7,5 quadros por segundo.</span><span class="sxs-lookup"><span data-stu-id="86025-154">Fraction of the call where frame rate is less than 7.5 frames per second.</span></span>|
|<span data-ttu-id="86025-155">lowVideoProcessingCapabilityRatio</span><span class="sxs-lookup"><span data-stu-id="86025-155">lowVideoProcessingCapabilityRatio</span></span>|<span data-ttu-id="86025-156">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-156">Double</span></span>|<span data-ttu-id="86025-157">Fração da chamada que o cliente está executando menos de 70% do recurso de processamento de vídeo esperado.</span><span class="sxs-lookup"><span data-stu-id="86025-157">Fraction of the call that the client is running less than 70% expected video processing capability.</span></span>|
|<span data-ttu-id="86025-158">maxAudioNetworkJitter</span><span class="sxs-lookup"><span data-stu-id="86025-158">maxAudioNetworkJitter</span></span>|<span data-ttu-id="86025-159">Duration</span><span class="sxs-lookup"><span data-stu-id="86025-159">Duration</span></span>|<span data-ttu-id="86025-160">Máximo de tremedeira de rede de áudio calculada em cada uma das janelas de 20 segundos durante a sessão, denotado no [formato ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="86025-160">Maximum of audio network jitter computed over each of the 20 second windows during the session, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="86025-161">Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.</span><span class="sxs-lookup"><span data-stu-id="86025-161">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="86025-162">maxJitter</span><span class="sxs-lookup"><span data-stu-id="86025-162">maxJitter</span></span>|<span data-ttu-id="86025-163">Duration</span><span class="sxs-lookup"><span data-stu-id="86025-163">Duration</span></span>|<span data-ttu-id="86025-164">Tremedeira máxima para o fluxo calculado conforme especificado no RFC 3550, indicado no [formato ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="86025-164">Maximum jitter for the stream computed as specified in RFC 3550, denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="86025-165">Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.</span><span class="sxs-lookup"><span data-stu-id="86025-165">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="86025-166">maxPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="86025-166">maxPacketLossRate</span></span>|<span data-ttu-id="86025-167">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-167">Double</span></span>|<span data-ttu-id="86025-168">Taxa máxima de perda de pacotes para o fluxo.</span><span class="sxs-lookup"><span data-stu-id="86025-168">Maximum packet loss rate for the stream.</span></span>|
|<span data-ttu-id="86025-169">maxRatioOfConcealedSamples</span><span class="sxs-lookup"><span data-stu-id="86025-169">maxRatioOfConcealedSamples</span></span>|<span data-ttu-id="86025-170">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-170">Double</span></span>|<span data-ttu-id="86025-171">Taxa máxima de pacotes ocultos pelo curador.</span><span class="sxs-lookup"><span data-stu-id="86025-171">Maximum ratio of packets concealed by the healer.</span></span>|
|<span data-ttu-id="86025-172">maxRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="86025-172">maxRoundTripTime</span></span>|<span data-ttu-id="86025-173">Duration</span><span class="sxs-lookup"><span data-stu-id="86025-173">Duration</span></span>|<span data-ttu-id="86025-174">Tempo máximo de propagação de rede calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601.][]</span><span class="sxs-lookup"><span data-stu-id="86025-174">Maximum network propagation round-trip time computed as specified in [RFC 3550][], denoted in [ISO 8601][] format.</span></span> <span data-ttu-id="86025-175">Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.</span><span class="sxs-lookup"><span data-stu-id="86025-175">For example, 1 second is denoted as `'PT1S'`, where 'P' is the duration designator, 'T' is the time designator, and 'S' is the second designator.</span></span>|
|<span data-ttu-id="86025-176">packetUtilization</span><span class="sxs-lookup"><span data-stu-id="86025-176">packetUtilization</span></span>|<span data-ttu-id="86025-177">Int64</span><span class="sxs-lookup"><span data-stu-id="86025-177">Int64</span></span>|<span data-ttu-id="86025-178">Contagem de pacotes para o fluxo.</span><span class="sxs-lookup"><span data-stu-id="86025-178">Packet count for the stream.</span></span>|
|<span data-ttu-id="86025-179">postForwardErrorCorrectionPacketLossRate</span><span class="sxs-lookup"><span data-stu-id="86025-179">postForwardErrorCorrectionPacketLossRate</span></span>|<span data-ttu-id="86025-180">Duplo</span><span class="sxs-lookup"><span data-stu-id="86025-180">Double</span></span>|<span data-ttu-id="86025-181">Taxa de perda de pacotes após a aplicação do FEC agregada em todos os fluxos de vídeo e codecs.</span><span class="sxs-lookup"><span data-stu-id="86025-181">Packet loss rate after FEC has been applied aggregated across all video streams and codecs.</span></span>|
|<span data-ttu-id="86025-182">startDateTime</span><span class="sxs-lookup"><span data-stu-id="86025-182">startDateTime</span></span>|<span data-ttu-id="86025-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86025-183">DateTimeOffset</span></span>|<span data-ttu-id="86025-184">Hora UTC quando o fluxo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="86025-184">UTC time when the stream started.</span></span> <span data-ttu-id="86025-185">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="86025-185">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="86025-186">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="86025-186">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="86025-187">streamDirection</span><span class="sxs-lookup"><span data-stu-id="86025-187">streamDirection</span></span>|<span data-ttu-id="86025-188">microsoft.graph.callRecords.mediaStreamDirection</span><span class="sxs-lookup"><span data-stu-id="86025-188">microsoft.graph.callRecords.mediaStreamDirection</span></span>|<span data-ttu-id="86025-189">Indica a direção do fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="86025-189">Indicates the direction of the media stream.</span></span> <span data-ttu-id="86025-190">Os valores possíveis são: `callerToCallee` e `calleeToCaller`.</span><span class="sxs-lookup"><span data-stu-id="86025-190">Possible values are: `callerToCallee`, `calleeToCaller`.</span></span>|
|<span data-ttu-id="86025-191">streamId</span><span class="sxs-lookup"><span data-stu-id="86025-191">streamId</span></span>|<span data-ttu-id="86025-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86025-192">String</span></span>|<span data-ttu-id="86025-193">Identificador exclusivo do fluxo.</span><span class="sxs-lookup"><span data-stu-id="86025-193">Unique identifier for the stream.</span></span>|
|<span data-ttu-id="86025-194">wasMediaBypassed</span><span class="sxs-lookup"><span data-stu-id="86025-194">wasMediaBypassed</span></span>|<span data-ttu-id="86025-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="86025-195">Boolean</span></span>|<span data-ttu-id="86025-196">True se o fluxo de mídia ignorar o Servidor de Mediação e ir direto entre cliente e Gateway PSTN/PBX, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="86025-196">True if the media stream bypassed the Mediation Server and went straight between client and PSTN Gateway/PBX, false otherwise.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="86025-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86025-197">JSON representation</span></span>

<span data-ttu-id="86025-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86025-198">The following is a JSON representation of the resource.</span></span>

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

