---
title: tipo de recurso deviceInfo
description: O tipo deviceInfo
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 944e827e0e7827190b3ff879a2f62d52d6fa15c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071515"
---
# <a name="deviceinfo-resource-type"></a><span data-ttu-id="5ee56-103">tipo de recurso deviceInfo</span><span class="sxs-lookup"><span data-stu-id="5ee56-103">deviceInfo resource type</span></span>

<span data-ttu-id="5ee56-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="5ee56-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ee56-105">Representa informações sobre um dispositivo (microfone, alto-falante, câmera, etc.) usados em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="5ee56-105">Represents information about a device (microphone, speaker, camera, etc.) used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="5ee56-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ee56-106">Properties</span></span>

| <span data-ttu-id="5ee56-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ee56-107">Property</span></span>     | <span data-ttu-id="5ee56-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ee56-108">Type</span></span>        | <span data-ttu-id="5ee56-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee56-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5ee56-110">captureDeviceDriver</span><span class="sxs-lookup"><span data-stu-id="5ee56-110">captureDeviceDriver</span></span>|<span data-ttu-id="5ee56-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee56-111">String</span></span>|<span data-ttu-id="5ee56-112">Nome do driver do dispositivo de captura usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="5ee56-112">Name of the capture device driver used by the media endpoint.</span></span>|
|<span data-ttu-id="5ee56-113">captureDeviceName</span><span class="sxs-lookup"><span data-stu-id="5ee56-113">captureDeviceName</span></span>|<span data-ttu-id="5ee56-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee56-114">String</span></span>|<span data-ttu-id="5ee56-115">Nome do dispositivo de captura usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="5ee56-115">Name of the capture device used by the media endpoint.</span></span>|
|<span data-ttu-id="5ee56-116">captureNotFunctioningEventRatio</span><span class="sxs-lookup"><span data-stu-id="5ee56-116">captureNotFunctioningEventRatio</span></span>|<span data-ttu-id="5ee56-117">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-117">Double</span></span>|<span data-ttu-id="5ee56-118">Fração da chamada em que o ponto de extremidade de mídia detectou que o dispositivo de captura não estava funcionando corretamente.</span><span class="sxs-lookup"><span data-stu-id="5ee56-118">Fraction of the call that the media endpoint detected the capture device was not working properly.</span></span>|
|<span data-ttu-id="5ee56-119">cpuInsufficentEventRatio</span><span class="sxs-lookup"><span data-stu-id="5ee56-119">cpuInsufficentEventRatio</span></span>|<span data-ttu-id="5ee56-120">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-120">Double</span></span>|<span data-ttu-id="5ee56-121">Fração da chamada em que o ponto de extremidade de mídia detectou que os recursos de CPU disponíveis eram insuficientes e causaram baixa qualidade do áudio enviado e recebido.</span><span class="sxs-lookup"><span data-stu-id="5ee56-121">Fraction of the call that the media endpoint detected the CPU resources available were insufficient and caused poor quality of the audio sent and received.</span></span>|
|<span data-ttu-id="5ee56-122">deviceClippingEventRatio</span><span class="sxs-lookup"><span data-stu-id="5ee56-122">deviceClippingEventRatio</span></span>|<span data-ttu-id="5ee56-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-123">Double</span></span>|<span data-ttu-id="5ee56-124">Fração da chamada que o ponto de extremidade de mídia detectou o corte no áudio capturado que causou baixa qualidade do áudio que está sendo enviado.</span><span class="sxs-lookup"><span data-stu-id="5ee56-124">Fraction of the call that the media endpoint detected clipping in the captured audio that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="5ee56-125">deviceGlitchEventRatio</span><span class="sxs-lookup"><span data-stu-id="5ee56-125">deviceGlitchEventRatio</span></span>|<span data-ttu-id="5ee56-126">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-126">Double</span></span>|<span data-ttu-id="5ee56-127">Fração da chamada em que o ponto de extremidade de mídia detectou falhas ou intervalos no áudio reproduzido ou capturado que causou baixa qualidade do áudio enviado ou recebido.</span><span class="sxs-lookup"><span data-stu-id="5ee56-127">Fraction of the call that the media endpoint detected glitches or gaps in the audio played or captured that caused poor quality of the audio being sent or received.</span></span>|
|<span data-ttu-id="5ee56-128">howlingEventCount</span><span class="sxs-lookup"><span data-stu-id="5ee56-128">howlingEventCount</span></span>|<span data-ttu-id="5ee56-129">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee56-129">Int32</span></span>|<span data-ttu-id="5ee56-130">Número de vezes durante a chamada em que o ponto de extremidade de mídia detectou o Howling ou o arranhão Audio.</span><span class="sxs-lookup"><span data-stu-id="5ee56-130">Number of times during the call that the media endpoint detected howling or screeching audio.</span></span>|
|<span data-ttu-id="5ee56-131">initialSignalLevelRootMeanSquare</span><span class="sxs-lookup"><span data-stu-id="5ee56-131">initialSignalLevelRootMeanSquare</span></span>|<span data-ttu-id="5ee56-132">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-132">Double</span></span>|<span data-ttu-id="5ee56-133">O quadrado de raiz média (RMS) do sinal de entrada de até os primeiros 30 segundos da chamada.</span><span class="sxs-lookup"><span data-stu-id="5ee56-133">The root mean square (RMS) of the incoming signal of up to the first 30 seconds of the call.</span></span>|
|<span data-ttu-id="5ee56-134">lowSpeechLevelEventRatio</span><span class="sxs-lookup"><span data-stu-id="5ee56-134">lowSpeechLevelEventRatio</span></span>|<span data-ttu-id="5ee56-135">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-135">Double</span></span>|<span data-ttu-id="5ee56-136">Fração da chamada que o ponto de extremidade de mídia detectou baixo nível de fala que causou baixa qualidade do áudio que está sendo enviado.</span><span class="sxs-lookup"><span data-stu-id="5ee56-136">Fraction of the call that the media endpoint detected low speech level that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="5ee56-137">lowSpeechToNoiseEventRatio</span><span class="sxs-lookup"><span data-stu-id="5ee56-137">lowSpeechToNoiseEventRatio</span></span>|<span data-ttu-id="5ee56-138">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-138">Double</span></span>|<span data-ttu-id="5ee56-139">Fração da chamada em que o ponto de extremidade de mídia detectou baixa fala no nível de ruído que causou baixa qualidade do áudio que está sendo enviado.</span><span class="sxs-lookup"><span data-stu-id="5ee56-139">Fraction of the call that the media endpoint detected low speech to noise level that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="5ee56-140">micGlitchRate</span><span class="sxs-lookup"><span data-stu-id="5ee56-140">micGlitchRate</span></span>|<span data-ttu-id="5ee56-141">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-141">Double</span></span>|<span data-ttu-id="5ee56-142">Falhas por intervalo de 5 minutos para o microfone do ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="5ee56-142">Glitches per 5 minute interval for the media endpoint's microphone.</span></span>|
|<span data-ttu-id="5ee56-143">receivedNoiseLevel</span><span class="sxs-lookup"><span data-stu-id="5ee56-143">receivedNoiseLevel</span></span>|<span data-ttu-id="5ee56-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee56-144">Int32</span></span>|<span data-ttu-id="5ee56-145">Nível de energia médio do áudio recebido para áudio classificado como ruído mono ou canal esquerdo de ruído estéreo pelo ponto de extremidade da mídia.</span><span class="sxs-lookup"><span data-stu-id="5ee56-145">Average energy level of received audio for audio classified as mono noise or left channel of stereo noise by the media endpoint.</span></span>|
|<span data-ttu-id="5ee56-146">receivedSignalLevel</span><span class="sxs-lookup"><span data-stu-id="5ee56-146">receivedSignalLevel</span></span>|<span data-ttu-id="5ee56-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee56-147">Int32</span></span>|<span data-ttu-id="5ee56-148">Nível de energia médio do áudio recebido para áudio classificado como fala mono ou canal esquerdo de fala estéreo pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="5ee56-148">Average energy level of received audio for audio classified as mono speech, or left channel of stereo speech by the media endpoint.</span></span>|
|<span data-ttu-id="5ee56-149">renderDeviceDriver</span><span class="sxs-lookup"><span data-stu-id="5ee56-149">renderDeviceDriver</span></span>|<span data-ttu-id="5ee56-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee56-150">String</span></span>|<span data-ttu-id="5ee56-151">Nome do driver de dispositivo de renderização usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="5ee56-151">Name of the render device driver used by the media endpoint.</span></span>|
|<span data-ttu-id="5ee56-152">renderDeviceName</span><span class="sxs-lookup"><span data-stu-id="5ee56-152">renderDeviceName</span></span>|<span data-ttu-id="5ee56-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee56-153">String</span></span>|<span data-ttu-id="5ee56-154">Nome do dispositivo de renderização usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="5ee56-154">Name of the render device used by the media endpoint.</span></span>|
|<span data-ttu-id="5ee56-155">renderMuteEventRatio</span><span class="sxs-lookup"><span data-stu-id="5ee56-155">renderMuteEventRatio</span></span>|<span data-ttu-id="5ee56-156">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-156">Double</span></span>|<span data-ttu-id="5ee56-157">Fração da chamada em que o ponto de extremidade de mídia detectou o processamento do dispositivo está com mudo ativado.</span><span class="sxs-lookup"><span data-stu-id="5ee56-157">Fraction of the call that media endpoint detected device render is muted.</span></span>|
|<span data-ttu-id="5ee56-158">renderNotFunctioningEventRatio</span><span class="sxs-lookup"><span data-stu-id="5ee56-158">renderNotFunctioningEventRatio</span></span>|<span data-ttu-id="5ee56-159">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-159">Double</span></span>|<span data-ttu-id="5ee56-160">Fração da chamada em que o ponto de extremidade de mídia detectou que o dispositivo de renderização não estava funcionando corretamente.</span><span class="sxs-lookup"><span data-stu-id="5ee56-160">Fraction of the call that the media endpoint detected the render device was not working properly.</span></span>|
|<span data-ttu-id="5ee56-161">renderZeroVolumeEventRatio</span><span class="sxs-lookup"><span data-stu-id="5ee56-161">renderZeroVolumeEventRatio</span></span>|<span data-ttu-id="5ee56-162">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-162">Double</span></span>|<span data-ttu-id="5ee56-163">Fração da chamada que o ponto de extremidade de mídia detectou que o volume de renderização do dispositivo está definido como 0.</span><span class="sxs-lookup"><span data-stu-id="5ee56-163">Fraction of the call that media endpoint detected device render volume is set to 0.</span></span>|
|<span data-ttu-id="5ee56-164">sentNoiseLevel</span><span class="sxs-lookup"><span data-stu-id="5ee56-164">sentNoiseLevel</span></span>|<span data-ttu-id="5ee56-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee56-165">Int32</span></span>|<span data-ttu-id="5ee56-166">Nível de energia médio do áudio enviado para áudio classificado como ruído mono ou canal esquerdo de ruído estéreo pelo ponto de extremidade da mídia.</span><span class="sxs-lookup"><span data-stu-id="5ee56-166">Average energy level of sent audio for audio classified as mono noise or left channel of stereo noise by the media endpoint.</span></span>|
|<span data-ttu-id="5ee56-167">sentSignalLevel</span><span class="sxs-lookup"><span data-stu-id="5ee56-167">sentSignalLevel</span></span>|<span data-ttu-id="5ee56-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee56-168">Int32</span></span>|<span data-ttu-id="5ee56-169">Nível de energia médio do áudio enviado para áudio classificado como fala mono ou canal esquerdo de fala estéreo pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="5ee56-169">Average energy level of sent audio for audio classified as mono speech, or left channel of stereo speech by the media endpoint.</span></span>|
|<span data-ttu-id="5ee56-170">speakerGlitchRate</span><span class="sxs-lookup"><span data-stu-id="5ee56-170">speakerGlitchRate</span></span>|<span data-ttu-id="5ee56-171">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ee56-171">Double</span></span>|<span data-ttu-id="5ee56-172">Falhas por 5 minutos internas para o ponto de extremidade de mídia Loudspeaker.</span><span class="sxs-lookup"><span data-stu-id="5ee56-172">Glitches per 5 minute internal for the media endpoint's loudspeaker.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5ee56-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ee56-173">JSON representation</span></span>

<span data-ttu-id="5ee56-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ee56-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.deviceInfo",
  "baseType": null
}-->

```json
{
  "captureDeviceDriver": "String",
  "captureDeviceName": "String",
  "captureNotFunctioningEventRatio": "Double",
  "cpuInsufficentEventRatio": "Double",
  "deviceClippingEventRatio": "Double",
  "deviceGlitchEventRatio": "Double",
  "howlingEventCount": 1024,
  "initialSignalLevelRootMeanSquare": "Double",
  "lowSpeechLevelEventRatio": "Double",
  "lowSpeechToNoiseEventRatio": "Double",
  "micGlitchRate": "Double",
  "receivedNoiseLevel": 1024,
  "receivedSignalLevel": 1024,
  "renderDeviceDriver": "String",
  "renderDeviceName": "String",
  "renderMuteEventRatio": "Double",
  "renderNotFunctioningEventRatio": "Double",
  "renderZeroVolumeEventRatio": "Double",
  "sentNoiseLevel": 1024,
  "sentSignalLevel": 1024,
  "speakerGlitchRate": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

