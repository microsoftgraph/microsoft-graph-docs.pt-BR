---
title: tipo de recurso vpnOnDemandRule
description: Definição de regra VPN sob demanda.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1bccd015e45291b344e7c77df4ac5c0a0af07d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161583"
---
# <a name="vpnondemandrule-resource-type"></a>tipo de recurso vpnOnDemandRule

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de regra VPN sob demanda.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|SSIDs|Coleção de cadeias de caracteres|Identificadores de conjuntos de serviços de rede (SSIDs).|
|dnsSearchDomains|Coleção de cadeias de caracteres|Domínios de pesquisa de DNS.|
|probeUrl|String|Uma URL para sondar. Se essa URL for obtida com êxito (retornando um código de status HTTP 200) sem redirecionamento, essa regra será correspondente.|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Ação. Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|domainaction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Ação de domínio (aplicável somente quando a ação é avaliar conexão). Os valores possíveis são: `connectIfNeeded` e `neverConnect`.|
|domínio|Coleção de cadeias de caracteres|Domains (só é aplicável quando Action é Evaluate Connection).|
|probeRequiredUrl|String|A URL obrigatória da sonda (aplicável somente quando Action é Evaluate Connection e domainaction é conectada se necessário).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```




