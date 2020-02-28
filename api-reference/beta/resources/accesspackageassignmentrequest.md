---
title: tipo de recurso accessPackageAssignmentRequest
description: Uma solicitação de atribuição de pacote do Access é criada por um usuário que deseja obter uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c2440dfc7e798ea5b0a197f60b62acce4199b4ca
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331266"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>tipo de recurso accessPackageAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote do Access. Se a solicitação for bem-sucedida, com todas as aprovações necessárias, o usuário receberá uma atribuição de pacote de acesso e será o assunto dessa atribuição de pacote de acesso resultante.  O Azure AD também cria solicitações de atribuição de pacote de acesso automaticamente para rastrear a remoção do acesso.


## <a name="methods"></a>Methods

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
|elabora|String|A justificativa fornecida pelo solicitante.|
|RequestState|String|Um de `Denied`, `Delivered`, `PartiallyDelivered` `Submitted` ou `Scheduled`. Somente leitura.|
|requestStatus|String|Mais informações sobre o status do processamento da solicitação. Somente leitura.|
|RequestType|String|Um de `UserAdd`, `UserRemove`, `AdminAdd` `AdminRemove` ou `SystemRemove`. Somente leitura.|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| Uma atribuição de pacote de acesso solicitada foi criada.|

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
  "createdDateTime": "2020-02-12T22:06:58.303Z",
  "completedDate": "2020-02-12T22:14:28.19Z",
  "id": "1244d439-5baa-4b9a-be5f-e8fdef5a998b",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "justification": ""
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
