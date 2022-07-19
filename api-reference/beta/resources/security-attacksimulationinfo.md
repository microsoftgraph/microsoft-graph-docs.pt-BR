---
title: Tipo de recurso attackSimulationInfo
description: Representa informações de simulação de ataque de envio de ameaças
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d7caee88f2d097c344c9fdcb3ba64767893e0276
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856482"
---
# <a name="attacksimulationinfo-resource-type"></a>Tipo de recurso attackSimulationInfo

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de simulação de ataque do envio de ameaças. Se um email fosse um email de simulação de ataque, o envio de ameaças de email conteria informações de simulação de ataque correspondentes.

## <a name="properties"></a>Propriedades
| Propriedade              | Tipo           | Descrição                          |
|:----------------------|:---------------|:-------------------------------------|
| attackSimDateTime     | DateTimeOffset | Especifica a data e hora da simulação de ataque.   |
| attackSimDurationTime | Duração       | Especifica a duração (no tempo) da simulação de ataque  |
| attackSimId           | Guid           | Especifica a ID da atividade para a simulação de ataque. |
| attackSimUserId       | Cadeia de caracteres         | Especifica a ID de usuário do usuário que recebeu o email de simulação de ataque   |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.attackSimulationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.attackSimulationInfo",
  "attackSimId": "Guid",
  "attackSimDateTime": "String (timestamp)",
  "attackSimDurationTime": "String (duration)",
  "attackSimUserId": "String"
}
```

