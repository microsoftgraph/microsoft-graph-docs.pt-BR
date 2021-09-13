---
title: Tipo de recurso vpnTrafficRule
description: Definição da Regra de Tráfego vpn.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5a9986231c0f4d974a02ed8eaaaf44a032ac341
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59027061"
---
# <a name="vpntrafficrule-resource-type"></a>Tipo de recurso vpnTrafficRule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição da Regra de Tráfego vpn.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|Cadeia de caracteres|Nome.|
|protocolos|Int32|Protocolos (0-255). Valores válidos de 0 a 255|
|localPortRanges|[coleção numberRange](../resources/intune-deviceconfig-numberrange.md)|O intervalo de portas local só pode ser definido quando o protocolo for TCP ou UDP (6 ou 17). Esta coleção pode conter um máximo de 500 elementos.|
|remotePortRanges|[coleção numberRange](../resources/intune-deviceconfig-numberrange.md)|O intervalo de portas remotas só pode ser definido quando o protocolo é TCP ou UDP (6 ou 17). Esta coleção pode conter um máximo de 500 elementos.|
|localAddressRanges|[Coleção iPv4Range](../resources/intune-shared-ipv4range.md)|Intervalo de endereços local. Esta coleção pode conter um máximo de 500 elementos.|
|remoteAddressRanges|[Coleção iPv4Range](../resources/intune-shared-ipv4range.md)|Intervalo de endereços remoto. Esta coleção pode conter um máximo de 500 elementos.|
|appId|String|Identificador de aplicativo, se essa regra de tráfego for disparada por um aplicativo.|
|appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|Tipo de aplicativo, se essa regra de tráfego for disparada por um aplicativo. Os valores possíveis são: `none`, `desktop`, `universal`.|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|Quando o aplicativo é acionado, indica se é possível habilitar o túnel dividido ao longo dessa rota. Os valores possíveis são: `none`, `splitTunnel`, `forceTunnel`.|
|claims|String|Declarações associadas a essa regra de tráfego.|

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



