---
title: tipo de recurso governanceRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 611622930d0ff79a2b65589a5029c9eff5e773af
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219232"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>tipo de recurso governanceRoleAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.

`governanceRoleAssignmentRequest`é uma entidade com modelo de tíquete usada para gerenciar o ciclo de vida das atribuições de função. Ele representa a intenção/decisão dos usuários e administradores, e também fornece a flexibilidade para permitir a implementação de Schduling recorrentes, Gates de aprovação e assim por diante, em comparação à exposição `POST` `PUT`direta e às `DELETE` operações em `governanceRoleAssignment`.

## <a name="methods"></a>Métodos

| Método          |Tipo de retorno  |Descrição|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Obtenha uma solicitação de atribuição de função especificada por ID.  
|[List](../api/governanceroleassignmentrequest-list.md) | coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Obter solicitações de atribuição de função em um recurso.|
|[Create](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Criar uma solicitação para gerenciar o ciclo de vida da atribuição de função nova ou existente.|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |Cancelar uma solicitação de atribuição de função pendente.|
|[Update](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Os administradores atualizam as decisões sobre solicitações se as solicitações estiverem no `PendingAdminDecision`status de.|

## <a name="properties"></a>Propriedades
| Propriedade                  | Tipo          |Descrição|
|:--------------------------|:--------------|:----------|
|id                         |String         |A ID da solicitação de atribuição de função.|
|resourceId                 |String         |Obrigatório. A ID do recurso ao qual a solicitação de atribuição de função está associada.|
|roleDefinitionId           |String         |Obrigatório. A ID da definição de função à qual a solicitação de atribuição de função está associada.|
|SubjectID                  |String         |Obrigatório. A ID da entidade à qual a solicitação de atribuição de função está associada.|
|tipo                       |String         |Obrigatório. Representando o tipo da operação na atribuição de função. O valor pode ser <ul><li>`AdminAdd`: Administradores atribuem usuários/grupos a funções;</li><li>`UserAdd`: Os usuários ativam atribuições qualificadas;</li><li> `AdminUpdate`: Administradores alterar as atribuições de função existentes</li><li>`AdminRemove`: Administradores removem usuários/grupos de funções;<li>`UserRemove`: Os usuários desativam atribuições ativas;<li>`UserExtend`: Os usuários solicitam estender suas atribuições de expiração;</li><li>`AdminExtend`: Os administradores extendem as atribuições expiradas.</li><li>`UserRenew`: Os usuários solicitam a renovação de suas atribuições expiradas;</li><li>`AdminRenew`: Os administradores extendem as atribuições expiradas.</li></ul>|
|assignmentstate|String  |Obrigatório. O estado da atribuição. O valor pode ser <ul><li> `Eligible`para atribuição qualificada</li><li> `Active`– Se ele for atribuído `Active` diretamente por administradores ou ativado em uma atribuição qualificada pelos usuários.</li></ul>|
|requestedDateTime          |DateTimeOffset |Somente leitura. O tempo de criação da solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|Cronograma                   |[governanceSchedule](governanceschedule.md)|O objeto Schedule da solicitação de atribuição de função.|
|motivo                     |Cadeia de Caracteres         |Uma mensagem fornecida por usuários e administradores quando você cria a solicitação sobre por que ela é necessária.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |O status da solicitação de atribuição de função.|
|linkedEligibleRoleAssignmentId|Cadeia de Caracteres        |Se esta for uma solicitação para ativação de função, ela representará a ID `eligible assignment` da referida; Caso contrário, o valor `null`será. |



## <a name="relationships"></a>Relações
| Relação | Tipo                                |Descrição|
|:-------------|:----------------------------------|:----------|
|recurso      |[governanceResource](../resources/governanceresource.md)            |Somente leitura. O recurso para o qual a solicitação pretende. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Somente leitura. A definição de função para a qual a solicitação pretende. |
|assunto       |[governanceSubject](../resources/governancesubject.md)|Somente leitura. A entidade de usuário/grupo.|

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
