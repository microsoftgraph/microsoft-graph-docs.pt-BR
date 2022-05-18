---
title: Tipo de recurso unifiedRoleAssignmentSchedule
description: Representa um agendamento para operações de atribuição de função ativa por meio Azure AD Privileged Identity Management.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ab32cf141bf16b8b763c5b2d54700df7d3f3d8a9
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461622"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>Tipo de recurso unifiedRoleAssignmentSchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o agendamento de uma atribuição de função ativa por meio Azure AD Privileged Identity Management. Um **unifiedRoleAssignmentSchedule** é criado por [um unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) e é usado para criar uma instância de [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md). Esse recurso dá suporte a operações de lista e de obter para recuperar o agendamento com a finalidade de exibir atribuições atuais e futuras.

Herda de [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentSchedules](../api/rbacapplication-list-roleassignmentschedules.md)|[Coleção unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Obtenha uma lista dos [objetos unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) e suas propriedades.|
|[Obter unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Leia as propriedades e as relações de um [objeto unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) .|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Obtenha uma lista dos [objetos unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) e suas propriedades concedidas a um usuário específico.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|String|Identificador do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|assignmentType|String|Tipo da atribuição. Pode ser ou `Assigned` `Activated`.|
|createdDateTime|DateTimeOffset|Hora em que a agenda foi criada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|String|ID da roleAssignmentScheduleRequest que criou esse agendamento. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|String|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|String|O identificador exclusivo para unifiedRoleAssignmentSchedule. Chave, não anulável, somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|Membertype|String|Tipo de associação da atribuição. Pode ser `Inherited`, `Direct`ou `Group`.|
|modifiedDateTime|DateTimeOffset|Última vez em que o agendamento foi atualizado. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|String| Objectid da entidade de segurança à qual a atribuição está sendo concedida. Pode ser um grupo ou um usuário. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Suporta `$filter` (`eq`).|
|roleDefinitionId|String|ID do unifiedRoleDefinition para o que a atribuição se aplica. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Suporta `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto de agendamento da solicitação de atribuição de função.|
|status|String|Status do `roleAssignmentSchedule`. Ele pode incluir mensagens relacionadas ao estado `Provisioned`, `Revoked`como , `Pending Provisioning`e `Pending Approval`. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Suporta `$filter` (`eq`).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Se a roleAssignmentSchedule for ativada por um roleEligibilitySchedule, esse será o link para esse agendamento.|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Será preterido. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de `$expand` diretório usando ao mesmo tempo que obter a atribuição de função. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência à entidade de segurança que está obtendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade de segurança `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade que indica a roleDefinition para a atribuição. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule",
  "baseType": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentSchedule",
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
  "assignmentType": "String",
  "memberType": "String"
}
```

