---
title: Tipo de recurso unifiedRoleEligibilitySchedule
description: Representa um agendamento para operações de atribuição de função qualificadas por meio Azure AD Privileged Identity Management.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e581e021df25547b276609d4075c162fcc5fed3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439918"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>Tipo de recurso unifiedRoleEligibilitySchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um agendamento para uma elegibilidade de função em seu locatário e é usado para criar uma instância de [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md).

Herda de [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilitySchedules](../api/rbacapplication-list-roleeligibilityschedules.md)|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Obtenha os agendamentos para operações de qualificação de função.|
|[Obter unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Recupere o agendamento de uma operação de qualificação de função.|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Recupere os agendamentos de eligibilidades de função para as quais o usuário conectado é a entidade de segurança.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|createdDateTime|DateTimeOffset|Hora em que a agenda foi criada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|Cadeia de caracteres|Identificador da roleEligibilityScheduleRequest que criou esse agendamento. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleEligibilitySchedule. Chave, não anulável, somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Suporta `$filter` (`eq`).|
|Membertype|Cadeia de caracteres|Tipo de associação da atribuição qualificada. Pode ser `Inherited`, `Direct`ou `Group`. Suporta `$filter` (`eq`).|
|modifiedDateTime|DateTimeOffset|Última vez em que o agendamento foi atualizado. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|Cadeia de caracteres| Identificador da entidade de segurança à qual a atribuição qualificada está sendo concedida. Pode ser um grupo ou um usuário. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Suporta `$filter` (`eq`).|
|roleDefinitionId|String|Identificador do unifiedRoleDefinition para o que a atribuição se aplica. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Suporta `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto de agendamento da solicitação de atribuição de função qualificada.|
|status|Cadeia de caracteres|Status do `roleEligibilitySchedule`. Ele pode incluir mensagens relacionadas ao estado `Provisioned`, `Revoked`como , `Pending Provisioning`e `Pending Approval`. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Suporta `$filter` (`eq`).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência ao objeto de diretório que é o escopo da atribuição qualificada. Fornecido para que os chamadores possam obter o objeto de `$expand` diretório usando ao mesmo tempo que obter a atribuição de função qualificada. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência à entidade de segurança que está obtendo uma atribuição de função qualificada por meio da solicitação. Fornecido para que os chamadores possam obter a entidade `$expand` de segurança usando ao mesmo tempo que obter a atribuição de função qualificada. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade que indica a roleDefinition para a qual a atribuição qualificada é. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função qualificada. roleDefinition.Id será expandido automaticamente. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

