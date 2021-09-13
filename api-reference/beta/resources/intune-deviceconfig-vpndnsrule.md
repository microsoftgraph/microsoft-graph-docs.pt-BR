---
title: Tipo de recurso vpnDnsRule
description: Definição da Regra DNS vpn.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e034016fe3a6eff5d84db1421e5e6e80d1f70be3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081210"
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
|servers|String collection|Servidores.|
|proxyServerUri|String|Proxy Server Uri.|
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



