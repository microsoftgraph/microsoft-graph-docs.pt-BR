---
title: tipo de recurso de vpnTrafficRule
description: Definição de regra de tráfego de VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b28d26356eea113f267c4eb0499f9600671f114
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415282"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="c81cf-103">tipo de recurso de vpnTrafficRule</span><span class="sxs-lookup"><span data-stu-id="c81cf-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="c81cf-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c81cf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c81cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c81cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c81cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c81cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c81cf-107">Definição de regra de tráfego de VPN.</span><span class="sxs-lookup"><span data-stu-id="c81cf-107">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c81cf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c81cf-108">Properties</span></span>
|<span data-ttu-id="c81cf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c81cf-109">Property</span></span>|<span data-ttu-id="c81cf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c81cf-110">Type</span></span>|<span data-ttu-id="c81cf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c81cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c81cf-112">name</span><span class="sxs-lookup"><span data-stu-id="c81cf-112">name</span></span>|<span data-ttu-id="c81cf-113">String</span><span class="sxs-lookup"><span data-stu-id="c81cf-113">String</span></span>|<span data-ttu-id="c81cf-114">Nome.</span><span class="sxs-lookup"><span data-stu-id="c81cf-114">Name.</span></span>|
|<span data-ttu-id="c81cf-115">protocolos</span><span class="sxs-lookup"><span data-stu-id="c81cf-115">protocols</span></span>|<span data-ttu-id="c81cf-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c81cf-116">Int32</span></span>|<span data-ttu-id="c81cf-117">Protocolos (0 a 255).</span><span class="sxs-lookup"><span data-stu-id="c81cf-117">Protocols (0-255).</span></span> <span data-ttu-id="c81cf-118">Valores válidos 0 a 255</span><span class="sxs-lookup"><span data-stu-id="c81cf-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="c81cf-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="c81cf-119">localPortRanges</span></span>|<span data-ttu-id="c81cf-120">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="c81cf-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="c81cf-121">Intervalo de porta local pode ser definido somente quando for de protocolo TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="c81cf-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="c81cf-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c81cf-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c81cf-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="c81cf-123">remotePortRanges</span></span>|<span data-ttu-id="c81cf-124">coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="c81cf-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="c81cf-125">Intervalo de porta remota pode ser definido somente quando for de protocolo TCP ou UDP (6 ou 17).</span><span class="sxs-lookup"><span data-stu-id="c81cf-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="c81cf-126">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c81cf-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c81cf-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="c81cf-127">localAddressRanges</span></span>|<span data-ttu-id="c81cf-128">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="c81cf-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="c81cf-129">Intervalo de endereços locais.</span><span class="sxs-lookup"><span data-stu-id="c81cf-129">Local address range.</span></span> <span data-ttu-id="c81cf-130">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c81cf-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c81cf-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="c81cf-131">remoteAddressRanges</span></span>|<span data-ttu-id="c81cf-132">coleção [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="c81cf-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="c81cf-133">Intervalo de endereços remoto.</span><span class="sxs-lookup"><span data-stu-id="c81cf-133">Remote address range.</span></span> <span data-ttu-id="c81cf-134">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c81cf-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c81cf-135">appId</span><span class="sxs-lookup"><span data-stu-id="c81cf-135">appId</span></span>|<span data-ttu-id="c81cf-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c81cf-136">String</span></span>|<span data-ttu-id="c81cf-137">Identificador de aplicativo, se esta regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c81cf-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="c81cf-138">tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="c81cf-138">appType</span></span>|[<span data-ttu-id="c81cf-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="c81cf-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="c81cf-140">Tipo de aplicativo, se esta regra de tráfego é disparada por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c81cf-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="c81cf-141">Os valores possíveis são: `none`, `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="c81cf-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="c81cf-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="c81cf-142">routingPolicyType</span></span>|[<span data-ttu-id="c81cf-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="c81cf-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="c81cf-144">Quando app disparada, indica se deseja habilitar o túnel em divisão ao longo desta rota.</span><span class="sxs-lookup"><span data-stu-id="c81cf-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="c81cf-145">Os valores possíveis são: `none`, `splitTunnel`, `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="c81cf-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="c81cf-146">declarações</span><span class="sxs-lookup"><span data-stu-id="c81cf-146">claims</span></span>|<span data-ttu-id="c81cf-147">String</span><span class="sxs-lookup"><span data-stu-id="c81cf-147">String</span></span>|<span data-ttu-id="c81cf-148">Declarações associadas a essa regra de tráfego.</span><span class="sxs-lookup"><span data-stu-id="c81cf-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c81cf-149">Relações</span><span class="sxs-lookup"><span data-stu-id="c81cf-149">Relationships</span></span>
<span data-ttu-id="c81cf-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c81cf-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c81cf-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c81cf-151">JSON Representation</span></span>
<span data-ttu-id="c81cf-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c81cf-152">Here is a JSON representation of the resource.</span></span>
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




