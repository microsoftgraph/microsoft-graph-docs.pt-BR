---
title: Tipo de recurso governanceRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função em Gerenciamento de Identidade Privilegd.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: eeda7ef9502632853afe95e98922668f19e06421
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722290"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>Tipo de recurso governanceRoleAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de operações de atribuição de função em Gerenciamento de Identidade Privilegd.

`governanceRoleAssignmentRequest` é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida das atribuições de função. Ele representa a intenção/decisão dos usuários e administradores e também oferece a flexibilidade para habilitar a implementação de esquemas recorrentes, portais de aprovação e assim por diante, em comparação com a exposição direta , e operações `POST` `PUT` em `DELETE` `governanceRoleAssignment` .

## <a name="methods"></a>Métodos

| Método          |Tipo de retorno  |Descrição|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Obter uma solicitação de atribuição de função especificada pela ID.  
|[List](../api/governanceroleassignmentrequest-list.md) | [Coleção governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Obter solicitações de atribuição de função em um recurso.|
|[Create](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Crie uma solicitação para gerenciar o ciclo de vida da atribuição de função existente ou nova.|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |Cancele uma solicitação de atribuição de função pendente.|
|[Update](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Os administradores atualizam as decisões sobre solicitações se as solicitações estão em status de `PendingAdminDecision` .|

## <a name="properties"></a>Propriedades
| Propriedade                  | Tipo          |Descrição|
|:--------------------------|:--------------|:----------|
|id                         |Cadeia de caracteres         |A id da solicitação de atribuição de função.|
|resourceId                 |Cadeia de caracteres         |Obrigatório. A id do recurso ao qual a solicitação de atribuição de função está associada.|
|roleDefinitionId           |Cadeia de caracteres         |Obrigatório. A id da definição de função à qual a solicitação de atribuição de função está associada.|
|subjectId                  |Cadeia de caracteres         |Obrigatório. A id do assunto ao qual a solicitação de atribuição de função está associada.|
|tipo                       |String         |Obrigatório. Representando o tipo da operação na atribuição de função. O valor pode ser <ul><li>`AdminAdd`: Os administradores atribuem usuários/grupos a funções;</li><li>`UserAdd`: Os usuários ativam atribuições qualificadas;</li><li> `AdminUpdate`: Os administradores alteram as atribuições de função existentes</li><li>`AdminRemove`: Os administradores removem usuários/grupos de funções;<li>`UserRemove`: Os usuários desativam as atribuições ativas;<li>`UserExtend`: Os usuários solicitam estender suas atribuições de expiração;</li><li>`AdminExtend`: Os administradores estendem atribuições expiradas.</li><li>`UserRenew`: Os usuários solicitam a renovação de suas atribuições expiradas;</li><li>`AdminRenew`: Os administradores estendem atribuições expiradas.</li></ul>|
|assignmentState|Cadeia de caracteres  |Obrigatório. O estado da atribuição. O valor pode ser <ul><li> `Eligible` para atribuição qualificada</li><li> `Active` - se ele for atribuído diretamente pelos administradores ou ativado em uma `Active` atribuição qualificada pelos usuários.</li></ul>|
|requestedDateTime          |DateTimeOffset |Somente leitura. A solicitação cria tempo. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|Cronograma                   |[governanceSchedule](governanceschedule.md)|O objeto schedule da solicitação de atribuição de função.|
|motivo                     |Cadeia de caracteres         |Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |O status da solicitação de atribuição de função.|
|linkedEligibleRoleAssignmentId|Cadeia de caracteres        |Se for uma solicitação de ativação de função, ela representará a id do `eligible assignment` referido; Caso contrário, o valor será `null` . |



## <a name="relationships"></a>Relações
| Relação | Tipo                                |Descrição|
|:-------------|:----------------------------------|:----------|
|recurso      |[governanceResource](../resources/governanceresource.md)            |Somente leitura. O recurso que a solicitação visa. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Somente leitura. A definição de função que a solicitação visa. |
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


