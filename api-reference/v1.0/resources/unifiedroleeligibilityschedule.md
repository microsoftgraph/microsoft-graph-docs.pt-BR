---
title: Tipo de recurso unifiedRoleEligibilitySchedule
description: Representa um agendamento para uma qualificação de função em seu locatário.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3bf5929c146cf054022ef33b2be73db323a0f13c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133882"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>Tipo de recurso unifiedRoleEligibilitySchedule

Namespace: microsoft.graph

Representa um agendamento para uma elegibilidade de função em seu locatário e é usado para criar uma instância de [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md).


Herda de [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilitySchedules](../api/rbacapplication-list-roleeligibilityschedules.md)|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Obtenha os agendamentos para operações de qualificação de função.|
|[Obter unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Recupere o agendamento de uma operação de qualificação de função.|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Recupere os agendamentos de eligibilidades de função para as quais o usuário conectado é a entidade de segurança.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando a elegibilidade de função está no escopo de um aplicativo. O escopo de uma elegibilidade de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|createdDateTime|DateTimeOffset|Quando a agenda foi criada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|Cadeia de caracteres|Identificador do objeto por meio do qual essa agenda foi criada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da elegibilidade da função. O escopo de uma elegibilidade de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de agendamento. Herdado da [entidade](../resources/entity.md). Suporta `$filter` (`eq`).|
|Membertype|Cadeia de caracteres|Como a elegibilidade de função é herdada. Pode ser `Inherited`, `Direct`ou `Group`. Isso pode implicar ainda se **o unifiedRoleEligibilitySchedule** pode ser gerenciado pelo chamador. Suporta `$filter` (`eq`, `ne`).|
|modifiedDateTime|DateTimeOffset|Quando a agenda foi modificada pela última vez. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança qualificada para uma função. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Suporta `$filter` (`eq`, `ne`).|
|roleDefinitionId|Cadeia de caracteres|Identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) para o qual uma entidade de segurança está qualificada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O período de qualificação da função.|
|status|Cadeia de caracteres|O status da solicitação de qualificação de função. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Os valores possíveis são: `Canceled`, `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, , `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`, , `Revoked`e `ScheduleCreated`. Não anulável. Suporta `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando a elegibilidade de função está no escopo de um aplicativo. Anulável. Suporta o `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto de diretório que é o escopo da qualificação de função. Somente leitura. Oferece suporte para `$expand`.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade de segurança qualificada para uma função por meio da solicitação. Suporta o `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Informações detalhadas para o objeto roleDefinition referenciado por meio da **propriedade roleDefinitionId** . Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilitySchedule",
  "baseType": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilitySchedule",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "memberType": "String"
}
```

