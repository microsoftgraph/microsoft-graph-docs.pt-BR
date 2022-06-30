---
title: Tipo de recurso unifiedRoleEligibilityScheduleRequest
description: Representa a solicitação para operações de atribuição de função qualificadas por meio Azure AD Privileged Identity Management.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 557f67028190621c817b24188f5f44eb3c4c8dca
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446347"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>Tipo de recurso unifiedRoleEligibilityScheduleRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma solicitação de qualificação de função para uma entidade de segurança por meio do PIM. A qualificação de função pode ser permanentemente qualificada sem uma data de expiração ou temporariamente qualificada com uma data de expiração. Herda da [solicitação](../resources/request.md).

Para obter mais informações sobre cenários de PIM que você pode definir por meio do tipo de recurso **unifiedRoleEligibilityScheduleRequest** , consulte Visão geral do gerenciamento de funções por meio da [API pim (privileged identity management](privilegedidentitymanagementv3-overview.md)).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilityScheduleRequests](../api/rbacapplication-list-roleeligibilityschedulerequests.md)|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Recupere as solicitações de eligibilidades de função para entidades de segurança feitas por meio do objeto unifiedRoleEligibilityScheduleRequest.|
|[Criar unifiedRoleEligibilityScheduleRequest](../api/rbacapplication-post-roleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Solicitação de qualificação de função para uma entidade de segurança por meio do objeto unifiedRoleEligibilityScheduleRequest.|
|[Obter unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Leia os detalhes de uma solicitação de qualificação de função feita por meio do objeto unifiedRoleEligibilityScheduleRequest.|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|No PIM, recupere as solicitações de eligibilidades de função para uma entidade de segurança específica. A entidade de segurança pode ser o criador ou aprovador do objeto unifiedRoleEligibilityScheduleRequest ou pode ser o destino da elegibilidade da função.|
|[cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)|Nenhum|Cancele imediatamente **um objeto unifiedRoleEligibilityScheduleRequest** cujo status `Granted` é e faça com que o sistema exclua automaticamente a solicitação cancelada após 30 dias.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|Cadeia de caracteres|Representa o tipo de operação na solicitação de qualificação de função. Os valores possíveis são: <br/><ul><li>`AdminAssign`: para que os administradores atribuam funções qualificadas às entidades de segurança.</li><li>`AdminRemove`: para que os administradores removam funções qualificadas das entidades de segurança.</li><li> `AdminUpdate`: para que os administradores alterem as eligibilidades de função existentes.</li><li>`AdminExtend`: para que os administradores estendam as eligibilidades de função expiradas.</li><li>`AdminRenew`: para que os administradores renovem as eligibilidades expiradas.</li><li>`UserAdd`: para que os usuários ativem suas atribuições qualificadas.</li><li>`UserRemove`: para que os usuários desativem suas atribuições qualificadas ativas.</li><li>`UserExtend`: para que os usuários solicitem a extensão de suas atribuições qualificadas de expiração.</li><li>`UserRenew`: para que os usuários solicitem a renovação de suas atribuições qualificadas expiradas.</li></ul>|
|approvalId|Cadeia de caracteres|O identificador da aprovação da solicitação. Herdado da [solicitação](../resources/request.md).|
|appScopeId|String|Identificador do escopo específico do aplicativo quando a elegibilidade de função está no escopo de um aplicativo. O escopo de uma elegibilidade de função determina o conjunto de recursos para os quais a entidade de segurança está qualificada para acessar. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação. Herdado da [solicitação](../resources/request.md).|
|createdBy|[identitySet](../resources/identityset.md)|A entidade de segurança que criou essa solicitação. Herdado da [solicitação](../resources/request.md).|
|createdDateTime|DateTimeOffset|A data de criação da solicitação. Herdado da [solicitação](../resources/request.md).|
|Customdata|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado. Herdado da [solicitação](../resources/request.md).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da elegibilidade da função. O escopo de uma elegibilidade de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|id|String|O identificador exclusivo do **objeto unifiedRoleEligibilityScheduleRequest** . Chave, não anulável, somente leitura.  Herdado da [entidade](../resources/entity.md).|
|isValidationOnly|Booliano|Determina se a chamada é uma validação ou uma chamada real. Defina essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|Justificação|String|Uma mensagem fornecida por usuários e administradores ao criar eles criam o objeto **unifiedRoleEligibilityScheduleRequest** .|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança que recebeu a qualificação de função. Suporta `$filter` (`eq`, `ne`).|
|roleDefinitionId|Cadeia de caracteres|Identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) que está sendo atribuído à entidade de segurança. Suporta `$filter` (`eq`, `ne`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O período de qualificação da função. No momento, não há suporte para agendamentos recorrentes.|
|status|Cadeia de caracteres|O status da solicitação de qualificação de função. Herdado da [solicitação](../resources/request.md). Somente leitura. Suporta `$filter` (`eq`, `ne`).|
|targetScheduleId|Cadeia de caracteres|Identificador do objeto de agendamento que está vinculado à solicitação de qualificação. Suporta `$filter` (`eq`, `ne`).|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Detalhes do tíquete vinculados à solicitação de qualificação de função, incluindo detalhes do número do tíquete e do sistema de tíquetes. Opcional.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando a elegibilidade de função está no escopo de um aplicativo. Anulável. Suporta o `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto de diretório que é o escopo da qualificação de função. Somente leitura. Oferece suporte para `$expand`.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade de segurança que está obtendo uma qualificação de função por meio da solicitação. Suporta o `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Informações detalhadas para [o objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) referenciado por meio da **propriedade roleDefinitionId** . Suporta o `$expand`.|
|targetSchedule|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|O agendamento para uma elegibilidade de função referenciada por meio da **propriedade targetScheduleId** . Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest",
  "baseType": "microsoft.graph.request",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
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

