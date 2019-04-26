---
title: tipo de recurso windowsFirewallRule
description: Uma regra que controla o tráfego por meio do firewall do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77df7da501aee80b534accbe4c0d33dcf0e8df63
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570212"
---
# <a name="windowsfirewallrule-resource-type"></a><span data-ttu-id="2def3-103">tipo de recurso windowsFirewallRule</span><span class="sxs-lookup"><span data-stu-id="2def3-103">windowsFirewallRule resource type</span></span>

> <span data-ttu-id="2def3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2def3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2def3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2def3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2def3-106">Uma regra que controla o tráfego por meio do firewall do Windows.</span><span class="sxs-lookup"><span data-stu-id="2def3-106">A rule controlling traffic through the Windows Firewall.</span></span>

## <a name="properties"></a><span data-ttu-id="2def3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2def3-107">Properties</span></span>
|<span data-ttu-id="2def3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2def3-108">Property</span></span>|<span data-ttu-id="2def3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2def3-109">Type</span></span>|<span data-ttu-id="2def3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2def3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2def3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2def3-111">displayName</span></span>|<span data-ttu-id="2def3-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2def3-112">String</span></span>|<span data-ttu-id="2def3-113">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="2def3-113">The display name of the rule.</span></span> <span data-ttu-id="2def3-114">Não precisa ser exclusivo.</span><span class="sxs-lookup"><span data-stu-id="2def3-114">Does not need to be unique.</span></span>|
|<span data-ttu-id="2def3-115">description</span><span class="sxs-lookup"><span data-stu-id="2def3-115">description</span></span>|<span data-ttu-id="2def3-116">String</span><span class="sxs-lookup"><span data-stu-id="2def3-116">String</span></span>|<span data-ttu-id="2def3-117">A descrição da regra.</span><span class="sxs-lookup"><span data-stu-id="2def3-117">The description of the rule.</span></span>|
|<span data-ttu-id="2def3-118">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="2def3-118">packageFamilyName</span></span>|<span data-ttu-id="2def3-119">String</span><span class="sxs-lookup"><span data-stu-id="2def3-119">String</span></span>|<span data-ttu-id="2def3-120">O nome da família de pacotes de um aplicativo da Microsoft Store que é afetado pela regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="2def3-120">The package family name of a Microsoft Store application that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="2def3-121">filePath</span><span class="sxs-lookup"><span data-stu-id="2def3-121">filePath</span></span>|<span data-ttu-id="2def3-122">String</span><span class="sxs-lookup"><span data-stu-id="2def3-122">String</span></span>|<span data-ttu-id="2def3-123">O caminho completo do arquivo de um aplicativo afetado pela regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="2def3-123">The full file path of an app that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="2def3-124">serviceName</span><span class="sxs-lookup"><span data-stu-id="2def3-124">serviceName</span></span>|<span data-ttu-id="2def3-125">String</span><span class="sxs-lookup"><span data-stu-id="2def3-125">String</span></span>|<span data-ttu-id="2def3-126">O nome usado em casos em que um serviço, não um aplicativo, está enviando ou recebendo tráfego.</span><span class="sxs-lookup"><span data-stu-id="2def3-126">The name used in cases when a service, not an application, is sending or receiving traffic.</span></span>|
|<span data-ttu-id="2def3-127">RDP</span><span class="sxs-lookup"><span data-stu-id="2def3-127">protocol</span></span>|<span data-ttu-id="2def3-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2def3-128">Int32</span></span>|<span data-ttu-id="2def3-129">0-255 número que representa o protocolo IP (TCP = 6, UDP = 17).</span><span class="sxs-lookup"><span data-stu-id="2def3-129">0-255 number representing the IP protocol (TCP = 6, UDP = 17).</span></span> <span data-ttu-id="2def3-130">Se não for especificado, o padrão é ALL.</span><span class="sxs-lookup"><span data-stu-id="2def3-130">If not specified, the default is All.</span></span> <span data-ttu-id="2def3-131">Valores válidos de 0 a 255</span><span class="sxs-lookup"><span data-stu-id="2def3-131">Valid values 0 to 255</span></span>|
|<span data-ttu-id="2def3-132">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="2def3-132">localPortRanges</span></span>|<span data-ttu-id="2def3-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2def3-133">String collection</span></span>|<span data-ttu-id="2def3-134">Lista de intervalos de porta locais.</span><span class="sxs-lookup"><span data-stu-id="2def3-134">List of local port ranges.</span></span> <span data-ttu-id="2def3-135">Por exemplo, "100-120", "200", "300-320".</span><span class="sxs-lookup"><span data-stu-id="2def3-135">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="2def3-136">Se não for especificado, o padrão é ALL.</span><span class="sxs-lookup"><span data-stu-id="2def3-136">If not specified, the default is All.</span></span>|
|<span data-ttu-id="2def3-137">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="2def3-137">remotePortRanges</span></span>|<span data-ttu-id="2def3-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2def3-138">String collection</span></span>|<span data-ttu-id="2def3-139">Lista de intervalos de portas remotas.</span><span class="sxs-lookup"><span data-stu-id="2def3-139">List of remote port ranges.</span></span> <span data-ttu-id="2def3-140">Por exemplo, "100-120", "200", "300-320".</span><span class="sxs-lookup"><span data-stu-id="2def3-140">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="2def3-141">Se não for especificado, o padrão é ALL.</span><span class="sxs-lookup"><span data-stu-id="2def3-141">If not specified, the default is All.</span></span>|
|<span data-ttu-id="2def3-142">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="2def3-142">localAddressRanges</span></span>|<span data-ttu-id="2def3-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2def3-143">String collection</span></span>|<span data-ttu-id="2def3-144">Lista de endereços locais cobertos pela regra.</span><span class="sxs-lookup"><span data-stu-id="2def3-144">List of local addresses covered by the rule.</span></span> <span data-ttu-id="2def3-145">Os tokens válidos incluem:</span><span class="sxs-lookup"><span data-stu-id="2def3-145">Valid tokens include:</span></span>
- <span data-ttu-id="2def3-146">"\*" indica qualquer endereço local.</span><span class="sxs-lookup"><span data-stu-id="2def3-146">"\*" indicates any local address.</span></span> <span data-ttu-id="2def3-147">Se presente, este deve ser o único token incluído.</span><span class="sxs-lookup"><span data-stu-id="2def3-147">If present, this must be the only token included.</span></span>
- <span data-ttu-id="2def3-148">Uma sub-rede pode ser especificada usando a máscara de sub-rede ou a notação de prefixo de rede.</span><span class="sxs-lookup"><span data-stu-id="2def3-148">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="2def3-149">Se nenhuma máscara de sub-rede ou prefixo de rede for especificado, a máscara de sub-rede padrão será 255.255.255.255.</span><span class="sxs-lookup"><span data-stu-id="2def3-149">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="2def3-150">Um endereço IPv6 válido.</span><span class="sxs-lookup"><span data-stu-id="2def3-150">A valid IPv6 address.</span></span>
- <span data-ttu-id="2def3-151">Um intervalo de endereços IPv4 no formato "Iniciar endereço-end endereço" sem espaços incluídos.</span><span class="sxs-lookup"><span data-stu-id="2def3-151">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="2def3-152">Um intervalo de endereços IPv6 no formato "Iniciar endereço-end endereço" sem espaços incluídos.</span><span class="sxs-lookup"><span data-stu-id="2def3-152">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="2def3-153">O padrão é qualquer endereço. | | remoteAddressRanges | Conjunto de cadeias de caracteres | Lista de tokens que especifica os endereços remotos cobertos pela regra.</span><span class="sxs-lookup"><span data-stu-id="2def3-153">Default is any address.| |remoteAddressRanges|String collection|List of tokens specifying the remote addresses covered by the rule.</span></span> <span data-ttu-id="2def3-154">Tokens não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="2def3-154">Tokens are case insensitive.</span></span> <span data-ttu-id="2def3-155">Os tokens válidos incluem:</span><span class="sxs-lookup"><span data-stu-id="2def3-155">Valid tokens include:</span></span>
- <span data-ttu-id="2def3-156">"\*" indica qualquer endereço remoto.</span><span class="sxs-lookup"><span data-stu-id="2def3-156">"\*" indicates any remote address.</span></span> <span data-ttu-id="2def3-157">Se presente, este deve ser o único token incluído.</span><span class="sxs-lookup"><span data-stu-id="2def3-157">If present, this must be the only token included.</span></span>
- <span data-ttu-id="2def3-158">"DefaultGateway"</span><span class="sxs-lookup"><span data-stu-id="2def3-158">"Defaultgateway"</span></span>
- <span data-ttu-id="2def3-159">ESCOPO</span><span class="sxs-lookup"><span data-stu-id="2def3-159">"DHCP"</span></span>
- <span data-ttu-id="2def3-160">DNS</span><span class="sxs-lookup"><span data-stu-id="2def3-160">"DNS"</span></span>
- <span data-ttu-id="2def3-161">WINS</span><span class="sxs-lookup"><span data-stu-id="2def3-161">"WINS"</span></span>
- <span data-ttu-id="2def3-162">"Intranet" (compatível com as versões do Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="2def3-162">"Intranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="2def3-163">"RmtIntranet" (suportado nas versões do Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="2def3-163">"RmtIntranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="2def3-164">"Internet" (suportado nas versões do Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="2def3-164">"Internet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="2def3-165">"Ply2Renders" (suportado nas versões do Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="2def3-165">"Ply2Renders" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="2def3-166">"LocalSubnet" indica qualquer endereço local na sub-rede local.</span><span class="sxs-lookup"><span data-stu-id="2def3-166">"LocalSubnet" indicates any local address on the local subnet.</span></span>
- <span data-ttu-id="2def3-167">Uma sub-rede pode ser especificada usando a máscara de sub-rede ou a notação de prefixo de rede.</span><span class="sxs-lookup"><span data-stu-id="2def3-167">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="2def3-168">Se nenhuma máscara de sub-rede ou prefixo de rede for especificado, a máscara de sub-rede padrão será 255.255.255.255.</span><span class="sxs-lookup"><span data-stu-id="2def3-168">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="2def3-169">Um endereço IPv6 válido.</span><span class="sxs-lookup"><span data-stu-id="2def3-169">A valid IPv6 address.</span></span>
- <span data-ttu-id="2def3-170">Um intervalo de endereços IPv4 no formato "Iniciar endereço-end endereço" sem espaços incluídos.</span><span class="sxs-lookup"><span data-stu-id="2def3-170">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="2def3-171">Um intervalo de endereços IPv6 no formato "Iniciar endereço-end endereço" sem espaços incluídos.</span><span class="sxs-lookup"><span data-stu-id="2def3-171">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="2def3-172">O padrão é qualquer endereço. | | profileTypes | [windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)| Especifica os perfis aos quais a regra pertence.</span><span class="sxs-lookup"><span data-stu-id="2def3-172">Default is any address.| |profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Specifies the profiles to which the rule belongs.</span></span> <span data-ttu-id="2def3-173">Se não for especificado, o padrão é ALL.</span><span class="sxs-lookup"><span data-stu-id="2def3-173">If not specified, the default is All.</span></span> <span data-ttu-id="2def3-174">Os valores possíveis são `notConfigured`: `domain`, `private`, `public`,. | | ação | [stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)| A ação que a regra impõe.</span><span class="sxs-lookup"><span data-stu-id="2def3-174">Possible values are: `notConfigured`, `domain`, `private`, `public`.| |action|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|The action the rule enforces.</span></span> <span data-ttu-id="2def3-175">Se não for especificado, o padrão será permitido.</span><span class="sxs-lookup"><span data-stu-id="2def3-175">If not specified, the default is Allowed.</span></span> <span data-ttu-id="2def3-176">Os valores possíveis são `notConfigured`: `blocked`, `allowed`,. | | trafficDirection | [windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)| A direção de tráfego para a qual a regra está habilitada.</span><span class="sxs-lookup"><span data-stu-id="2def3-176">Possible values are: `notConfigured`, `blocked`, `allowed`.| |trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|The traffic direction that the rule is enabled for.</span></span> <span data-ttu-id="2def3-177">Se não for especificado, o padrão será out. Os valores possíveis são `notConfigured`: `out`, `in`,. | | Interfaces | [windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)| Os tipos de interface da regra.</span><span class="sxs-lookup"><span data-stu-id="2def3-177">If not specified, the default is Out. Possible values are: `notConfigured`, `out`, `in`.| |interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|The interface types of the rule.</span></span> <span data-ttu-id="2def3-178">Os valores possíveis são `notConfigured`: `remoteAccess`, `wireless`, `lan`,. | | localUserAuthorizations | Cadeia de caracteres | Especifica a lista de usuários locais autorizados para o contêiner de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="2def3-178">Possible values are: `notConfigured`, `remoteAccess`, `wireless`, `lan`.| |localUserAuthorizations|String|Specifies the list of authorized local users for the app container.</span></span> <span data-ttu-id="2def3-179">Esta é uma cadeia de caracteres no formato SDDL (Security Descriptor Definition Language). |</span><span class="sxs-lookup"><span data-stu-id="2def3-179">This is a string in Security Descriptor Definition Language (SDDL) format.|</span></span>

## <a name="relationships"></a><span data-ttu-id="2def3-180">Relações</span><span class="sxs-lookup"><span data-stu-id="2def3-180">Relationships</span></span>
<span data-ttu-id="2def3-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2def3-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2def3-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2def3-182">JSON Representation</span></span>
<span data-ttu-id="2def3-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2def3-183">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "localUserAuthorizations": "String"
}
```





