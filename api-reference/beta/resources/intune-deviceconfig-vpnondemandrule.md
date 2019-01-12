---
title: tipo de recurso de vpnOnDemandRule
description: Definição de regra de sob demanda de VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43908a55ff43c533d02ace629a80b96dc09c10ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955412"
---
# <a name="vpnondemandrule-resource-type"></a>tipo de recurso de vpnOnDemandRule

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Definição de regra de sob demanda de VPN.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|SSIDs|String collection|Identificadores (SSIDs) do conjunto de serviço de rede.|
|dnsSearchDomains|String collection|Domínios de pesquisa DNS.|
|probeUrl|String|Uma URL para teste. Se essa URL é com êxito procurada (retornando um código de status HTTP 200) sem redirecionamento, correspondentes a esta regra.|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Ação. Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Ação de domínio (aplicável somente quando a ação é avaliar a conexão). Os valores possíveis são: `connectIfNeeded` e `neverConnect`.|
|domínios|String collection|Domínios (aplicáveis somente quando a ação é avaliar a conexão).|
|probeRequiredUrl|String|Investigue obrigatório Url (aplicável somente quando a ação é avaliar a conexão e DomainAction é conectar, se necessário).|

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





