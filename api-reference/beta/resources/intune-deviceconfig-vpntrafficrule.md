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
# <a name="vpntrafficrule-resource-type"></a>tipo de recurso de vpnTrafficRule

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Definição de regra de tráfego de VPN.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|name|String|Nome.|
|protocolos|Int32|Protocolos (0 a 255). Valores válidos 0 a 255|
|localPortRanges|coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)|Intervalo de porta local pode ser definido somente quando for de protocolo TCP ou UDP (6 ou 17). Esta coleção pode conter um máximo de 500 elementos.|
|remotePortRanges|coleção [numberRange](../resources/intune-deviceconfig-numberrange.md)|Intervalo de porta remota pode ser definido somente quando for de protocolo TCP ou UDP (6 ou 17). Esta coleção pode conter um máximo de 500 elementos.|
|localAddressRanges|coleção [iPv4Range](../resources/intune-shared-ipv4range.md)|Intervalo de endereços locais. Esta coleção pode conter um máximo de 500 elementos.|
|remoteAddressRanges|coleção [iPv4Range](../resources/intune-shared-ipv4range.md)|Intervalo de endereços remoto. Esta coleção pode conter um máximo de 500 elementos.|
|appId|Cadeia de caracteres|Identificador de aplicativo, se esta regra de tráfego é disparada por um aplicativo.|
|tipo de aplicativo|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|Tipo de aplicativo, se esta regra de tráfego é disparada por um aplicativo. Os valores possíveis são: `none`, `desktop`, `universal`.|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|Quando app disparada, indica se deseja habilitar o túnel em divisão ao longo desta rota. Os valores possíveis são: `none`, `splitTunnel`, `forceTunnel`.|
|declarações|String|Declarações associadas a essa regra de tráfego.|

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




