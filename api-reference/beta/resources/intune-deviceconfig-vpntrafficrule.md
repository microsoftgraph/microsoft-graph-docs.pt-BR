---
title: tipo de recurso vpnTrafficRule
description: Definição de regra de tráfego VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9eecec1ca70b897f88003b884ea3e5e3a024a7b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529274"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="a4107-103">tipo de recurso vpnTrafficRule</span><span class="sxs-lookup"><span data-stu-id="a4107-103">vpnTrafficRule resource type</span></span>

<span data-ttu-id="a4107-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a4107-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4107-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4107-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4107-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4107-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4107-107">Definição de regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="a4107-107">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a4107-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4107-108">Properties</span></span>
|<span data-ttu-id="a4107-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4107-109">Property</span></span>|<span data-ttu-id="a4107-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4107-110">Type</span></span>|<span data-ttu-id="a4107-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4107-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4107-112">nome</span><span class="sxs-lookup"><span data-stu-id="a4107-112">name</span></span>|<span data-ttu-id="a4107-113">String</span><span class="sxs-lookup"><span data-stu-id="a4107-113">String</span></span>|<span data-ttu-id="a4107-114">Tdomínio.</span><span class="sxs-lookup"><span data-stu-id="a4107-114">Name.</span></span>|
|<span data-ttu-id="a4107-115">protocolos</span><span class="sxs-lookup"><span data-stu-id="a4107-115">protocols</span></span>|<span data-ttu-id="a4107-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a4107-116">Int32</span></span>|<span data-ttu-id="a4107-117">Protocolos (0-255).</span><span class="sxs-lookup"><span data-stu-id="a4107-117">Protocols (0-255).</span></span> <span data-ttu-id="a4107-118">Valores válidos de 0 a 255</span><span class="sxs-lookup"><span data-stu-id="a4107-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="a4107-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="a4107-119">localPortRanges</span></span>|<span data-ttu-id="a4107-120">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="a4107-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="a4107-121">O intervalo de porta local só pode ser definido quando o protocolo é TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="a4107-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="a4107-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a4107-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a4107-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="a4107-123">remotePortRanges</span></span>|<span data-ttu-id="a4107-124">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="a4107-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="a4107-125">O intervalo de porta remoto só pode ser definido quando o protocolo é TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="a4107-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="a4107-126">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a4107-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a4107-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="a4107-127">localAddressRanges</span></span>|<span data-ttu-id="a4107-128">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="a4107-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="a4107-129">Intervalo de endereços local.</span><span class="sxs-lookup"><span data-stu-id="a4107-129">Local address range.</span></span> <span data-ttu-id="a4107-130">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a4107-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a4107-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="a4107-131">remoteAddressRanges</span></span>|<span data-ttu-id="a4107-132">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="a4107-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="a4107-133">Intervalo de endereços remoto.</span><span class="sxs-lookup"><span data-stu-id="a4107-133">Remote address range.</span></span> <span data-ttu-id="a4107-134">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a4107-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a4107-135">appId</span><span class="sxs-lookup"><span data-stu-id="a4107-135">appId</span></span>|<span data-ttu-id="a4107-136">String</span><span class="sxs-lookup"><span data-stu-id="a4107-136">String</span></span>|<span data-ttu-id="a4107-137">Identificador de aplicativo, se essa regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a4107-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="a4107-138">appType</span><span class="sxs-lookup"><span data-stu-id="a4107-138">appType</span></span>|[<span data-ttu-id="a4107-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="a4107-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="a4107-140">Tipo de aplicativo, se essa regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a4107-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="a4107-141">Os valores possíveis são: `none`, `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="a4107-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="a4107-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="a4107-142">routingPolicyType</span></span>|[<span data-ttu-id="a4107-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="a4107-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="a4107-144">Quando o aplicativo é acionado, indica se deseja habilitar o túnel de divisão ao longo desta rota.</span><span class="sxs-lookup"><span data-stu-id="a4107-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="a4107-145">Os valores possíveis são: `none`, `splitTunnel`, `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="a4107-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="a4107-146">afirma</span><span class="sxs-lookup"><span data-stu-id="a4107-146">claims</span></span>|<span data-ttu-id="a4107-147">String</span><span class="sxs-lookup"><span data-stu-id="a4107-147">String</span></span>|<span data-ttu-id="a4107-148">Declarações associadas a esta regra de tráfego.</span><span class="sxs-lookup"><span data-stu-id="a4107-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4107-149">Relações</span><span class="sxs-lookup"><span data-stu-id="a4107-149">Relationships</span></span>
<span data-ttu-id="a4107-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4107-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4107-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4107-151">JSON Representation</span></span>
<span data-ttu-id="a4107-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4107-152">Here is a JSON representation of the resource.</span></span>
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



