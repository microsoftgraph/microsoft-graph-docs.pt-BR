---
title: tipo de recurso de vpnTrafficRule
description: Definição de regra de tráfego de VPN.
ms.openlocfilehash: 564528cf0c0ae39785a2cc43dc800d8dbdf7d285
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034970"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="0c044-103">tipo de recurso de vpnTrafficRule</span><span class="sxs-lookup"><span data-stu-id="0c044-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="0c044-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c044-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c044-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c044-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c044-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0c044-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c044-107">Definição de regra de tráfego de VPN.</span><span class="sxs-lookup"><span data-stu-id="0c044-107">VPN Traffic Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="0c044-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c044-108">Properties</span></span>
|<span data-ttu-id="0c044-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c044-109">Property</span></span>|<span data-ttu-id="0c044-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c044-110">Type</span></span>|<span data-ttu-id="0c044-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c044-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c044-112">name</span><span class="sxs-lookup"><span data-stu-id="0c044-112">name</span></span>|<span data-ttu-id="0c044-113">String</span><span class="sxs-lookup"><span data-stu-id="0c044-113">String</span></span>|<span data-ttu-id="0c044-114">Nome.</span><span class="sxs-lookup"><span data-stu-id="0c044-114">Name.</span></span>|
|<span data-ttu-id="0c044-115">protocolos</span><span class="sxs-lookup"><span data-stu-id="0c044-115">protocols</span></span>|<span data-ttu-id="0c044-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0c044-116">Int32</span></span>|<span data-ttu-id="0c044-117">Protocolos (0 a 255).</span><span class="sxs-lookup"><span data-stu-id="0c044-117">Protocols (0-255).</span></span> <span data-ttu-id="0c044-118">Valores válidos 0 a 255</span><span class="sxs-lookup"><span data-stu-id="0c044-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="0c044-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="0c044-119">localPortRanges</span></span>|<span data-ttu-id="0c044-120">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="0c044-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="0c044-121">Intervalo de porta local pode ser definido somente quando for de protocolo TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="0c044-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="0c044-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0c044-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0c044-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="0c044-123">remotePortRanges</span></span>|<span data-ttu-id="0c044-124">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="0c044-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="0c044-125">Intervalo de porta remota pode ser definido somente quando for de protocolo TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="0c044-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="0c044-126">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0c044-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0c044-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="0c044-127">localAddressRanges</span></span>|<span data-ttu-id="0c044-128">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="0c044-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="0c044-129">Intervalo de endereços locais.</span><span class="sxs-lookup"><span data-stu-id="0c044-129">Local address range.</span></span> <span data-ttu-id="0c044-130">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0c044-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0c044-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="0c044-131">remoteAddressRanges</span></span>|<span data-ttu-id="0c044-132">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="0c044-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="0c044-133">Intervalo de endereços remoto.</span><span class="sxs-lookup"><span data-stu-id="0c044-133">Remote address range.</span></span> <span data-ttu-id="0c044-134">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0c044-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0c044-135">appId</span><span class="sxs-lookup"><span data-stu-id="0c044-135">appId</span></span>|<span data-ttu-id="0c044-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c044-136">String</span></span>|<span data-ttu-id="0c044-137">Identificador de aplicativo, se esta regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c044-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="0c044-138">tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c044-138">appType</span></span>|[<span data-ttu-id="0c044-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="0c044-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="0c044-140">Tipo de aplicativo, se esta regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c044-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="0c044-141">Os valores possíveis são: `none`, `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="0c044-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="0c044-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="0c044-142">routingPolicyType</span></span>|[<span data-ttu-id="0c044-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="0c044-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="0c044-144">Quando app disparada, indica se deseja habilitar o túnel em divisão ao longo desta rota.</span><span class="sxs-lookup"><span data-stu-id="0c044-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="0c044-145">Os valores possíveis são: `none`, `splitTunnel`, `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="0c044-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="0c044-146">declarações</span><span class="sxs-lookup"><span data-stu-id="0c044-146">claims</span></span>|<span data-ttu-id="0c044-147">String</span><span class="sxs-lookup"><span data-stu-id="0c044-147">String</span></span>|<span data-ttu-id="0c044-148">Declarações associadas a essa regra de tráfego.</span><span class="sxs-lookup"><span data-stu-id="0c044-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c044-149">Relações</span><span class="sxs-lookup"><span data-stu-id="0c044-149">Relationships</span></span>
<span data-ttu-id="0c044-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c044-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c044-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c044-151">JSON Representation</span></span>
<span data-ttu-id="0c044-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c044-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": 1024,
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "remoteAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "appId": "String",
  "appType": "String",
  "routingPolicyType": "String",
  "claims": "String"
}
```





