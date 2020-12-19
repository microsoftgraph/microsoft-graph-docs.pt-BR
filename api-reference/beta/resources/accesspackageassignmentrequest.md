---
title: tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote do Access é criada por um usuário que deseja obter uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9ecaa9b77a92dc6393b3c7231976937e36502c8d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719752"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>tipo de recurso accessPackageAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote do Access. Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.  O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para rastrear a remoção do acesso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | coleção [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Recupere uma lista de objetos accesspackageassignmentrequest. |
| [Criar accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Criar um novo accessPackageAssignmentRequest. |
| [Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Ler propriedades e relações de um objeto accessPackageAssignmentRequest. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|A data do final do processamento, bem como êxito ou falha, de uma solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|id|String| Somente leitura.|
|isValidationOnly|Booliano|True se a solicitação não deve ser processada para a atribuição.|
|elabora|Cadeia de caracteres|A justificativa fornecida pelo solicitante.|
|RequestState|Cadeia de caracteres|Um dos `PendingApproval` , `Canceled` ,  `Denied` , `Delivering` , `Delivered` , `PartiallyDelivered` `Submitted` ou `Scheduled` . Somente leitura.|
|requestStatus|Cadeia de caracteres|Mais informações sobre o status do processamento da solicitação. Somente leitura.|
|RequestType|Cadeia de caracteres|Um de `UserAdd` , `UserRemove` , `AdminAdd` `AdminRemove` ou `SystemRemove` . Uma solicitação do próprio usuário teria o RequestType de `UserAdd` ou `UserRemove` . Somente leitura.|
|Cronograma|[requestSchedule](requestschedule.md)| O intervalo de datas que o Access deve ser atribuído ao solicitante. Somente leitura.|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| Para um RequestType `UserAdd` ou `AdminAdd` , esta é uma atribuição de pacote de acesso solicitada a ser criada.  Para um RequestType de `UserRemove` , `AdminRemove` ou `SystemRemove` , isso tem a `id` propriedade de uma atribuição existente a ser removida.|
|às|coleção [accessPackageAnswer](accesspackageanswer.md)|As respostas fornecidas pelo solicitante para [accessPackageQuestions](accesspackagequestion.md) as solicitadas no momento da solicitação.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|solicitante|[accessPackageSubject](accesspackagesubject.md)| O assunto que solicitou ou, se uma atribuição direta, foi atribuído. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "",
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

