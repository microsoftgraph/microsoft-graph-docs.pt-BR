---
title: tipo de recurso vpnDnsRule
description: Definição de regra DNS de VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bd40af2d8aa9a2ecb036f60e86d4056727b03a2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299706"
---
# <a name="vpndnsrule-resource-type"></a>tipo de recurso vpnDnsRule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de regra DNS de VPN.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|Tdomínio.|
|servidores|Coleção de cadeias de caracteres|Servidores.|
|proxyServerUri|String|URI do servidor proxy.|
|Gatilho autotrigger|Booliano|Conectar-se automaticamente à VPN quando o dispositivo se conectar a este domínio: padrão false.|
|persistente|Booliano|Manter esta regra ativa mesmo quando a VPN não estiver conectada: false padrão|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```




