---
title: tipo de recurso appleVpnAlwaysOnConfiguration
description: Configuração de VPN AlwaysOn para MacOS e iOS IKEv2
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3b963556254766cff951faeed707e5c6aceed05f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527151"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a><span data-ttu-id="41421-103">tipo de recurso appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="41421-103">appleVpnAlwaysOnConfiguration resource type</span></span>

<span data-ttu-id="41421-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="41421-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41421-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41421-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41421-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41421-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41421-107">Configuração de VPN AlwaysOn para MacOS e iOS IKEv2</span><span class="sxs-lookup"><span data-stu-id="41421-107">Always On VPN configuration for MacOS and iOS IKEv2</span></span>

## <a name="properties"></a><span data-ttu-id="41421-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41421-108">Properties</span></span>
|<span data-ttu-id="41421-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41421-109">Property</span></span>|<span data-ttu-id="41421-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="41421-110">Type</span></span>|<span data-ttu-id="41421-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41421-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41421-112">tunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="41421-112">tunnelConfiguration</span></span>|[<span data-ttu-id="41421-113">vpnTunnelConfigurationType</span><span class="sxs-lookup"><span data-stu-id="41421-113">vpnTunnelConfigurationType</span></span>](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|<span data-ttu-id="41421-114">Determina a quais conexões a configuração de túnel específica se aplica.</span><span class="sxs-lookup"><span data-stu-id="41421-114">Determines what connections the specific tunnel configuration applies to.</span></span> <span data-ttu-id="41421-115">Os valores possíveis são: `wifiAndCellular`, `cellular`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="41421-115">Possible values are: `wifiAndCellular`, `cellular`, `wifi`.</span></span>|
|<span data-ttu-id="41421-116">userToggleEnabled</span><span class="sxs-lookup"><span data-stu-id="41421-116">userToggleEnabled</span></span>|<span data-ttu-id="41421-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="41421-117">Boolean</span></span>|<span data-ttu-id="41421-118">Permitir que o usuário alterne a configuração VPN usando a interface do usuário</span><span class="sxs-lookup"><span data-stu-id="41421-118">Allow the user to toggle the VPN configuration using the UI</span></span>|
|<span data-ttu-id="41421-119">voicemailExceptionAction</span><span class="sxs-lookup"><span data-stu-id="41421-119">voicemailExceptionAction</span></span>|[<span data-ttu-id="41421-120">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="41421-120">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="41421-121">Determine se o serviço de caixa postal será isento da conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="41421-121">Determine whether voicemail service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="41421-122">Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="41421-122">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="41421-123">airPrintExceptionAction</span><span class="sxs-lookup"><span data-stu-id="41421-123">airPrintExceptionAction</span></span>|[<span data-ttu-id="41421-124">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="41421-124">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="41421-125">Determine se o serviço de impressão do servidor será isento da conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="41421-125">Determine whether AirPrint service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="41421-126">Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="41421-126">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="41421-127">cellularExceptionAction</span><span class="sxs-lookup"><span data-stu-id="41421-127">cellularExceptionAction</span></span>|[<span data-ttu-id="41421-128">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="41421-128">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="41421-129">Determine se o serviço celular será isento da conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="41421-129">Determine whether Cellular service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="41421-130">Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="41421-130">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="41421-131">allowAllCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="41421-131">allowAllCaptiveNetworkPlugins</span></span>|<span data-ttu-id="41421-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="41421-132">Boolean</span></span>|<span data-ttu-id="41421-133">Especifica se o tráfego de todos os plugins de rede prisioneiros deve ser permitido fora da VPN</span><span class="sxs-lookup"><span data-stu-id="41421-133">Specifies whether traffic from all captive network plugins should be allowed outside the vpn</span></span>|
|<span data-ttu-id="41421-134">allowedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="41421-134">allowedCaptiveNetworkPlugins</span></span>|[<span data-ttu-id="41421-135">specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="41421-135">specifiedCaptiveNetworkPlugins</span></span>](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|<span data-ttu-id="41421-136">Determina se todos, alguns ou nenhum aplicativo de rede cativo não nativo são permitidos</span><span class="sxs-lookup"><span data-stu-id="41421-136">Determines whether all, some, or no non-native captive networking apps are allowed</span></span>|
|<span data-ttu-id="41421-137">allowCaptiveWebSheet</span><span class="sxs-lookup"><span data-stu-id="41421-137">allowCaptiveWebSheet</span></span>|<span data-ttu-id="41421-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="41421-138">Boolean</span></span>|<span data-ttu-id="41421-139">Determina se o tráfego do aplicativo Websheet é permitido fora da VPN</span><span class="sxs-lookup"><span data-stu-id="41421-139">Determines whether traffic from the Websheet app is allowed outside of the VPN</span></span>|
|<span data-ttu-id="41421-140">natKeepAliveIntervalInSeconds</span><span class="sxs-lookup"><span data-stu-id="41421-140">natKeepAliveIntervalInSeconds</span></span>|<span data-ttu-id="41421-141">Int32</span><span class="sxs-lookup"><span data-stu-id="41421-141">Int32</span></span>|<span data-ttu-id="41421-142">Especifica com que frequência, em segundos, enviar um pacote de KeepAlive de conversão de endereços de rede através da VPN</span><span class="sxs-lookup"><span data-stu-id="41421-142">Specifies how often in seconds to send a network address translation keepalive package through the VPN</span></span>|
|<span data-ttu-id="41421-143">natKeepAliveOffloadEnable</span><span class="sxs-lookup"><span data-stu-id="41421-143">natKeepAliveOffloadEnable</span></span>|<span data-ttu-id="41421-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="41421-144">Boolean</span></span>|<span data-ttu-id="41421-145">Habilitar descarregamento de hardware de sinais de KeepAlive de NAT quando o dispositivo estiver suspenso</span><span class="sxs-lookup"><span data-stu-id="41421-145">Enable hardware offloading of NAT keepalive signals when the device is asleep</span></span>|

## <a name="relationships"></a><span data-ttu-id="41421-146">Relações</span><span class="sxs-lookup"><span data-stu-id="41421-146">Relationships</span></span>
<span data-ttu-id="41421-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41421-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41421-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41421-148">JSON Representation</span></span>
<span data-ttu-id="41421-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41421-149">Here is a JSON representation of the resource.</span></span>
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



