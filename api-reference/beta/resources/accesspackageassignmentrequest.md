---
title: Tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 89977897860133b92fc445036296de283a56b922
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433261"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>Tipo de recurso accessPackageAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma solicitação de atribuição de pacote de acesso é criada por ou em nome de um usuário que deseja obter uma atribuição de pacote de acesso. Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.  O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para controlar a remoção de acesso.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [coleção accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Recupere uma lista de objetos accesspackageassignmentrequest. |
| [Criar accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Crie um novo accessPackageAssignmentRequest. |
| [Obter accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Leia propriedades e relações de um objeto accessPackageAssignmentRequest. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|A data do final do processamento, bem-sucedida ou falha, de uma solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|id|String| Somente leitura.|
|isValidationOnly|Booliano|True se a solicitação não for processada para atribuição.|
|justification|String|A justificativa fornecida pelo solicitante.|
|requestState|String|Um dos `PendingApproval` , , , , , ou `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` . Somente leitura.|
|requestStatus|String|Mais informações sobre o status do processamento de solicitação. Somente leitura.|
|requestType|String|Um dos `UserAdd` , `UserRemove` , ou `AdminAdd` `AdminRemove` `SystemRemove` . Uma solicitação do próprio usuário teria requestType de `UserAdd` ou `UserRemove` . Somente leitura.|
|Cronograma|[requestSchedule](requestschedule.md)| O intervalo de datas que o acesso deve ser atribuído ao solicitante. Somente leitura.|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| Para um requestType de `UserAdd` ou , esta é uma `AdminAdd` atribuição de pacote de acesso solicitada a ser criada.  Para um requestType `UserRemove` de , ou , isso tem a propriedade de uma `AdminRemove` `SystemRemove` `id` atribuição existente a ser removida.|
|answers|[Coleção accessPackageAnswer](accesspackageanswer.md)|Respostas fornecidas pelo solicitante para [acessarPackageQuestions solicitadas](accesspackagequestion.md) no momento da solicitação.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
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

