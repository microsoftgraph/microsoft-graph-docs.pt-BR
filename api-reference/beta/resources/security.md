---
title: tipo de recurso de segurança
description: Conecta produtos, serviços e parceiros de segurança da Microsoft para simplificar as operações de segurança e melhorar os recursos de proteção, detecção e resposta a ameaças.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c7342f83c64b895b08a66429e0e20ab2cd7b5960
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856285"
---
# <a name="security-resource-type"></a>tipo de recurso de segurança

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Conecta produtos, serviços e parceiros de segurança da Microsoft para simplificar as operações de segurança e melhorar os recursos de proteção, detecção e resposta a ameaças.

## <a name="methods"></a>Métodos
Nenhum.

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|alertas|conjunto [alerta](../resources/alert.md) |Notificações de problemas de segurança suspeitos ou potenciais no locatário de um cliente.|
|attackSimulation|[attackSimulationRoot](../resources/attacksimulationroot.md)|Fornece aos locatários a capacidade de iniciar um ataque de phishing simulado e realista e aprender com ele.|
|securityactions|[Securityaction](../resources/securityaction.md)|Ações que respondem a alertas para bloquear atividades mal-intencionadas.|
|tiindicators|[Coleção tiIndicator](../resources/tiindicator.md)|Indicadores de ameaça enviados à Microsoft que identificam atividades mal-intencionadas.|
|threatSubmission|[security.threatSubmission](../resources/security-threatsubmission.md)|Um envio de ameaça enviado à Microsoft; por exemplo, uma ameaça suspeita de email, ameaça de URL ou ameaça de arquivo.|

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

