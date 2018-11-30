---
title: tipo de recurso de governanceRoleAssignmentRequest
description: Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.
ms.openlocfilehash: 4b19ed04b4c78fa084c1247fc1798a39b08c3fdb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27032942"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>tipo de recurso de governanceRoleAssignmentRequest

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.

`governanceRoleAssignmentRequest`uma entidade modelada de tíquete é usada para gerenciar o ciclo de vida de atribuições de função. Ele representa a intenção/decisão dos usuários e administradores e também oferece flexibilidade para permitir a implementação de schduling recorrente, entradas de aprovação e assim por diante, em relação ao diretamente expondo `POST`, `PUT`, e `DELETE` operações em `governanceRoleAssignment`.

## <a name="methods"></a>Métodos

| Método          |Tipo de retorno  |Descrição|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Obtenha uma solicitação de atribuição de função especificada por ID.  
|[List](../api/governanceroleassignmentrequest-list.md) | coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Obtenha as solicitações de atribuição de função em um recurso.|
|[Create](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Crie uma solicitação para gerenciar o ciclo de vida de atribuição de função de novo ou existente.|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |Cancele uma solicitação de atribuição de função pendente.|
|[Update](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Os administradores atualizar as decisões sobre solicitações se as solicitações são no status de `PendingAdminDecision`.|

## <a name="properties"></a>Propriedades
| Propriedade                  | Tipo          |Descrição|
|:--------------------------|:--------------|:----------|
|id                         |String         |A identificação da solicitação de atribuição de função.|
|resourceId                 |Cadeia de caracteres         |Obrigatório. A identificação do recurso que a solicitação de atribuição de função é associada.|
|roleDefinitionId           |Cadeia de caracteres         |Obrigatório. A id da definição de função que a solicitação de atribuição de função é associada.|
|subjectId                  |Cadeia de caracteres         |Obrigatório. A identificação do assunto da qual a solicitação de atribuição de função é associada.|
|type                       |Cadeia de caracteres         |Obrigatório. Representando o o tipo da operação na atribuição de função. O valor pode ser <ul><li>`AdminAdd`: Os administradores de atribuir funções; a usuários/grupos</li><li>`UserAdd`: Usuários ativarem elegíveis atribuições;</li><li> `AdminUpdate`: Os administradores alterar as atribuições de função existente</li><li>`AdminRemove`: Os administradores de removam usuários/grupos de funções;<li>`UserRemove`: Usuários desativar atribuições ativas;<li>`UserExtend`: Solicitação de usuários para estender as suas atribuições expiradas;</li><li>`AdminExtend`: Administradores estendem atribuições expiradas.</li><li>`UserRenew`: Solicitação de os usuários de renovação de suas atribuições expiradas;</li><li>`AdminRenew`: Administradores estendem atribuições expiradas.</li></ul>|
|assignmentState|Cadeia de caracteres  |Obrigatório. O estado da atribuição. O valor pode ser <ul><li> `Eligible`para atribuição elegível</li><li> `Active`-se diretamente atribuída `Active` pelos administradores, ou ativado em uma atribuição elegível pelos usuários.</li></ul>|
|requestedDateTime          |DateTimeOffset |Somente leitura. A solicitação criar horário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|roleAssignmentStartDateTime|DateTimeOffset |A hora de início para a atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|roleAssignmentEndDateTime|DateTimeOffset   |A hora de término para a atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|agenda                   |[governanceSchedule](governanceschedule.md)|O objeto de agendamento da solicitação de atribuição de função.|
|motivo                     |String         |Uma mensagem fornecida por usuários e administradores quando criar a solicitação sobre por que ele é necessário.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |O status da solicitação de atribuição de função.|
|linkedEligibleRoleAssignmentId|String        |Se essa for uma solicitação de ativação de função, ela representa a identificação do `eligible assignment` sendo chamada; Caso contrário, o valor será `null`. |



## <a name="relationships"></a>Relações
| Relação | Tipo                                |Descrição|
|:-------------|:----------------------------------|:----------|
|recurso      |[governanceResource](../resources/governanceresource.md)            |Somente leitura. O recurso que visa a solicitação. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Somente leitura. A definição de função que visa a solicitação. |
|subject       |[governanceSubject](../resources/governancesubject.md)|Somente leitura. A entidade de segurança do usuário/grupo.|

### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "type": "String",
  "assignmentState": "String",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleAssignmentStartDateTime": "String (timestamp)",
  "roleAssignmentEndDateTime": "String (timestamp)",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
