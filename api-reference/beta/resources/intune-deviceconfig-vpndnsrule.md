---
title: tipo de recurso vpnDnsRule
description: Definição de regra DNS de VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ffc8c01aadfe77bd3d92d9f7618a5846cf7c855
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787387"
---
# <a name="vpndnsrule-resource-type"></a>tipo de recurso vpnDnsRule

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de regra DNS de VPN.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|Tdomínio.|
|servidores|Coleção de cadeias de caracteres|Servidores.|
|proxyServerUri|String|URI do servidor proxy.|
|Gatilho autotrigger|Boolean|Conectar-se automaticamente à VPN quando o dispositivo se conectar a este domínio: padrão false.|
|persistente|Boolean|Manter esta regra ativa mesmo quando a VPN não estiver conectada: false padrão|

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



