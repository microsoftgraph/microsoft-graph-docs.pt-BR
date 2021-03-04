---
title: Tipo de recurso accessPackageAssignmentPolicy
description: Uma política de atribuição de pacote de acesso especifica a política pela qual os titulares podem solicitar ou ser atribuídos um pacote de acesso por meio de uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 269a3a27d83951c82d50dcaf0ba52c6ce7a5a1bb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433263"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>Tipo de recurso accessPackageAssignmentPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma política de atribuição de pacote de acesso especifica a política pela qual os titulares podem solicitar ou ter um pacote de acesso atribuído por meio de uma atribuição de pacote de acesso. Um pacote de acesso pode ter zero ou mais políticas. Quando uma solicitação de um assunto é recebida, o assunto é corresponder a cada política para encontrar a política (se alguma) com requestorSettings que incluem esse assunto. Em seguida, a política determina se a solicitação requer aprovação, a duração da atribuição do pacote de acesso e se a atribuição precisa ser revisada regularmente.

Para atribuir um usuário a um pacote de acesso, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faz referência ao pacote de acesso e à política de atribuição de pacote de acesso.


## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [coleção accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Recupere uma lista de objetos accessPackageAssignmentPolicy. |
| [Criar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Crie um novo objeto accessPackageAssignmentPolicy. |
| [Obter accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Ler propriedades e relações de um objeto accessPackageAssignmentPolicy. |
| [Atualizar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Atualize as propriedades de um objeto accessPackageAssignmentPolicy. |
| [Excluir accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Exclua um accessPackageAssignmentPolicy. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageId|String|ID do pacote de acesso.|
|accessReviewSettings|[assignmentReviewSettings](assignmentreviewsettings.md)|Quem deve revisar e com que frequência as atribuições para o pacote de acesso desta política. Essa propriedade será nula se as avaliações não são necessárias.|
|canExtend|Booliano|Indica se um usuário pode estender a duração da atribuição do pacote de acesso após a aprovação.|
|createdBy|String|Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|descrição|String|A descrição da política.|
|displayName|String|O nome de exibição da política.|
|durationInDays|Int32|O número de dias em que as atribuições dessa política duram até expirar.|
|expirationDateTime|DateTimeOffset|A data de expiração das atribuições criadas nesta política. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| Somente leitura.|
|modifiedBy|String|Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|requestApprovalSettings|[approvalSettings](approvalsettings.md)|Quem deve aprovar solicitações de pacote de acesso nesta política.|
|requestorSettings|[requestorSettings](requestorsettings.md)|Quem pode solicitar esse pacote de acesso a partir dessa política.|
|questions|[Coleção accessPackageQuestion](accesspackagequestion.md)|Perguntas que são colocadas ao solicitante.|


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| O pacote de acesso com essa política. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "string",
    "accessPackageId": "string",
    "displayName": "string",
    "description": "string",
    "isDenyPolicy": false,
    "canExtend": false,
    "durationInDays": 365,
    "requestorSettings": {
        "scopeType": "string",
        "acceptRequests": true,
        "allowedRequestors": [{
            "@odata.type": "#microsoft.graph.userSet"
        }]
    },
    "requestApprovalSettings": {
        "isApprovalRequired": false,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": false,
        "approvalMode": "string",
        "approvalStages": [{
            "approvalStageTimeOutInDays": 14,
            "isApproverJustificationRequired": true,
            "isEscalationEnabled": true,
            "escalationTimeInMinutes": 11520,
            "primaryApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }],
            "escalationApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }]
        }]
    },
    "accessReviewSettings": null,
    "questions": [{
        "@odata.type": "#microsoft.graph.question"
    }]
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

