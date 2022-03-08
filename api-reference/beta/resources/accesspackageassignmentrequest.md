---
title: Tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b12d512b34c1b42751cae22c6a387ff9c2e69e8d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337520"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>Tipo de recurso accessPackageAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-overview.md), uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote de acesso. Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.  O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para controlar a remoção de acesso.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignmentRequests](../api/entitlementmanagement-list-accesspackageassignmentrequests.md) | [coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Recupere uma lista **de objetos accesspackageassignmentrequest** . |
| [Criar accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Crie um novo **accessPackageAssignmentRequest**. |
| [Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Leia propriedades e relações de um **objeto accessPackageAssignmentRequest** . |
| [Excluir accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |Nenhum | **Exclua um accessPackageAssignmentRequest**. |
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Recupere a lista de **objetos accessPackageAssignmentRequest** filtrados no usuário de entrada.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Cancele **um objeto accessPackageAssignmentRequest** que está em estado cancelável.|
| [reprocessamento](../api/accesspackageassignmentrequest-reprocess.md) | Nenhum | Repetir automaticamente a solicitação de acesso de um usuário a um pacote de acesso.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|A data do final do processamento, bem-sucedida ou falha, de uma solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|customExtensionHandlerInstances|[Coleção customExtensionHandlerInstance](../resources/customextensionhandlerinstance.md)| Uma coleção de [instâncias de extensão de](customaccesspackageworkflowextension.md) fluxo de trabalho personalizadas sendo executados em uma solicitação de atribuição. Somente leitura. |
|id|String| Somente leitura.|
|isValidationOnly|Booliano|True se a solicitação não for processada para atribuição.|
|justification|Cadeia de caracteres|A justificativa fornecida pelo solicitante.|
|requestState|String|Um de `PendingApproval`, `Canceled``Denied`, , `Delivering`, `Delivered`, `PartiallyDelivered`, `DeliveryFailed`, ou `Scheduled``Submitted` . Somente leitura.|
|requestStatus|String|Mais informações sobre o status do processamento de solicitação. Somente leitura.|
|requestType|String|Um dos `UserAdd`, `UserRemove`, `AdminAdd`ou `AdminRemove` `SystemRemove`. Uma solicitação do próprio usuário teria requestType de `UserAdd` ou `UserRemove`. Somente leitura.|
|Cronograma|[requestSchedule](requestschedule.md)| O intervalo de datas que o acesso deve ser atribuído ao solicitante. Somente leitura.|
|answers|[Coleção accessPackageAnswer](accesspackageanswer.md)|Respostas fornecidas pelo solicitante para [acessarPackageQuestions solicitadas](accesspackagequestion.md) no momento da solicitação.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](../resources/accesspackage.md)|O pacote de acesso associado ao accessPackageAssignmentRequest. Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos. Somente leitura. Anulável. Suporta o `$expand`.|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| Para um **requestType** de `UserAdd` ou `AdminAdd`, esta é uma atribuição de pacote de acesso solicitada a ser criada.  Para um **requestType** de `UserRemove`, `AdminRemove` ou `SystemRemove`, isso tem `id` a propriedade de uma atribuição existente a ser removida.  Suporta o `$expand`.|
|requestor|[accessPackageSubject](accesspackagesubject.md)| O assunto que solicitou ou, se uma atribuição direta, foi atribuído. Somente leitura. Anulável. Suporta o `$expand`.|


## <a name="json-representation"></a>Representação JSON


Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "String (identifier)",
  "requestType": "String",
  "requestState": "String",
  "requestStatus": "String",
  "isValidationOnly": "Boolean",
  "createdDateTime": "String (timestamp)",
  "completedDate": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "justification": "String",
  "schedule": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "answers": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerString"
    }
  ],
  "customExtensionHandlerInstances": [
    {
      "@odata.type": "microsoft.graph.customExtensionHandlerInstance"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
