---
title: Tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cdf2e4111daeea48babd57aac912006bd2418187
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698356"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>Tipo de recurso accessPackageAssignmentRequest

Namespace: microsoft.graph


No [Azure AD gerenciamento](entitlementmanagement-overview.md) de direitos, uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote de acesso. Se a solicitação for bem-sucedida, com as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.  Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para controlar a remoção de acesso.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md)|[coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md)|Recupere uma lista de **objetos accesspackageassignmentrequest** . |
| [Criar accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Cria um novo **objeto accessPackageAssignmentRequest** . |
|[Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)|Ler propriedades e relações de um **objeto accessPackageAssignmentRequest** . |
|[Excluir accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|Nenhum|**Exclua um accessPackageAssignmentRequest**. |
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Recupere a lista **de objetos accessPackageAssignmentRequest** filtrados no usuário conectado.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Cancele **um objeto accessPackageAssignmentRequest** que esteja em um estado cancelável.|
|[Reprocessar](../api/accesspackageassignmentrequest-reprocess.md) | Nenhum | Repita automaticamente a solicitação de acesso de um usuário a um pacote de acesso.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|A data do final do processamento, bem-sucedida ou falha, de uma solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|id|String|Somente leitura.|
|Requesttype|accessPackageRequestType|O tipo da solicitação. Os valores possíveis são: , , , , , `adminAdd`, `adminUpdate`, `adminRemove`, `systemAdd`, `systemUpdate`, , `systemRemove`, , `onBehalfAdd`, `unknownFutureValue`. `userRemove``userUpdate``userAdd``notSpecified` Uma solicitação do próprio usuário teria requestType de `UserAdd` ou `UserRemove`. Essa propriedade não pode ser alterada depois de definida.|
|Cronograma|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|O intervalo de datas que o acesso deve ser atribuído ao solicitante. Essa propriedade não pode ser alterada depois de definida.|
|state|accessPackageRequestState|O estado da solicitação. Os valores possíveis são `submitted`, `pendingApproval`, `delivering`, `delivered`, `deliveryFailed`, `denied`, `scheduled`, `canceled`, `partiallyDelivered`, `unknownFutureValue`. Somente leitura.|
|status|Cadeia de caracteres|Mais informações sobre o status de processamento da solicitação. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|O pacote de acesso associado ao accessPackageAssignmentRequest. Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos. Somente leitura. Anulável. <br/><br/> Suporta o `$expand`.|
|Atribuição|[accessPackageAssignment](../resources/accesspackageassignment.md)|Para um **requestType** de `UserAdd` ou `AdminAdd`, esta é uma atribuição de pacote de acesso solicitada para ser criada.  Para um **requestType** de `UserRemove`, `AdminRemove` ou `SystemRemove`, isso tem `id` a propriedade de uma atribuição existente a ser removida.  <br/><br/> Oferece suporte para `$expand`.|
|Solicitante|[accessPackageSubject](../resources/accesspackagesubject.md)|O assunto que solicitou ou, se uma atribuição direta, foi atribuído. Somente leitura. Anulável. Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "String (identifier)",
  "requestType": "String",
  "state": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


