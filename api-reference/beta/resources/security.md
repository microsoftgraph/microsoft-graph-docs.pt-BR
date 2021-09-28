---
title: tipo de recurso de segurança
description: Para conectar produtos, serviços e parceiros de segurança da Microsoft para simplificar as operações de segurança e melhorar os recursos de proteção, detecção e resposta contra ameaças.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9f4640acb574c5099d0c1e928452099047f9cc71
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979503"
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
|securityactions|[securityAction](../resources/securityaction.md)|Ações que respondem a alertas para bloquear atividades mal-intencionadas.|
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

