---
title: Tipo de recurso governanceRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função em Gerenciamento de Identidade Privada.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 8bee3a0abe303d1fe14e592104388b229e4d6424
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694271"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>Tipo de recurso governanceRoleAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1resourceroles-deprecation](../../includes/pim-v1resourceroles-deprecation.md)]

Representa a solicitação de operações de atribuição de função Privileged Identity Management.

`governanceRoleAssignmentRequest` é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida das atribuições de função. Ele representa a intenção/decisão dos usuários e administradores e também oferece a flexibilidade para habilitar a implementação de esquemas recorrentes, portais de aprovação e assim por diante, em comparação com a exposição direta , e operações `POST` `PUT` em `DELETE` `governanceRoleAssignment` .

## <a name="methods"></a>Methods

| Método          |Tipo de retorno  |Descrição|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Obter uma solicitação de atribuição de função especificada pela ID.  
|[Lista](../api/governanceroleassignmentrequest-list.md) | [Coleção governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Obter solicitações de atribuição de função em um recurso.|
|[Criar](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Crie uma solicitação para gerenciar o ciclo de vida da atribuição de função existente ou nova.|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |Cancele uma solicitação de atribuição de função pendente.|
|[Atualizar](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Os administradores atualizam as decisões sobre solicitações se as solicitações estão em status de `PendingAdminDecision` .|

## <a name="properties"></a>Propriedades
| Propriedade                  | Tipo          |Descrição|
|:--------------------------|:--------------|:----------|
|id                         |String         |A id da solicitação de atribuição de função.|
|resourceId                 |String         |Obrigatório. A id do recurso ao qual a solicitação de atribuição de função está associada.|
|roleDefinitionId           |String         |Obrigatório. A id da definição de função à qual a solicitação de atribuição de função está associada.|
|subjectId                  |String         |Obrigatório. A id do assunto ao qual a solicitação de atribuição de função está associada.|
|type                       |String        |Obrigatório. Representando o tipo da operação na atribuição de função. Os valores possíveis são: `AdminAdd` , , , , , , , , `UserAdd` , `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminExtend` `UserRenew` `AdminRenew` .|
|assignmentState|String  |Obrigatório. O estado da atribuição. Os valores possíveis são: (para atribuição qualificada), (se for atribuída diretamente), (por administradores ou ativada em uma atribuição qualificada `Eligible`  `Active` pelos `Active` usuários).|
|requestedDateTime          |DateTimeOffset |Somente leitura. A solicitação cria tempo. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|Cronograma                   |[governanceSchedule](governanceschedule.md)|O objeto schedule da solicitação de atribuição de função.|
|motivo                     |String         |Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |O status da solicitação de atribuição de função.|
|linkedEligibleRoleAssignmentId|String        |Se for uma solicitação de ativação de função, ela representará a id do `eligible assignment` referido; Caso contrário, o valor será `null` . |

|Member|Descrição|
|:---|:---|
|AdminAdd|Os administradores atribuem usuários/grupos a funções.|
|UserAdd|Os usuários ativam atribuições qualificadas.|
|AdminUpdate|Os administradores alteram as atribuições de função existentes.|
|AdminRemove|Os administradores removem usuários/grupos de funções.|
|UserRemove|Os usuários desativam as atribuições ativas.|
|UserExtend|Os usuários solicitam estender suas atribuições de expiração.|
|AdminExtend|Os administradores estendem atribuições expiradas.|
|UserRenew|Os usuários solicitam renovar suas atribuições expiradas.|
|AdminRenew|Os administradores estendem atribuições expiradas.|



## <a name="relationships"></a>Relações
| Relação | Tipo                                |Descrição|
|:-------------|:----------------------------------|:----------|
|recurso      |[governanceResource](../resources/governanceresource.md)            |Apenas leitura. O recurso que a solicitação visa. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Apenas leitura. A definição de função que a solicitação visa. |
|assunto       |[governanceSubject](../resources/governancesubject.md)|Apenas leitura. A entidade de usuário/grupo.|

### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


