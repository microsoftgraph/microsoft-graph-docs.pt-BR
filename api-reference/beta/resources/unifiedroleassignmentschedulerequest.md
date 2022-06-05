---
title: Tipo de recurso unifiedRoleAssignmentScheduleRequest
description: No PIM, representa uma solicitação para uma atribuição de função ativa a uma entidade de segurança. A atribuição de função pode ser permanentemente ativa com ou sem uma data de expiração ou temporariamente ativa após a ativação de uma atribuição qualificada.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f7483c7ce6a78654906c9122b936742d1992d324
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900391"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>Tipo de recurso unifiedRoleAssignmentScheduleRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

I PIM, representa uma solicitação para uma atribuição de função ativa para uma entidade de segurança. A atribuição de função pode ser permanentemente ativa com ou sem uma data de expiração ou temporariamente ativa após a ativação de uma atribuição qualificada. Herda da [solicitação](../resources/request.md).

Para obter mais informações sobre cenários de PIM que você pode definir por meio do tipo de recurso **unifiedRoleAssignmentScheduleRequest** , consulte Visão geral do gerenciamento de funções por meio da [API pim (privileged identity management](privilegedidentitymanagementv3-overview.md)).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentScheduleRequests](../api/rbacapplication-list-roleassignmentschedulerequests.md)|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)| Recupere as solicitações de atribuições de função ativas feitas por meio do [objeto unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) .|
|[Criar unifiedRoleAssignmentScheduleRequest](../api/rbacapplication-post-roleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Crie uma solicitação para uma atribuição de função ativa e persistente ou ative, desative, estenda ou renove uma atribuição de função qualificada.|
|[Obter unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Recupere uma solicitação para uma atribuição de função ativa feita por meio do [objeto unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) .|
|[cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)|Nenhum| Cancele uma solicitação para uma atribuição de função ativa. |
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)| Recupere as solicitações de atribuições de função ativas para uma entidade de segurança específica.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|Cadeia de Caracteres|Representa o tipo da operação na solicitação de atribuição de função. Os valores possíveis são `adminAssign`, `adminUpdate`, `adminRemove`, `selfActivate`, `selfDeactivate`, `adminExtend`, `adminRenew`, `selfExtend`, `selfRenew`, `unknownFutureValue`. <br/><ul><li>`adminAssign`: para que os administradores atribuam funções a entidades de segurança.</li><li>`adminRemove`: para que os administradores removam entidades de segurança das funções.</li><li> `adminUpdate`: para que os administradores alterem as atribuições de função existentes.</li><li>`adminExtend`: para que os administradores estendam as atribuições de expiração.</li><li>`adminRenew`: para que os administradores renovem atribuições expiradas.</li><li>`selfActivate`: para entidades de segurança ativarem suas atribuições.</li><li>`selfDeactivate`: para entidades de segurança desativarem suas atribuições ativas.</li><li>`selfExtend`: para que as entidades de segurança solicitem a extensão de suas atribuições de expiração.</li><li>`selfRenew`: para que as entidades de segurança solicitem a renovação de suas atribuições expiradas.</li></ul>|
|approvalId|Cadeia de Caracteres|O identificador da aprovação da solicitação. Herdado da [solicitação](../resources/request.md).|
|appScopeId|Cadeia de Caracteres|Identificador do escopo específico do aplicativo quando a atribuição está no escopo de um aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação. Herdado da [solicitação](../resources/request.md).|
|createdBy|[identitySet](../resources/identityset.md)|A entidade de segurança que criou essa solicitação. Herdado da [solicitação](../resources/request.md). Somente leitura. Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|createdDateTime|DateTimeOffset|A data de criação da solicitação. Herdado da [solicitação](../resources/request.md). Somente leitura.|
|Customdata|Cadeia de Caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado. Herdado da [solicitação](../resources/request.md).|
|directoryScopeId|Cadeia de Caracteres|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|id|String|O identificador exclusivo do **objeto unifiedRoleAssignmentScheduleRequest** . Chave, não anulável, somente leitura. Herdado da [entidade](../resources/entity.md). Suporta `$filter` (`eq`, `ne`).|
|isValidationOnly|Booliano|Determina se a chamada é uma validação ou uma chamada real. Defina essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|Justificação|Cadeia de Caracteres|Uma mensagem fornecida por usuários e administradores ao criar eles criam o objeto **unifiedRoleAssignmentScheduleRequest** .|
|principalId|Cadeia de Caracteres|Identificador da entidade de segurança que recebeu a atribuição. Suporta `$filter` (`eq`, `ne`).|
|roleDefinitionId|Cadeia de Caracteres|Identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) que está sendo atribuído à entidade de segurança. Suporta `$filter` (`eq`, `ne`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O período da atribuição de função. No momento, não há suporte para agendamentos recorrentes.|
|status|String|O status da solicitação de atribuição de função. Herdado da [solicitação](../resources/request.md). Somente leitura. Suporta `$filter` (`eq`, `ne`).|
|targetScheduleId|Cadeia de Caracteres|Identificador do objeto de agendamento que está vinculado à solicitação de atribuição. Suporta `$filter` (`eq`, `ne`).|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Detalhes do tíquete vinculados à solicitação de atribuição de função, incluindo detalhes do número do tíquete e do sistema de tíquetes.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Se a solicitação for de um administrador qualificado para ativar uma função, esse parâmetro mostrará a atribuição qualificada relacionada para essa ativação. Caso contrário, é `null`. Suporta o `$expand`.|
|appScope|[appScope](../resources/appscope.md)| Propriedade somente leitura com detalhes do escopo específico do aplicativo quando a atribuição está no escopo de um aplicativo. Anulável. Suporta o `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto de diretório que é o escopo da atribuição. Somente leitura. Oferece suporte para `$expand`.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade de segurança que está obtendo uma atribuição de função por meio da solicitação. Suporta o `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Informações detalhadas para [o objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) referenciado por meio da **propriedade roleDefinitionId** . Suporta o `$expand`.|
|targetSchedule|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|O agendamento para uma atribuição de função qualificada referenciada por meio da **propriedade targetScheduleId** . Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "baseType": "microsoft.graph.request",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```

