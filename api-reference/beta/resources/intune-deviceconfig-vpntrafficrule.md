---
title: tipo de recurso vpnTrafficRule
description: Definição de regra de tráfego VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd004341928260187518966e2356f59faff57898
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139939"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="fe2b9-103">tipo de recurso vpnTrafficRule</span><span class="sxs-lookup"><span data-stu-id="fe2b9-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="fe2b9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe2b9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe2b9-106">Definição de regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-106">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="fe2b9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe2b9-107">Properties</span></span>
|<span data-ttu-id="fe2b9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe2b9-108">Property</span></span>|<span data-ttu-id="fe2b9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe2b9-109">Type</span></span>|<span data-ttu-id="fe2b9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe2b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe2b9-111">name</span><span class="sxs-lookup"><span data-stu-id="fe2b9-111">name</span></span>|<span data-ttu-id="fe2b9-112">String</span><span class="sxs-lookup"><span data-stu-id="fe2b9-112">String</span></span>|<span data-ttu-id="fe2b9-113">Tdomínio.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-113">Name.</span></span>|
|<span data-ttu-id="fe2b9-114">protocolos</span><span class="sxs-lookup"><span data-stu-id="fe2b9-114">protocols</span></span>|<span data-ttu-id="fe2b9-115">Int32</span><span class="sxs-lookup"><span data-stu-id="fe2b9-115">Int32</span></span>|<span data-ttu-id="fe2b9-116">Protocolos (0-255).</span><span class="sxs-lookup"><span data-stu-id="fe2b9-116">Protocols (0-255).</span></span> <span data-ttu-id="fe2b9-117">Valores válidos de 0 a 255</span><span class="sxs-lookup"><span data-stu-id="fe2b9-117">Valid values 0 to 255</span></span>|
|<span data-ttu-id="fe2b9-118">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="fe2b9-118">localPortRanges</span></span>|<span data-ttu-id="fe2b9-119">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="fe2b9-119">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="fe2b9-120">O intervalo de porta local só pode ser definido quando o protocolo é TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="fe2b9-120">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="fe2b9-121">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fe2b9-122">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="fe2b9-122">remotePortRanges</span></span>|<span data-ttu-id="fe2b9-123">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="fe2b9-123">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="fe2b9-124">O intervalo de porta remoto só pode ser definido quando o protocolo é TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="fe2b9-124">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="fe2b9-125">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-125">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fe2b9-126">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="fe2b9-126">localAddressRanges</span></span>|<span data-ttu-id="fe2b9-127">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="fe2b9-127">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="fe2b9-128">Intervalo de endereços local.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-128">Local address range.</span></span> <span data-ttu-id="fe2b9-129">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fe2b9-130">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="fe2b9-130">remoteAddressRanges</span></span>|<span data-ttu-id="fe2b9-131">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="fe2b9-131">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="fe2b9-132">Intervalo de endereços remoto.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-132">Remote address range.</span></span> <span data-ttu-id="fe2b9-133">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-133">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fe2b9-134">appId</span><span class="sxs-lookup"><span data-stu-id="fe2b9-134">appId</span></span>|<span data-ttu-id="fe2b9-135">String</span><span class="sxs-lookup"><span data-stu-id="fe2b9-135">String</span></span>|<span data-ttu-id="fe2b9-136">Identificador de aplicativo, se essa regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-136">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="fe2b9-137">appType</span><span class="sxs-lookup"><span data-stu-id="fe2b9-137">appType</span></span>|[<span data-ttu-id="fe2b9-138">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="fe2b9-138">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="fe2b9-139">Tipo de aplicativo, se essa regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-139">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="fe2b9-140">Os valores possíveis são: `none`, `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-140">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="fe2b9-141">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="fe2b9-141">routingPolicyType</span></span>|[<span data-ttu-id="fe2b9-142">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="fe2b9-142">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="fe2b9-143">Quando o aplicativo é acionado, indica se deseja habilitar o túnel de divisão ao longo desta rota.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-143">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="fe2b9-144">Os valores possíveis são: `none`, `splitTunnel`, `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-144">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="fe2b9-145">afirma</span><span class="sxs-lookup"><span data-stu-id="fe2b9-145">claims</span></span>|<span data-ttu-id="fe2b9-146">String</span><span class="sxs-lookup"><span data-stu-id="fe2b9-146">String</span></span>|<span data-ttu-id="fe2b9-147">Declarações associadas a esta regra de tráfego.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-147">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe2b9-148">Relações</span><span class="sxs-lookup"><span data-stu-id="fe2b9-148">Relationships</span></span>
<span data-ttu-id="fe2b9-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe2b9-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe2b9-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe2b9-150">JSON Representation</span></span>
<span data-ttu-id="fe2b9-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe2b9-151">Here is a JSON representation of the resource.</span></span>
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




