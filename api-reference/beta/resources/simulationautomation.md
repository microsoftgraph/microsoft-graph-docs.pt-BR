---
title: Tipo de recurso simulationAutomation
description: Representa a automação de simulação criada para ser executado em um locatário.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 38f8bf63ef41053666a4bdd58121bd81e09fe51c
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758307"
---
# <a name="simulationautomation-resource-type"></a>Tipo de recurso simulationAutomation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a automação de simulação criada para ser executado em um locatário.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar simulationAutomations](../api/attacksimulationroot-list-simulationautomations.md)|[Coleção simulationAutomation](../resources/simulationautomation.md)|Obter uma lista dos objetos [simulationAutomation](../resources/simulationautomation.md) e suas propriedades.|
|[Listar executa](../api/simulationautomation-list-runs.md)|[Coleção simulationAutomationRun](../resources/simulationautomationrun.md)|Obter uma lista da automação de simulação de ataque executado para um locatário.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[emailIdentity](../resources/emailidentity.md)|Identidade do usuário que criou a automação de simulação de ataque.|
|createdDateTime|DateTimeOffset|Data e hora em que a automação de simulação de ataque foi criada.|
|descrição|Cadeia de caracteres|Descrição da automação de simulação de ataque.|
|displayName|Cadeia de caracteres|Nome de exibição da automação de simulação de ataque. Oferece suporte para `$filter` e `$orderby`.|
|id|Cadeia de caracteres|Identificador exclusivo para a automação de simulação de ataque.|
|lastModifiedBy|[emailIdentity](../resources/emailidentity.md)|Identidade do usuário que modificou a automação de simulação de ataque mais recentemente.|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que a automação de simulação de ataque foi modificada mais recentemente.|
|lastRunDateTime|DateTimeOffset|Data e hora da última versão da automação de simulação de ataque.|
|nextRunDateTime|DateTimeOffset|Data e hora da próxima executar a automação de simulação de ataque.|
|status|[simulationAutomationStatus](#simulationautomationstatus-values)|Status da automação de simulação de ataque. Oferece suporte para `$filter` e `$orderby`. Os valores possíveis são: `unknown`, `draft`, `notRunning`, `running`, `completed`, `unknownFutureValue`.|

### <a name="simulationautomationstatus-values"></a>valores simulationAutomationStatus

|Member|Descrição |
|:---|:---|
|desconhecido| O status da automação de simulação não está definido. |
|draft| A automação de simulação está no modo de rascunho. |
|notRunning| A automação de simulação não está em execução. |
|running| A automação de simulação está em execução. |
|completed| A automação de simulação foi concluída. |
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|runs|[Coleção simulationAutomationRun](../resources/simulationautomationrun.md)|Uma coleção de simulações de automação é executado. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.simulationAutomation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationAutomation",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastRunDateTime": "String (timestamp)",
  "nextRunDateTime": "String (timestamp)",
  "status": "String"
}
```

