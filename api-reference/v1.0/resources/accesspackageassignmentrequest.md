---
title: Tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2581172e02eede572de589b4122bec646306baed
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242184"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>Tipo de recurso accessPackageAssignmentRequest

Namespace: microsoft.graph


No [Azure AD Entitlement Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote de acesso. Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.  O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para controlar a remoção de acesso.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md)|[coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md)|Recupere uma lista **de objetos accesspackageassignmentrequest.** |
|[Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)|Leia propriedades e relações de um **objeto accessPackageAssignmentRequest.** |
|[Excluir accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|Nenhum|Excluir um **accessPackageAssignmentRequest**. |
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Recupere a lista de **objetos accessPackageAssignmentRequest** filtrados no usuário de entrada.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Cancele **um objeto accessPackageAssignmentRequest** que está em estado cancelável.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|completedDate|DateTimeOffset|A data do final do processamento, bem-sucedida ou falha, de uma solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|id|String|Somente leitura.|
|requestType|accessPackageRequestType|O tipo da solicitação. Os valores possíveis são: `notSpecified` , , , , , , , , `userAdd` , , , `userUpdate` , , `userRemove` `adminAdd` `adminUpdate` `adminRemove` `systemAdd` `systemUpdate` `systemRemove` `onBehalfAdd` `unknownFutureValue` . Uma solicitação do próprio usuário teria requestType de `UserAdd` ou `UserRemove` . Essa propriedade não pode ser alterada uma vez definida.|
|Cronograma|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|O intervalo de datas que o acesso deve ser atribuído ao solicitante. Essa propriedade não pode ser alterada uma vez definida.|
|state|accessPackageRequestState|O estado da solicitação. Os valores possíveis são `submitted`, `pendingApproval`, `delivering`, `delivered`, `deliveryFailed`, `denied`, `scheduled`, `canceled`, `partiallyDelivered`, `unknownFutureValue`. Apenas leitura.|
|status|Cadeia de caracteres|Mais informações sobre o status do processamento de solicitação. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|O pacote de acesso associado ao accessPackageAssignmentRequest. Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos. Somente leitura. Anulável. <br/><br/> Suporta o `$expand`.|
|assignment|[accessPackageAssignment](../resources/accesspackageassignment.md)|Para um **requestType** de `UserAdd` ou , esta é uma `AdminAdd` atribuição de pacote de acesso solicitada a ser criada.  Para um **requestType** `UserRemove` de , ou , isso tem a propriedade de uma `AdminRemove` `SystemRemove` `id` atribuição existente a ser removida.  <br/><br/> Suporta o `$expand`.|
|requestor|[accessPackageSubject](../resources/accesspackagesubject.md)|O assunto que solicitou ou, se uma atribuição direta, foi atribuído. Somente leitura. Anulável. Suporta o `$expand`.|

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
  "completedDate": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


