---
title: tipo de recurso networkInfo
description: O tipo networkInfo
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fcf683d99d660d6ea69ee944542e6701d2201a9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069362"
---
# <a name="networkinfo-resource-type"></a><span data-ttu-id="6d26e-103">tipo de recurso networkInfo</span><span class="sxs-lookup"><span data-stu-id="6d26e-103">networkInfo resource type</span></span>

<span data-ttu-id="6d26e-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="6d26e-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="6d26e-105">Representa informações sobre a rede usada em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="6d26e-105">Represents information about the network used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="6d26e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d26e-106">Properties</span></span>

| <span data-ttu-id="6d26e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d26e-107">Property</span></span>     | <span data-ttu-id="6d26e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d26e-108">Type</span></span>        | <span data-ttu-id="6d26e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d26e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6d26e-110">bandwidthLowEventRatio</span><span class="sxs-lookup"><span data-stu-id="6d26e-110">bandwidthLowEventRatio</span></span>|<span data-ttu-id="6d26e-111">Duplo</span><span class="sxs-lookup"><span data-stu-id="6d26e-111">Double</span></span>|<span data-ttu-id="6d26e-112">Fração da chamada em que o ponto de extremidade de mídia detectou que a política de largura de banda ou largura de banda disponível era baixa o suficiente para causar baixa qualidade do áudio enviado.</span><span class="sxs-lookup"><span data-stu-id="6d26e-112">Fraction of the call that the media endpoint detected the available bandwidth or bandwidth policy was low enough to cause poor quality of the audio sent.</span></span>|
|<span data-ttu-id="6d26e-113">basicServiceSetIdentifier</span><span class="sxs-lookup"><span data-stu-id="6d26e-113">basicServiceSetIdentifier</span></span>|<span data-ttu-id="6d26e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-114">String</span></span>|<span data-ttu-id="6d26e-115">O identificador do conjunto de serviços básicos de LAN sem fio do ponto de extremidade de mídia usado para se conectar à rede.</span><span class="sxs-lookup"><span data-stu-id="6d26e-115">The wireless LAN basic service set identifier of the media endpoint used to connect to the network.</span></span>|
|<span data-ttu-id="6d26e-116">Connection</span><span class="sxs-lookup"><span data-stu-id="6d26e-116">connectionType</span></span>|<span data-ttu-id="6d26e-117">Microsoft. Graph. callRecords. networkConnectionType</span><span class="sxs-lookup"><span data-stu-id="6d26e-117">microsoft.graph.callRecords.networkConnectionType</span></span>|<span data-ttu-id="6d26e-118">Tipo de rede usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-118">Type of network used by the media endpoint.</span></span> <span data-ttu-id="6d26e-119">Os possíveis valores são: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6d26e-119">Possible values are: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6d26e-120">delayEventRatio</span><span class="sxs-lookup"><span data-stu-id="6d26e-120">delayEventRatio</span></span>|<span data-ttu-id="6d26e-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="6d26e-121">Double</span></span>|<span data-ttu-id="6d26e-122">Fração da chamada em que o ponto de extremidade de mídia detectou que o atraso de rede era suficientemente significativo para afetar a capacidade de comunicação bidirecional em tempo real.</span><span class="sxs-lookup"><span data-stu-id="6d26e-122">Fraction of the call that the media endpoint detected the network delay was significant enough to impact the ability to have real-time two-way communication.</span></span>|
|<span data-ttu-id="6d26e-123">dnsSuffix</span><span class="sxs-lookup"><span data-stu-id="6d26e-123">dnsSuffix</span></span>|<span data-ttu-id="6d26e-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-124">String</span></span>|<span data-ttu-id="6d26e-125">Sufixo DNS associado ao adaptador de rede do ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-125">DNS suffix associated with the network adapter of the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6d26e-126">ipAddress</span></span>|<span data-ttu-id="6d26e-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-127">String</span></span>|<span data-ttu-id="6d26e-128">Endereço IP do ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-128">IP address of the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-129">linkSpeed</span><span class="sxs-lookup"><span data-stu-id="6d26e-129">linkSpeed</span></span>|<span data-ttu-id="6d26e-130">Int64</span><span class="sxs-lookup"><span data-stu-id="6d26e-130">Int64</span></span>|<span data-ttu-id="6d26e-131">Velocidade do link em bits por segundo relatado pelo adaptador de rede usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-131">Link speed in bits per second reported by the network adapter used by the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-132">macAddress</span><span class="sxs-lookup"><span data-stu-id="6d26e-132">macAddress</span></span>|<span data-ttu-id="6d26e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-133">String</span></span>|<span data-ttu-id="6d26e-134">O endereço MAC (controle de acesso de mídia) do dispositivo de rede do ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-134">The media access control (MAC) address of the media endpoint's network device.</span></span>|
|<span data-ttu-id="6d26e-135">propor</span><span class="sxs-lookup"><span data-stu-id="6d26e-135">port</span></span>|<span data-ttu-id="6d26e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6d26e-136">Int32</span></span>|<span data-ttu-id="6d26e-137">Número da porta de rede usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-137">Network port number used by media endpoint.</span></span>|
|<span data-ttu-id="6d26e-138">receivedQualityEventRatio</span><span class="sxs-lookup"><span data-stu-id="6d26e-138">receivedQualityEventRatio</span></span>|<span data-ttu-id="6d26e-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="6d26e-139">Double</span></span>|<span data-ttu-id="6d26e-140">Fração da chamada em que o ponto de extremidade de mídia detectou que a rede estava causando baixa qualidade do áudio recebido.</span><span class="sxs-lookup"><span data-stu-id="6d26e-140">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio received.</span></span>|
|<span data-ttu-id="6d26e-141">reflexiveIPAddress</span><span class="sxs-lookup"><span data-stu-id="6d26e-141">reflexiveIPAddress</span></span>|<span data-ttu-id="6d26e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-142">String</span></span>|<span data-ttu-id="6d26e-143">Endereço IP do ponto de extremidade de mídia conforme visto pelo servidor de Media Relay.</span><span class="sxs-lookup"><span data-stu-id="6d26e-143">IP address of the media endpoint as seen by the media relay server.</span></span> <span data-ttu-id="6d26e-144">Em geral, esse é o endereço IP público da Internet associado ao ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="6d26e-144">This is typically the public internet IP address associated to the endpoint.</span></span>|
|<span data-ttu-id="6d26e-145">relayIPAddress</span><span class="sxs-lookup"><span data-stu-id="6d26e-145">relayIPAddress</span></span>|<span data-ttu-id="6d26e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-146">String</span></span>|<span data-ttu-id="6d26e-147">Endereço IP do servidor de Media Relay alocado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-147">IP address of the media relay server allocated by the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-148">relayPort</span><span class="sxs-lookup"><span data-stu-id="6d26e-148">relayPort</span></span>|<span data-ttu-id="6d26e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6d26e-149">Int32</span></span>|<span data-ttu-id="6d26e-150">Número de porta de rede alocado no servidor de Media Relay pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-150">Network port number allocated on the media relay server by the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-151">sentQualityEventRatio</span><span class="sxs-lookup"><span data-stu-id="6d26e-151">sentQualityEventRatio</span></span>|<span data-ttu-id="6d26e-152">Duplo</span><span class="sxs-lookup"><span data-stu-id="6d26e-152">Double</span></span>|<span data-ttu-id="6d26e-153">Fração da chamada em que o ponto de extremidade de mídia detectou que a rede estava causando baixa qualidade do áudio enviado.</span><span class="sxs-lookup"><span data-stu-id="6d26e-153">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio sent.</span></span>|
|<span data-ttu-id="6d26e-154">-</span><span class="sxs-lookup"><span data-stu-id="6d26e-154">subnet</span></span>|<span data-ttu-id="6d26e-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-155">String</span></span>|<span data-ttu-id="6d26e-156">Sub-rede usada para fluxo de mídia pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-156">Subnet used for media stream by the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-157">wifiBand</span><span class="sxs-lookup"><span data-stu-id="6d26e-157">wifiBand</span></span>|<span data-ttu-id="6d26e-158">Microsoft. Graph. callRecords. wifiBand</span><span class="sxs-lookup"><span data-stu-id="6d26e-158">microsoft.graph.callRecords.wifiBand</span></span>|<span data-ttu-id="6d26e-159">Banda WiFi usada pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-159">WiFi band used by the media endpoint.</span></span> <span data-ttu-id="6d26e-160">Os valores possíveis são: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6d26e-160">Possible values are: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6d26e-161">wifiBatteryCharge</span><span class="sxs-lookup"><span data-stu-id="6d26e-161">wifiBatteryCharge</span></span>|<span data-ttu-id="6d26e-162">Int32</span><span class="sxs-lookup"><span data-stu-id="6d26e-162">Int32</span></span>|<span data-ttu-id="6d26e-163">Carga da bateria restante estimada em porcentagem relatada pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-163">Estimated remaining battery charge in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-164">wifiChannel</span><span class="sxs-lookup"><span data-stu-id="6d26e-164">wifiChannel</span></span>|<span data-ttu-id="6d26e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6d26e-165">Int32</span></span>|<span data-ttu-id="6d26e-166">O canal WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-166">WiFi channel used by the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-167">wifiMicrosoftDriver</span><span class="sxs-lookup"><span data-stu-id="6d26e-167">wifiMicrosoftDriver</span></span>|<span data-ttu-id="6d26e-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-168">String</span></span>|<span data-ttu-id="6d26e-169">Nome do driver do Microsoft WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-169">Name of the Microsoft WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="6d26e-170">O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="6d26e-170">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="6d26e-171">wifiMicrosoftDriverVersion</span><span class="sxs-lookup"><span data-stu-id="6d26e-171">wifiMicrosoftDriverVersion</span></span>|<span data-ttu-id="6d26e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-172">String</span></span>|<span data-ttu-id="6d26e-173">Versão do driver do Microsoft WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-173">Version of the Microsoft WiFi driver used by the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-174">wifiRadioType</span><span class="sxs-lookup"><span data-stu-id="6d26e-174">wifiRadioType</span></span>|<span data-ttu-id="6d26e-175">Microsoft. Graph. callRecords. wifiRadioType</span><span class="sxs-lookup"><span data-stu-id="6d26e-175">microsoft.graph.callRecords.wifiRadioType</span></span>|<span data-ttu-id="6d26e-176">Tipo de rádio WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-176">Type of WiFi radio used by the media endpoint.</span></span> <span data-ttu-id="6d26e-177">Os valores possíveis são: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6d26e-177">Possible values are: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6d26e-178">wifiSignalStrength</span><span class="sxs-lookup"><span data-stu-id="6d26e-178">wifiSignalStrength</span></span>|<span data-ttu-id="6d26e-179">Int32</span><span class="sxs-lookup"><span data-stu-id="6d26e-179">Int32</span></span>|<span data-ttu-id="6d26e-180">Intensidade do sinal WiFi em porcentagem reportada pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-180">WiFi signal strength in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="6d26e-181">wifiVendorDriver</span><span class="sxs-lookup"><span data-stu-id="6d26e-181">wifiVendorDriver</span></span>|<span data-ttu-id="6d26e-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-182">String</span></span>|<span data-ttu-id="6d26e-183">Nome do driver WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-183">Name of the WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="6d26e-184">O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="6d26e-184">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="6d26e-185">wifiVendorDriverVersion</span><span class="sxs-lookup"><span data-stu-id="6d26e-185">wifiVendorDriverVersion</span></span>|<span data-ttu-id="6d26e-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d26e-186">String</span></span>|<span data-ttu-id="6d26e-187">Versão do driver WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="6d26e-187">Version of the WiFi driver used by the media endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d26e-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d26e-188">JSON representation</span></span>

<span data-ttu-id="6d26e-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d26e-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.networkInfo",
  "baseType": null
}-->

```json
{
  "bandwidthLowEventRatio": "Double",
  "basicServiceSetIdentifier": "String",
  "connectionType": "String",
  "delayEventRatio": "Double",
  "dnsSuffix": "String",
  "ipAddress": "String",
  "linkSpeed": 1024,
  "macAddress": "String",
  "port": 1024,
  "receivedQualityEventRatio": "Double",
  "reflexiveIPAddress": "String",
  "relayIPAddress": "String",
  "relayPort": 1024,
  "sentQualityEventRatio": "Double",
  "subnet": "String",
  "wifiBand": "String",
  "wifiBatteryCharge": 1024,
  "wifiChannel": 1024,
  "wifiMicrosoftDriver": "String",
  "wifiMicrosoftDriverVersion": "String",
  "wifiRadioType": "String",
  "wifiSignalStrength": 1024,
  "wifiVendorDriver": "String",
  "wifiVendorDriverVersion": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
