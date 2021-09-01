---
title: Tipo de recurso vpnDnsRule
description: Definição da Regra DNS vpn.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1277bb254a9485bc2adc26859185adfe5d22ad5b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793870"
---
# <a name="vpndnsrule-resource-type"></a>Tipo de recurso vpnDnsRule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição da Regra DNS vpn.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|Cadeia de caracteres|Nome.|
|servers|Coleção de cadeias de caracteres|Servidores.|
|proxyServerUri|Cadeia de caracteres|Proxy Server Uri.|
|autoTrigger|Boleano|Conecte-se automaticamente à VPN quando o dispositivo se conectar a esse domínio: False padrão.|
|persistent|Boleano|Mantenha essa regra ativa mesmo quando a VPN não estiver conectada: False padrão|

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



