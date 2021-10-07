---
title: tipo de recurso de segurança
description: Para conectar produtos, serviços e parceiros de segurança da Microsoft para simplificar as operações de segurança e melhorar os recursos de proteção, detecção e resposta contra ameaças.
author: preetikr
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 494fc483645fe0a5422013556b2a44cc21aaadaf
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220763"
---
# <a name="security-resource-type"></a>tipo de recurso de segurança

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Para conectar produtos, serviços e parceiros de segurança da Microsoft para simplificar as operações de segurança e melhorar os recursos de proteção, detecção e resposta contra ameaças.

## <a name="methods"></a>Métodos
Nenhum.

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|alertas|conjunto [alerta](../resources/alert.md) |Notificações para problemas de segurança suspeitos ou potenciais no locatário de um cliente.|
|attackSimulation|[attackSimulationRoot](../resources/attacksimulationroot.md)|Fornece aos locatários a capacidade de iniciar um ataque de phishing simulado e realista e aprender com ele.|
|incidentes | [coleção incident](incident.md) | Uma coleção de incidentes em Microsoft 365 Defender, cada um deles é um conjunto de alertas correlacionados e metadados associados que reflete a história de um ataque.|
|secureScores | [Coleção secureScore](securescores.md) | Medidas da postura de segurança dos locatários para ajudar a protegê-los contra ameaças. |
|securityactions|[Coleção securityAction](../resources/securityaction.md)|Ações que respondem a alertas para bloquear atividades mal-intencionadas.|
|tiindicators|[Coleção tiIndicator](../resources/tiindicator.md)|Indicadores de ameaça enviados à Microsoft que identificam atividades mal-intencionadas.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security"
}
```

