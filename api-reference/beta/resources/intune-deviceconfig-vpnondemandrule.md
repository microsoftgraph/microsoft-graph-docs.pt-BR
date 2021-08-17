---
title: Tipo de recurso vpnOnDemandRule
description: Definição de regra de vpn sob demanda.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 71bfbf09f9fcb8de63956855ec3c13fed60a2d604d1a3b1601c1b2f6007e8867
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54131175"
---
# <a name="vpnondemandrule-resource-type"></a>Tipo de recurso vpnOnDemandRule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de regra de vpn sob demanda.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ssids|String collection|Identificadores de conjunto de serviços de rede (SSIDs).|
|dnsSearchDomains|String collection|Domínios de Pesquisa DNS.|
|probeUrl|Cadeia de caracteres|Uma URL para sondar. Se essa URL for buscada com êxito (retornando um código de status HTTP 200) sem redirecionamento, essa regra corresponde.|
|ação|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Ação. Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Ação de domínio (aplicável somente quando Ação é avaliar conexão). Os valores possíveis são: `connectIfNeeded` e `neverConnect`.|
|domínios|String collection|Domínios (aplicável somente quando Ação é avaliar conexão).|
|probeRequiredUrl|Cadeia de caracteres|Url Necessária da Sonda (Somente aplicável quando Action é avaliar a conexão e DomainAction é conectar-se, se necessário).|

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




