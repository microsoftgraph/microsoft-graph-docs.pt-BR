---
title: tipo de recurso networkInfo
description: O tipo networkInfo
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c24f53054d474ac8a50959127d98f5920789e620
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394658"
---
# <a name="networkinfo-resource-type"></a><span data-ttu-id="74698-103">tipo de recurso networkInfo</span><span class="sxs-lookup"><span data-stu-id="74698-103">networkInfo resource type</span></span>

<span data-ttu-id="74698-104">Namespace: Microsoft. Graph. callRecords</span><span class="sxs-lookup"><span data-stu-id="74698-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74698-105">Representa informações sobre a rede usada em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="74698-105">Represents information about the network used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="74698-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74698-106">Properties</span></span>

| <span data-ttu-id="74698-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74698-107">Property</span></span>     | <span data-ttu-id="74698-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="74698-108">Type</span></span>        | <span data-ttu-id="74698-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="74698-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74698-110">bandwidthLowEventRatio</span><span class="sxs-lookup"><span data-stu-id="74698-110">bandwidthLowEventRatio</span></span>|<span data-ttu-id="74698-111">Duplo</span><span class="sxs-lookup"><span data-stu-id="74698-111">Double</span></span>|<span data-ttu-id="74698-112">Fração da chamada em que o ponto de extremidade de mídia detectou que a política de largura de banda ou largura de banda disponível era baixa o suficiente para causar baixa qualidade do áudio enviado.</span><span class="sxs-lookup"><span data-stu-id="74698-112">Fraction of the call that the media endpoint detected the available bandwidth or bandwidth policy was low enough to cause poor quality of the audio sent.</span></span>|
|<span data-ttu-id="74698-113">basicServiceSetIdentifier</span><span class="sxs-lookup"><span data-stu-id="74698-113">basicServiceSetIdentifier</span></span>|<span data-ttu-id="74698-114">String</span><span class="sxs-lookup"><span data-stu-id="74698-114">String</span></span>|<span data-ttu-id="74698-115">O identificador do conjunto de serviços básicos de LAN sem fio do ponto de extremidade de mídia usado para se conectar à rede.</span><span class="sxs-lookup"><span data-stu-id="74698-115">The wireless LAN basic service set identifier of the media endpoint used to connect to the network.</span></span>|
|<span data-ttu-id="74698-116">Connection</span><span class="sxs-lookup"><span data-stu-id="74698-116">connectionType</span></span>|<span data-ttu-id="74698-117">String</span><span class="sxs-lookup"><span data-stu-id="74698-117">String</span></span>|<span data-ttu-id="74698-118">Tipo de rede usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-118">Type of network used by the media endpoint.</span></span> <span data-ttu-id="74698-119">Os possíveis valores são: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="74698-119">Possible values are: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="74698-120">delayEventRatio</span><span class="sxs-lookup"><span data-stu-id="74698-120">delayEventRatio</span></span>|<span data-ttu-id="74698-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="74698-121">Double</span></span>|<span data-ttu-id="74698-122">Fração da chamada em que o ponto de extremidade de mídia detectou que o atraso de rede era suficientemente significativo para afetar a capacidade de comunicação bidirecional em tempo real.</span><span class="sxs-lookup"><span data-stu-id="74698-122">Fraction of the call that the media endpoint detected the network delay was significant enough to impact the ability to have real-time two-way communication.</span></span>|
|<span data-ttu-id="74698-123">dnsSuffix</span><span class="sxs-lookup"><span data-stu-id="74698-123">dnsSuffix</span></span>|<span data-ttu-id="74698-124">String</span><span class="sxs-lookup"><span data-stu-id="74698-124">String</span></span>|<span data-ttu-id="74698-125">Sufixo DNS associado ao adaptador de rede do ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-125">DNS suffix associated with the network adapter of the media endpoint.</span></span>|
|<span data-ttu-id="74698-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="74698-126">ipAddress</span></span>|<span data-ttu-id="74698-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74698-127">String</span></span>|<span data-ttu-id="74698-128">Endereço IP do ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-128">IP address of the media endpoint.</span></span>|
|<span data-ttu-id="74698-129">linkSpeed</span><span class="sxs-lookup"><span data-stu-id="74698-129">linkSpeed</span></span>|<span data-ttu-id="74698-130">Int64</span><span class="sxs-lookup"><span data-stu-id="74698-130">Int64</span></span>|<span data-ttu-id="74698-131">Velocidade do link em bits por segundo relatado pelo adaptador de rede usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-131">Link speed in bits per second reported by the network adapter used by the media endpoint.</span></span>|
|<span data-ttu-id="74698-132">macAddress</span><span class="sxs-lookup"><span data-stu-id="74698-132">macAddress</span></span>|<span data-ttu-id="74698-133">String</span><span class="sxs-lookup"><span data-stu-id="74698-133">String</span></span>|<span data-ttu-id="74698-134">O endereço MAC (controle de acesso de mídia) do dispositivo de rede do ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-134">The media access control (MAC) address of the media endpoint's network device.</span></span>|
|<span data-ttu-id="74698-135">propor</span><span class="sxs-lookup"><span data-stu-id="74698-135">port</span></span>|<span data-ttu-id="74698-136">Int32</span><span class="sxs-lookup"><span data-stu-id="74698-136">Int32</span></span>|<span data-ttu-id="74698-137">Número da porta de rede usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-137">Network port number used by media endpoint.</span></span>|
|<span data-ttu-id="74698-138">receivedQualityEventRatio</span><span class="sxs-lookup"><span data-stu-id="74698-138">receivedQualityEventRatio</span></span>|<span data-ttu-id="74698-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="74698-139">Double</span></span>|<span data-ttu-id="74698-140">Fração da chamada em que o ponto de extremidade de mídia detectou que a rede estava causando baixa qualidade do áudio recebido.</span><span class="sxs-lookup"><span data-stu-id="74698-140">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio received.</span></span>|
|<span data-ttu-id="74698-141">reflexiveIPAddress</span><span class="sxs-lookup"><span data-stu-id="74698-141">reflexiveIPAddress</span></span>|<span data-ttu-id="74698-142">String</span><span class="sxs-lookup"><span data-stu-id="74698-142">String</span></span>|<span data-ttu-id="74698-143">Endereço IP do ponto de extremidade de mídia conforme visto pelo servidor de Media Relay.</span><span class="sxs-lookup"><span data-stu-id="74698-143">IP address of the media endpoint as seen by the media relay server.</span></span> <span data-ttu-id="74698-144">Em geral, esse é o endereço IP público da Internet associado ao ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="74698-144">This is typically the public internet IP address associated to the endpoint.</span></span>|
|<span data-ttu-id="74698-145">relayIPAddress</span><span class="sxs-lookup"><span data-stu-id="74698-145">relayIPAddress</span></span>|<span data-ttu-id="74698-146">String</span><span class="sxs-lookup"><span data-stu-id="74698-146">String</span></span>|<span data-ttu-id="74698-147">Endereço IP do servidor de Media Relay alocado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-147">IP address of the media relay server allocated by the media endpoint.</span></span>|
|<span data-ttu-id="74698-148">relayPort</span><span class="sxs-lookup"><span data-stu-id="74698-148">relayPort</span></span>|<span data-ttu-id="74698-149">Int32</span><span class="sxs-lookup"><span data-stu-id="74698-149">Int32</span></span>|<span data-ttu-id="74698-150">Número de porta de rede alocado no servidor de Media Relay pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-150">Network port number allocated on the media relay server by the media endpoint.</span></span>|
|<span data-ttu-id="74698-151">sentQualityEventRatio</span><span class="sxs-lookup"><span data-stu-id="74698-151">sentQualityEventRatio</span></span>|<span data-ttu-id="74698-152">Duplo</span><span class="sxs-lookup"><span data-stu-id="74698-152">Double</span></span>|<span data-ttu-id="74698-153">Fração da chamada em que o ponto de extremidade de mídia detectou que a rede estava causando baixa qualidade do áudio enviado.</span><span class="sxs-lookup"><span data-stu-id="74698-153">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio sent.</span></span>|
|<span data-ttu-id="74698-154">-</span><span class="sxs-lookup"><span data-stu-id="74698-154">subnet</span></span>|<span data-ttu-id="74698-155">String</span><span class="sxs-lookup"><span data-stu-id="74698-155">String</span></span>|<span data-ttu-id="74698-156">Sub-rede usada para fluxo de mídia pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-156">Subnet used for media stream by the media endpoint.</span></span>|
|<span data-ttu-id="74698-157">wifiBand</span><span class="sxs-lookup"><span data-stu-id="74698-157">wifiBand</span></span>|<span data-ttu-id="74698-158">String</span><span class="sxs-lookup"><span data-stu-id="74698-158">String</span></span>|<span data-ttu-id="74698-159">Banda WiFi usada pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-159">WiFi band used by the media endpoint.</span></span> <span data-ttu-id="74698-160">Os valores possíveis são: `unknown`, `frequency24GHz`, `frequency50GHz`.</span><span class="sxs-lookup"><span data-stu-id="74698-160">Possible values are: `unknown`, `frequency24GHz`, `frequency50GHz`.</span></span>|
|<span data-ttu-id="74698-161">wifiBatteryCharge</span><span class="sxs-lookup"><span data-stu-id="74698-161">wifiBatteryCharge</span></span>|<span data-ttu-id="74698-162">Int32</span><span class="sxs-lookup"><span data-stu-id="74698-162">Int32</span></span>|<span data-ttu-id="74698-163">Carga da bateria restante estimada em porcentagem relatada pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-163">Estimated remaining battery charge in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="74698-164">wifiChannel</span><span class="sxs-lookup"><span data-stu-id="74698-164">wifiChannel</span></span>|<span data-ttu-id="74698-165">Int32</span><span class="sxs-lookup"><span data-stu-id="74698-165">Int32</span></span>|<span data-ttu-id="74698-166">O canal WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-166">WiFi channel used by the media endpoint.</span></span>|
|<span data-ttu-id="74698-167">wifiMicrosoftDriver</span><span class="sxs-lookup"><span data-stu-id="74698-167">wifiMicrosoftDriver</span></span>|<span data-ttu-id="74698-168">String</span><span class="sxs-lookup"><span data-stu-id="74698-168">String</span></span>|<span data-ttu-id="74698-169">Nome do driver do Microsoft WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-169">Name of the Microsoft WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="74698-170">O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="74698-170">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="74698-171">wifiMicrosoftDriverVersion</span><span class="sxs-lookup"><span data-stu-id="74698-171">wifiMicrosoftDriverVersion</span></span>|<span data-ttu-id="74698-172">String</span><span class="sxs-lookup"><span data-stu-id="74698-172">String</span></span>|<span data-ttu-id="74698-173">Versão do driver do Microsoft WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-173">Version of the Microsoft WiFi driver used by the media endpoint.</span></span>|
|<span data-ttu-id="74698-174">wifiRadioType</span><span class="sxs-lookup"><span data-stu-id="74698-174">wifiRadioType</span></span>|<span data-ttu-id="74698-175">String</span><span class="sxs-lookup"><span data-stu-id="74698-175">String</span></span>|<span data-ttu-id="74698-176">Tipo de rádio WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-176">Type of WiFi radio used by the media endpoint.</span></span> <span data-ttu-id="74698-177">Os valores possíveis são: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="74698-177">Possible values are: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="74698-178">wifiSignalStrength</span><span class="sxs-lookup"><span data-stu-id="74698-178">wifiSignalStrength</span></span>|<span data-ttu-id="74698-179">Int32</span><span class="sxs-lookup"><span data-stu-id="74698-179">Int32</span></span>|<span data-ttu-id="74698-180">Intensidade do sinal WiFi em porcentagem reportada pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-180">WiFi signal strength in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="74698-181">wifiVendorDriver</span><span class="sxs-lookup"><span data-stu-id="74698-181">wifiVendorDriver</span></span>|<span data-ttu-id="74698-182">String</span><span class="sxs-lookup"><span data-stu-id="74698-182">String</span></span>|<span data-ttu-id="74698-183">Nome do driver WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-183">Name of the WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="74698-184">O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="74698-184">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="74698-185">wifiVendorDriverVersion</span><span class="sxs-lookup"><span data-stu-id="74698-185">wifiVendorDriverVersion</span></span>|<span data-ttu-id="74698-186">String</span><span class="sxs-lookup"><span data-stu-id="74698-186">String</span></span>|<span data-ttu-id="74698-187">Versão do driver WiFi usado pelo ponto de extremidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="74698-187">Version of the WiFi driver used by the media endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74698-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74698-188">JSON representation</span></span>

<span data-ttu-id="74698-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74698-189">The following is a JSON representation of the resource.</span></span>

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