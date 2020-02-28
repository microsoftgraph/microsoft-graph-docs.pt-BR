---
title: tipo de recurso accessPackageAssignmentPolicy
description: Uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 08fcefafe9a354a57415a7d05bee1ec57ffdc138
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331301"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>tipo de recurso accessPackageAssignmentPolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access. Um pacote de acesso pode ter zero ou mais políticas. Quando uma solicitação de um assunto é recebida, o assunto é correspondido em relação a cada política para localizar a política (se houver) com requestorSettings que inclua esse assunto. A política determina se a solicitação requer aprovação, a duração da atribuição do pacote de acesso e se a atribuição precisa ser revisada regularmente.

Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.


## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Recupere uma lista de objetos accessPackageAssignmentPolicy. |
| [Criar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Criar um novo objeto accessPackageAssignmentPolicy. |
| [Obter accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Ler propriedades e relações de um objeto accessPackageAssignmentPolicy. |
| [Excluir accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Excluir um accessPackageAssignmentPolicy. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageId|String|ID do pacote de acesso.|
|accessReviewSettings|[assignmentReviewSettings](assignmentreviewsettings.md)|Quem deve revisar e com que frequência as atribuições para o pacote de acesso desta política. Essa propriedade será nula se as revisões não forem necessárias.|
|exextend|Booliano|Indica se um usuário pode estender a duração da atribuição de pacote de acesso após a aprovação.|
|createdBy|String|Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|descrição|String|A descrição da política.|
|displayName|Cadeia de caracteres|O nome de exibição da política.|
|durationInDays|Int32|O número de dias em que as atribuições dessa política duram até que tenham expirado.|
|expirationDateTime|DateTimeOffset|A data de validade das atribuições criadas nesta política. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| Somente leitura.|
|isDenyPolicy|Booliano|Se true, a política não permitirá o acesso. Somente leitura.|
|modifiedBy|String|Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|requestApprovalSettings|[approvalSettings](approvalsettings.md)|Quem deve aprovar solicitações de pacote do Access nessa política.|
|requestorSettings|[requestorSettings](requestorsettings.md)|Quem pode solicitar esse pacote de acesso desta política.|


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| O pacote de acesso com esta política. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
    "displayName": "All Users",
    "description": "All users can request for access to the directory.",
    "isDenyPolicy": false,
    "canExtend": false,
    "durationInDays": 365,
    "requestorSettings" : {
      "scopeType": "AllExistingDirectorySubjects",
      "acceptRequests": true,
      "allowedRequestors": []
    },
    "requestApprovalSettings" : {
      "isApprovalRequired": false,
      "isApprovalRequiredForExtension": false,
      "isRequestorJustificationRequired": false,
      "approvalMode": "NoApproval",
      "approvalStages": []
    },
    "accessReviewSettings" : null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
