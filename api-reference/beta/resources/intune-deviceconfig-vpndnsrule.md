---
title: Tipo de recurso vpnDnsRule
description: Definição da Regra DNS vpn.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e11233ceb703e9b0a587c55d304cbd74d8eeb712710f33336acbb62575473742
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54173125"
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
|proxyServerUri|Cadeia de caracteres|Proxy Server Uri.|
|autoTrigger|Boolean|Conecte-se automaticamente à VPN quando o dispositivo se conectar a esse domínio: False padrão.|
|persistent|Boolean|Mantenha essa regra ativa mesmo quando a VPN não estiver conectada: False padrão|

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




