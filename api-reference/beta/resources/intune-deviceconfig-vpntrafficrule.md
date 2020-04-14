---
title: tipo de recurso vpnTrafficRule
description: Definição de regra de tráfego VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f1e87a3076c53d4d95b60f0ac884cc825da6a85
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43359377"
---
# <a name="vpntrafficrule-resource-type"></a>tipo de recurso vpnTrafficRule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de regra de tráfego VPN.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|Tdomínio.|
|protocolos|Int32|Protocolos (0-255). Valores válidos de 0 a 255|
|localPortRanges|coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)|O intervalo de porta local só pode ser definido quando o protocolo é TCP ou UDP (6 ou 17). Esta coleção pode conter um máximo de 500 elementos.|
|remotePortRanges|coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)|O intervalo de porta remoto só pode ser definido quando o protocolo é TCP ou UDP (6 ou 17). Esta coleção pode conter um máximo de 500 elementos.|
|localAddressRanges|coleção [iPv4Range](../resources/intune-shared-ipv4range.md)|Intervalo de endereços local. Esta coleção pode conter um máximo de 500 elementos.|
|remoteAddressRanges|coleção [iPv4Range](../resources/intune-shared-ipv4range.md)|Intervalo de endereços remoto. Esta coleção pode conter um máximo de 500 elementos.|
|appId|String|Identificador de aplicativo, se essa regra de tráfego é disparada por um aplicativo.|
|appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|Tipo de aplicativo, se essa regra de tráfego é disparada por um aplicativo. Os valores possíveis são: `none`, `desktop`, `universal`.|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|Quando o aplicativo é acionado, indica se deseja habilitar o túnel de divisão ao longo desta rota. Os valores possíveis são: `none`, `splitTunnel`, `forceTunnel`.|
|afirma|String|Declarações associadas a esta regra de tráfego.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
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



