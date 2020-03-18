---
title: tipo de recurso appleVpnAlwaysOnConfiguration
description: Configuração de VPN AlwaysOn para MacOS e iOS IKEv2
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 10facf24c8fd56786c2706e1fa8ee999f48e2ed7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796065"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a><span data-ttu-id="037a0-103">tipo de recurso appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="037a0-103">appleVpnAlwaysOnConfiguration resource type</span></span>

> <span data-ttu-id="037a0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="037a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="037a0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="037a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="037a0-106">Configuração de VPN AlwaysOn para MacOS e iOS IKEv2</span><span class="sxs-lookup"><span data-stu-id="037a0-106">Always On VPN configuration for MacOS and iOS IKEv2</span></span>

## <a name="properties"></a><span data-ttu-id="037a0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="037a0-107">Properties</span></span>
|<span data-ttu-id="037a0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="037a0-108">Property</span></span>|<span data-ttu-id="037a0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="037a0-109">Type</span></span>|<span data-ttu-id="037a0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="037a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="037a0-111">tunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="037a0-111">tunnelConfiguration</span></span>|[<span data-ttu-id="037a0-112">vpnTunnelConfigurationType</span><span class="sxs-lookup"><span data-stu-id="037a0-112">vpnTunnelConfigurationType</span></span>](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|<span data-ttu-id="037a0-113">Determina a quais conexões a configuração de túnel específica se aplica.</span><span class="sxs-lookup"><span data-stu-id="037a0-113">Determines what connections the specific tunnel configuration applies to.</span></span> <span data-ttu-id="037a0-114">Os valores possíveis são: `wifiAndCellular`, `cellular`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="037a0-114">Possible values are: `wifiAndCellular`, `cellular`, `wifi`.</span></span>|
|<span data-ttu-id="037a0-115">userToggleEnabled</span><span class="sxs-lookup"><span data-stu-id="037a0-115">userToggleEnabled</span></span>|<span data-ttu-id="037a0-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="037a0-116">Boolean</span></span>|<span data-ttu-id="037a0-117">Permitir que o usuário alterne a configuração VPN usando a interface do usuário</span><span class="sxs-lookup"><span data-stu-id="037a0-117">Allow the user to toggle the VPN configuration using the UI</span></span>|
|<span data-ttu-id="037a0-118">voicemailExceptionAction</span><span class="sxs-lookup"><span data-stu-id="037a0-118">voicemailExceptionAction</span></span>|[<span data-ttu-id="037a0-119">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="037a0-119">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="037a0-120">Determine se o serviço de caixa postal será isento da conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="037a0-120">Determine whether voicemail service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="037a0-121">Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="037a0-121">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="037a0-122">airPrintExceptionAction</span><span class="sxs-lookup"><span data-stu-id="037a0-122">airPrintExceptionAction</span></span>|[<span data-ttu-id="037a0-123">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="037a0-123">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="037a0-124">Determine se o serviço de impressão do servidor será isento da conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="037a0-124">Determine whether AirPrint service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="037a0-125">Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="037a0-125">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="037a0-126">cellularExceptionAction</span><span class="sxs-lookup"><span data-stu-id="037a0-126">cellularExceptionAction</span></span>|[<span data-ttu-id="037a0-127">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="037a0-127">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="037a0-128">Determine se o serviço celular será isento da conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="037a0-128">Determine whether Cellular service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="037a0-129">Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="037a0-129">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="037a0-130">allowAllCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="037a0-130">allowAllCaptiveNetworkPlugins</span></span>|<span data-ttu-id="037a0-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="037a0-131">Boolean</span></span>|<span data-ttu-id="037a0-132">Especifica se o tráfego de todos os plugins de rede prisioneiros deve ser permitido fora da VPN</span><span class="sxs-lookup"><span data-stu-id="037a0-132">Specifies whether traffic from all captive network plugins should be allowed outside the vpn</span></span>|
|<span data-ttu-id="037a0-133">allowedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="037a0-133">allowedCaptiveNetworkPlugins</span></span>|[<span data-ttu-id="037a0-134">specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="037a0-134">specifiedCaptiveNetworkPlugins</span></span>](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|<span data-ttu-id="037a0-135">Determina se todos, alguns ou nenhum aplicativo de rede cativo não nativo são permitidos</span><span class="sxs-lookup"><span data-stu-id="037a0-135">Determines whether all, some, or no non-native captive networking apps are allowed</span></span>|
|<span data-ttu-id="037a0-136">allowCaptiveWebSheet</span><span class="sxs-lookup"><span data-stu-id="037a0-136">allowCaptiveWebSheet</span></span>|<span data-ttu-id="037a0-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="037a0-137">Boolean</span></span>|<span data-ttu-id="037a0-138">Determina se o tráfego do aplicativo Websheet é permitido fora da VPN</span><span class="sxs-lookup"><span data-stu-id="037a0-138">Determines whether traffic from the Websheet app is allowed outside of the VPN</span></span>|
|<span data-ttu-id="037a0-139">natKeepAliveIntervalInSeconds</span><span class="sxs-lookup"><span data-stu-id="037a0-139">natKeepAliveIntervalInSeconds</span></span>|<span data-ttu-id="037a0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="037a0-140">Int32</span></span>|<span data-ttu-id="037a0-141">Especifica com que frequência, em segundos, enviar um pacote de KeepAlive de conversão de endereços de rede através da VPN</span><span class="sxs-lookup"><span data-stu-id="037a0-141">Specifies how often in seconds to send a network address translation keepalive package through the VPN</span></span>|
|<span data-ttu-id="037a0-142">natKeepAliveOffloadEnable</span><span class="sxs-lookup"><span data-stu-id="037a0-142">natKeepAliveOffloadEnable</span></span>|<span data-ttu-id="037a0-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="037a0-143">Boolean</span></span>|<span data-ttu-id="037a0-144">Habilitar descarregamento de hardware de sinais de KeepAlive de NAT quando o dispositivo estiver suspenso</span><span class="sxs-lookup"><span data-stu-id="037a0-144">Enable hardware offloading of NAT keepalive signals when the device is asleep</span></span>|

## <a name="relationships"></a><span data-ttu-id="037a0-145">Relações</span><span class="sxs-lookup"><span data-stu-id="037a0-145">Relationships</span></span>
<span data-ttu-id="037a0-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="037a0-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="037a0-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="037a0-147">JSON Representation</span></span>
<span data-ttu-id="037a0-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="037a0-148">Here is a JSON representation of the resource.</span></span>
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



