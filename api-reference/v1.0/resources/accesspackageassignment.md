---
title: Tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bd2493b96043286c4585bec60b5af6f47130cf77
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651320"
---
# <a name="accesspackageassignment-resource-type"></a>Tipo de recurso accessPackageAssignment

Namespace: microsoft.graph

No [Azure AD Entitlement Management](entitlementmanagement-overview.md), uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.  Por exemplo, uma atribuição de pacote de acesso pode dizer que a usuária Alice recebeu acesso por meio do pacote de acesso Vendas do período de janeiro de 2019 a julho de 2019.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackageAssignments](../api/entitlementmanagement-list-assignments.md)|[Coleção accessPackageAssignment](accesspackageassignment.md)|Recupere uma lista de **objetos accessPackageAssignment.** |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)|Recupere a lista de **objetos accessPackageAssignment** filtrados no usuário de entrada.|

> [!NOTE]
> Para criar ou remover uma atribuição de pacote de acesso para um usuário, use o método [create a accessPackageAssignmentRequest.](../api/entitlementmanagement-post-assignmentrequests.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|expiredDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|id|String|Somente leitura.|
|Cronograma|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Quando a atribuição de acesso estiver no local. Somente leitura.|
|state|accessPackageAssignmentState|O estado da atribuição do pacote de acesso. Os valores possíveis são: `delivering`, `partiallyDelivered`, `delivered`, `expired`, `deliveryFailed`, `unknownFutureValue`. Somente leitura. Suporta `$filter` (`eq`).|
|status|String|Mais informações sobre o ciclo de vida da atribuição.  Os valores possíveis `Delivering` `Delivered` incluem , `NearExpiry1DayNotificationTriggered` , ou `ExpiredNotificationTriggered` .  Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackage|[accessPackage](accesspackage.md)|Somente leitura. Anulável. Suporta `$filter` ( ) na propriedade `eq` **id** `$expand` e parâmetros de consulta.|
|destino|[accessPackageSubject](accesspackagesubject.md)|O assunto da atribuição do pacote de acesso. Somente leitura. Anulável. Suporta o `$expand`. Suporta `$filter` ( ) em `eq` **objectId**.|

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


