---
title: tipo de recurso vpnTrafficRule
description: Definição de regra de tráfego VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff432af56f41ab92abfff8b168dabdac15d6dee1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724541"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="a8e65-103">tipo de recurso vpnTrafficRule</span><span class="sxs-lookup"><span data-stu-id="a8e65-103">vpnTrafficRule resource type</span></span>

<span data-ttu-id="a8e65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8e65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8e65-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8e65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8e65-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8e65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8e65-107">Definição de regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="a8e65-107">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a8e65-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8e65-108">Properties</span></span>
|<span data-ttu-id="a8e65-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8e65-109">Property</span></span>|<span data-ttu-id="a8e65-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8e65-110">Type</span></span>|<span data-ttu-id="a8e65-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e65-112">nome</span><span class="sxs-lookup"><span data-stu-id="a8e65-112">name</span></span>|<span data-ttu-id="a8e65-113">String</span><span class="sxs-lookup"><span data-stu-id="a8e65-113">String</span></span>|<span data-ttu-id="a8e65-114">Tdomínio.</span><span class="sxs-lookup"><span data-stu-id="a8e65-114">Name.</span></span>|
|<span data-ttu-id="a8e65-115">protocolos</span><span class="sxs-lookup"><span data-stu-id="a8e65-115">protocols</span></span>|<span data-ttu-id="a8e65-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a8e65-116">Int32</span></span>|<span data-ttu-id="a8e65-117">Protocolos (0-255).</span><span class="sxs-lookup"><span data-stu-id="a8e65-117">Protocols (0-255).</span></span> <span data-ttu-id="a8e65-118">Valores válidos de 0 a 255</span><span class="sxs-lookup"><span data-stu-id="a8e65-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="a8e65-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="a8e65-119">localPortRanges</span></span>|<span data-ttu-id="a8e65-120">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="a8e65-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="a8e65-121">O intervalo de porta local só pode ser definido quando o protocolo é TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="a8e65-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="a8e65-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a8e65-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a8e65-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="a8e65-123">remotePortRanges</span></span>|<span data-ttu-id="a8e65-124">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="a8e65-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="a8e65-125">O intervalo de porta remoto só pode ser definido quando o protocolo é TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="a8e65-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="a8e65-126">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a8e65-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a8e65-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="a8e65-127">localAddressRanges</span></span>|<span data-ttu-id="a8e65-128">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="a8e65-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="a8e65-129">Intervalo de endereços local.</span><span class="sxs-lookup"><span data-stu-id="a8e65-129">Local address range.</span></span> <span data-ttu-id="a8e65-130">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a8e65-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a8e65-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="a8e65-131">remoteAddressRanges</span></span>|<span data-ttu-id="a8e65-132">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="a8e65-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="a8e65-133">Intervalo de endereços remoto.</span><span class="sxs-lookup"><span data-stu-id="a8e65-133">Remote address range.</span></span> <span data-ttu-id="a8e65-134">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a8e65-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a8e65-135">appId</span><span class="sxs-lookup"><span data-stu-id="a8e65-135">appId</span></span>|<span data-ttu-id="a8e65-136">String</span><span class="sxs-lookup"><span data-stu-id="a8e65-136">String</span></span>|<span data-ttu-id="a8e65-137">Identificador de aplicativo, se essa regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8e65-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="a8e65-138">appType</span><span class="sxs-lookup"><span data-stu-id="a8e65-138">appType</span></span>|[<span data-ttu-id="a8e65-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="a8e65-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="a8e65-140">Tipo de aplicativo, se essa regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8e65-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="a8e65-141">Os valores possíveis são: `none`, `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="a8e65-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="a8e65-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="a8e65-142">routingPolicyType</span></span>|[<span data-ttu-id="a8e65-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="a8e65-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="a8e65-144">Quando o aplicativo é acionado, indica se deseja habilitar o túnel de divisão ao longo desta rota.</span><span class="sxs-lookup"><span data-stu-id="a8e65-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="a8e65-145">Os valores possíveis são: `none`, `splitTunnel`, `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="a8e65-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="a8e65-146">afirma</span><span class="sxs-lookup"><span data-stu-id="a8e65-146">claims</span></span>|<span data-ttu-id="a8e65-147">String</span><span class="sxs-lookup"><span data-stu-id="a8e65-147">String</span></span>|<span data-ttu-id="a8e65-148">Declarações associadas a esta regra de tráfego.</span><span class="sxs-lookup"><span data-stu-id="a8e65-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8e65-149">Relações</span><span class="sxs-lookup"><span data-stu-id="a8e65-149">Relationships</span></span>
<span data-ttu-id="a8e65-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8e65-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8e65-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8e65-151">JSON Representation</span></span>
<span data-ttu-id="a8e65-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8e65-152">Here is a JSON representation of the resource.</span></span>
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





