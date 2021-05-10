---
title: Tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7825b19e80274c8bcd54a5d8d03aa1dd40cf49c9
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298495"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>Tipo de recurso accessPackageAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote de acesso. Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.  O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para controlar a remoção de acesso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Recupere uma lista **de objetos accesspackageassignmentrequest.** |
| [Criar accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Crie um novo **accessPackageAssignmentRequest**. |
| [Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Leia propriedades e relações de um **objeto accessPackageAssignmentRequest.** |
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Recupere a lista de **objetos accessPackageAssignmentRequest** filtrados no usuário de entrada.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Cancele **um objeto accessPackageAssignmentRequest** que está em estado cancelável.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|A data do final do processamento, bem-sucedida ou falha, de uma solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|id|String| Somente leitura.|
|isValidationOnly|Booliano|True se a solicitação não for processada para atribuição.|
|justification|Cadeia de caracteres|A justificativa fornecida pelo solicitante.|
|requestState|Cadeia de caracteres|Um dos `PendingApproval` , , , , , ou `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` . Somente leitura.|
|requestStatus|Cadeia de caracteres|Mais informações sobre o status do processamento de solicitação. Somente leitura.|
|requestType|Cadeia de caracteres|Um dos `UserAdd` , `UserRemove` , ou `AdminAdd` `AdminRemove` `SystemRemove` . Uma solicitação do próprio usuário teria requestType de `UserAdd` ou `UserRemove` . Somente leitura.|
|Cronograma|[requestSchedule](requestschedule.md)| O intervalo de datas que o acesso deve ser atribuído ao solicitante. Somente leitura.|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| Para um requestType de `UserAdd` ou , esta é uma `AdminAdd` atribuição de pacote de acesso solicitada a ser criada.  Para um requestType `UserRemove` de , ou , isso tem a propriedade de uma `AdminRemove` `SystemRemove` `id` atribuição existente a ser removida.|
|answers|[Coleção accessPackageAnswer](accesspackageanswer.md)|Respostas fornecidas pelo solicitante para [acessarPackageQuestions solicitadas](accesspackagequestion.md) no momento da solicitação.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](../resources/accesspackage.md)|O pacote de acesso associado ao accessPackageAssignmentRequest. Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos. Somente leitura. Anulável.|
|requestor|[accessPackageSubject](accesspackagesubject.md)| O assunto que solicitou ou, se uma atribuição direta, foi atribuído. Somente leitura. Anulável.|


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
    "createdDateTime": "string",
    "completedDate": "string",
    "id": "string",
    "requestType": "string",
    "requestState": "string",
    "requestStatus": "string",
    "isValidationOnly": false,
    "justification": "string",
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "string",
        "answeredQuestion": {
            "id": "string",
            "text": {
                "defaultText": "string",
                "localizedTexts": [{
                    "text": "string",
                    "languageCode": "string"
                }]
            },
            "isRequired": true,
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": true
        }
    }]
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

