---
title: Tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2b063bf4cc0e0d53c970a53d27578cb5dceb0a8e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242201"
---
# <a name="accesspackageassignment-resource-type"></a>Tipo de recurso accessPackageAssignment

Namespace: microsoft.graph

No [Azure AD Entitlement Management](entitlementmanagement-root.md), uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.  Por exemplo, uma atribuição de pacote de acesso pode dizer que a usuária Alice recebeu acesso por meio do pacote de acesso Vendas do período de janeiro de 2019 a julho de 2019.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackageAssignments](../api/entitlementmanagement-list-assignments.md)|[Coleção accessPackageAssignment](accesspackageassignment.md)|Recupere uma lista de **objetos accessPackageAssignment.** |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)|Recupere a lista de **objetos accessPackageAssignment** filtrados no usuário de entrada.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|expiredDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|id|String|Somente leitura.|
|Cronograma|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Quando a atribuição de acesso estiver no local. Somente leitura.|
|state|accessPackageAssignmentState|O estado da atribuição do pacote de acesso. Os valores possíveis são: `delivering`, `partiallyDelivered`, `delivered`, `expired`, `deliveryFailed`, `unknownFutureValue`. Apenas leitura.|
|status|Cadeia de caracteres|Mais informações sobre o ciclo de vida da atribuição.  Os valores possíveis `Delivering` `Delivered` incluem , `NearExpiry1DayNotificationTriggered` , ou `ExpiredNotificationTriggered` .  Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackage|[accessPackage](accesspackage.md)|Somente leitura. Anulável.|
|destino|[accessPackageSubject](accesspackagesubject.md)|O assunto da atribuição do pacote de acesso. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "String (identifier)",
  "state": "String",
  "status": "String",
  "expiredDateTime": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


