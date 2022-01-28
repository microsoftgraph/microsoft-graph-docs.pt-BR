---
title: tipo de recurso teamworkNetworkConfiguration
description: Representa os detalhes sobre a configuração de rede de um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5f08d5d3263917adfb9bc20ca5f964972281ecbb
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262243"
---
# <a name="teamworknetworkconfiguration-resource-type"></a>tipo de recurso teamworkNetworkConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre a configuração de rede de um dispositivo Microsoft Teams habilitado [para Microsoft Teams.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|defaultGateway|Cadeia de caracteres|O gateway padrão é o caminho usado para passar informações quando o destino é desconhecido para o dispositivo.|
|domainName|Cadeia de caracteres|O domínio de rede do dispositivo, por exemplo, contoso.com.|
|hostName|Cadeia de caracteres|O nome do dispositivo em uma rede.|
|ipAddress|Cadeia de caracteres|O endereço IP é um rótulo numérico que identifica exclusivamente todos os dispositivos conectados à Internet.|
|isDhcpEnabled|Booliano|`True` se o DHCP estiver habilitado.|
|isPCPortEnabled|Booliano|`True` se a porta do computador estiver habilitada.|
|primaryDns|Cadeia de caracteres|Um DNS primário é o primeiro ponto de contato para um dispositivo que converte o nome do host em um endereço IP.|
|secondaryDns|Cadeia de caracteres|Um DNS secundário é usado quando o DNS principal não está disponível.|
|subnetMask|String|Uma máscara de sub-rede é um número que distingue o endereço de rede e o endereço host em um endereço IP.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkNetworkConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkNetworkConfiguration",
  "defaultGateway": "String",
  "domainName": "String",
  "hostName": "String",
  "ipAddress": "String",
  "isDhcpEnabled": "Boolean",
  "isPCPortEnabled": "Boolean",
  "primaryDns": "String",
  "secondaryDns": "String",
  "subnetMask": "String"
}
```

