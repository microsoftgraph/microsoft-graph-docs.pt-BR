---
title: tipo de recurso appleVpnAlwaysOnConfiguration
description: Configuração de VPN AlwaysOn para MacOS e iOS IKEv2
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5bf41b54e64f31cd02a362f7abfcbb2fc12fb434
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042537"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a><span data-ttu-id="d145a-103">tipo de recurso appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d145a-103">appleVpnAlwaysOnConfiguration resource type</span></span>

<span data-ttu-id="d145a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d145a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d145a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d145a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d145a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d145a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d145a-107">Configuração de VPN AlwaysOn para MacOS e iOS IKEv2</span><span class="sxs-lookup"><span data-stu-id="d145a-107">Always On VPN configuration for MacOS and iOS IKEv2</span></span>

## <a name="properties"></a><span data-ttu-id="d145a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d145a-108">Properties</span></span>
|<span data-ttu-id="d145a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d145a-109">Property</span></span>|<span data-ttu-id="d145a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d145a-110">Type</span></span>|<span data-ttu-id="d145a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d145a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d145a-112">tunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="d145a-112">tunnelConfiguration</span></span>|[<span data-ttu-id="d145a-113">vpnTunnelConfigurationType</span><span class="sxs-lookup"><span data-stu-id="d145a-113">vpnTunnelConfigurationType</span></span>](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|<span data-ttu-id="d145a-114">Determina a quais conexões a configuração de túnel específica se aplica.</span><span class="sxs-lookup"><span data-stu-id="d145a-114">Determines what connections the specific tunnel configuration applies to.</span></span> <span data-ttu-id="d145a-115">Os valores possíveis são: `wifiAndCellular`, `cellular`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="d145a-115">Possible values are: `wifiAndCellular`, `cellular`, `wifi`.</span></span>|
|<span data-ttu-id="d145a-116">userToggleEnabled</span><span class="sxs-lookup"><span data-stu-id="d145a-116">userToggleEnabled</span></span>|<span data-ttu-id="d145a-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="d145a-117">Boolean</span></span>|<span data-ttu-id="d145a-118">Permitir que o usuário alterne a configuração VPN usando a interface do usuário</span><span class="sxs-lookup"><span data-stu-id="d145a-118">Allow the user to toggle the VPN configuration using the UI</span></span>|
|<span data-ttu-id="d145a-119">voicemailExceptionAction</span><span class="sxs-lookup"><span data-stu-id="d145a-119">voicemailExceptionAction</span></span>|[<span data-ttu-id="d145a-120">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="d145a-120">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="d145a-121">Determine se o serviço de caixa postal será isento da conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="d145a-121">Determine whether voicemail service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="d145a-122">Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="d145a-122">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="d145a-123">airPrintExceptionAction</span><span class="sxs-lookup"><span data-stu-id="d145a-123">airPrintExceptionAction</span></span>|[<span data-ttu-id="d145a-124">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="d145a-124">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="d145a-125">Determine se o serviço de impressão do servidor será isento da conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="d145a-125">Determine whether AirPrint service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="d145a-126">Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="d145a-126">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="d145a-127">cellularExceptionAction</span><span class="sxs-lookup"><span data-stu-id="d145a-127">cellularExceptionAction</span></span>|[<span data-ttu-id="d145a-128">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="d145a-128">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="d145a-129">Determine se o serviço celular será isento da conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="d145a-129">Determine whether Cellular service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="d145a-130">Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="d145a-130">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="d145a-131">allowAllCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="d145a-131">allowAllCaptiveNetworkPlugins</span></span>|<span data-ttu-id="d145a-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="d145a-132">Boolean</span></span>|<span data-ttu-id="d145a-133">Especifica se o tráfego de todos os plugins de rede prisioneiros deve ser permitido fora da VPN</span><span class="sxs-lookup"><span data-stu-id="d145a-133">Specifies whether traffic from all captive network plugins should be allowed outside the vpn</span></span>|
|<span data-ttu-id="d145a-134">allowedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="d145a-134">allowedCaptiveNetworkPlugins</span></span>|[<span data-ttu-id="d145a-135">specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="d145a-135">specifiedCaptiveNetworkPlugins</span></span>](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|<span data-ttu-id="d145a-136">Determina se todos, alguns ou nenhum aplicativo de rede cativo não nativo são permitidos</span><span class="sxs-lookup"><span data-stu-id="d145a-136">Determines whether all, some, or no non-native captive networking apps are allowed</span></span>|
|<span data-ttu-id="d145a-137">allowCaptiveWebSheet</span><span class="sxs-lookup"><span data-stu-id="d145a-137">allowCaptiveWebSheet</span></span>|<span data-ttu-id="d145a-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="d145a-138">Boolean</span></span>|<span data-ttu-id="d145a-139">Determina se o tráfego do aplicativo Websheet é permitido fora da VPN</span><span class="sxs-lookup"><span data-stu-id="d145a-139">Determines whether traffic from the Websheet app is allowed outside of the VPN</span></span>|
|<span data-ttu-id="d145a-140">natKeepAliveIntervalInSeconds</span><span class="sxs-lookup"><span data-stu-id="d145a-140">natKeepAliveIntervalInSeconds</span></span>|<span data-ttu-id="d145a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d145a-141">Int32</span></span>|<span data-ttu-id="d145a-142">Especifica com que frequência, em segundos, enviar um pacote de KeepAlive de conversão de endereços de rede através da VPN</span><span class="sxs-lookup"><span data-stu-id="d145a-142">Specifies how often in seconds to send a network address translation keepalive package through the VPN</span></span>|
|<span data-ttu-id="d145a-143">natKeepAliveOffloadEnable</span><span class="sxs-lookup"><span data-stu-id="d145a-143">natKeepAliveOffloadEnable</span></span>|<span data-ttu-id="d145a-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="d145a-144">Boolean</span></span>|<span data-ttu-id="d145a-145">Habilitar descarregamento de hardware de sinais de KeepAlive de NAT quando o dispositivo estiver suspenso</span><span class="sxs-lookup"><span data-stu-id="d145a-145">Enable hardware offloading of NAT keepalive signals when the device is asleep</span></span>|

## <a name="relationships"></a><span data-ttu-id="d145a-146">Relações</span><span class="sxs-lookup"><span data-stu-id="d145a-146">Relationships</span></span>
<span data-ttu-id="d145a-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d145a-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d145a-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d145a-148">JSON Representation</span></span>
<span data-ttu-id="d145a-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d145a-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnAlwaysOnConfiguration",
  "tunnelConfiguration": "String",
  "userToggleEnabled": true,
  "voicemailExceptionAction": "String",
  "airPrintExceptionAction": "String",
  "cellularExceptionAction": "String",
  "allowAllCaptiveNetworkPlugins": true,
  "allowedCaptiveNetworkPlugins": {
    "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
    "allowedBundleIdentifiers": [
      "String"
    ]
  },
  "allowCaptiveWebSheet": true,
  "natKeepAliveIntervalInSeconds": 1024,
  "natKeepAliveOffloadEnable": true
}
```






