---
title: Atualizar accessPackageAssignmentPolicy
description: Atualize as propriedades de um objeto accessPackageAssignmentPolicy.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a5c02fc2b0850ec3a58638ce98e0dac45683ee39
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63332970"
---
# <a name="update-accesspackageassignmentpolicy"></a>Atualizar accessPackageAssignmentPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) existente para alterar uma ou mais de suas propriedades, como o nome de exibição ou a descrição.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .

A tabela a seguir mostra as propriedades que são necessárias ao atualizar [um accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da política.|
|descrição|String|A descrição da política.|
|canExtend|Booliano|Indica se um usuário pode estender a duração da atribuição do pacote de acesso após a aprovação.|
|durationInDays|Int32|O número de dias em que as atribuições dessa política duram até expirar.|
|expirationDateTime|DateTimeOffset|A data de expiração das atribuições criadas nesta política. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|requestorSettings|[requestorSettings](../resources/requestorsettings.md)|Who pode solicitar esse pacote de acesso a partir desta política.|
|requestApprovalSettings|[approvalSettings](../resources/approvalsettings.md)|Who deve aprovar solicitações para o pacote de acesso nesta política.|
|accessReviewSettings|[assignmentReviewSettings](../resources/assignmentreviewsettings.md)|Who deve revisar e com que frequência as atribuições para o pacote de acesso desta política. Essa propriedade será nula se as avaliações não são necessárias.|


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) atualizado no corpo da resposta.


## <a name="examples"></a>Exemplos

### <a name="example-1-update-the-details-of-a-policy"></a>Exemplo 1: atualizar os detalhes de uma política

#### <a name="request"></a>Solicitação
Nesta atualização de política, uma das opções para a pergunta de múltipla escolha foi removida. Os futuros solicitadores não terão mais a opção removida disponível para eles.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/b2eba9a1-b357-42ee-83a8-336522ed6cbf
Content-Type: application/json

{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "4c02f928-7752-49aa-8fc8-e286d973a965",
    "displayName": "All Users",
    "description": "All users can request for access to the directory.",
    "canExtend": false,
    "durationInDays": 365,
    "expirationDateTime": null,
    "requestorSettings": {
        "scopeType": "AllExistingConnectedOrganizationSubjects",
        "acceptRequests": true,
        "allowedRequestors": []
    },
    "requestApprovalSettings": {
        "isApprovalRequired": true,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": true,
        "approvalMode": "SingleStage",
        "approvalStages": [{
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": false,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [{
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "d2dcb9a1-a445-42ee-83a8-476522ed6cbf",
                        "description": "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.externalSponsors",
                        "isBackup": false
                    }
                ]
            }
        ]
    },
    "questions": [{
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
}
```
# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accesspackageassignmentpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "4c02f928-7752-49aa-8fc8-e286d973a965",
    "displayName": "Users from connected organizations can request",
    "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
    "questions": [{
        "id" : "BD3F6B95-458D-4BC8-A9A6-8D4B29F64F3D",
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "OH",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Ohio",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "id" : "F652C13C-A660-4E4C-A1E0-CE9FEC6EE57A",
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
}
```



### <a name="example-2-remove-the-customextensionhandlers-from-a-policy"></a>Exemplo 2: Remover os customExtensionHandlers de uma política

Para remover a coleção **de customExtensionHandlers** e seus objetos de extensão de fluxo de trabalho personalizados associados de uma política, atribua uma coleção vazia ao **objeto customExtensionHandlers** .

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy_delete_customExtensionHandlers"
}
-->

```http
PUT https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/4540a08f-8ab5-43f6-a923-015275799197
Content-Type: application/json

{
    "id": "4540a08f-8ab5-43f6-a923-015275799197",
    "displayName": "policy with custom access package workflow extension",
    "description": "Run specified custom access package workflow extension at different stages.",
    "accessPackageId": "ba5807c7-2aa9-4c8a-907e-4a17ee587500",
    "expiration": {
        "type": "afterDuration",
        "duration": "P365D"
    },
    "requestApprovalSettings": null,
    "requestorSettings": {
        "acceptRequests": true,
        "scopeType": "AllExistingDirectorySubjects",
        "allowedRequestors": []
    },
    "accessReviewSettings": null,
    "customExtensionHandlers": []
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackageassignmentpolicy-delete-customextensionhandlers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a>Resposta
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "4540a08f-8ab5-43f6-a923-015275799197",
    "displayName": "policy with custom access package workflow extension",
    "description": "Run specified custom access package workflow extension at different stages.",
    "accessPackageId": "ba5807c7-2aa9-4c8a-907e-4a17ee587500",
    "expiration": {
        "type": "afterDuration",
        "duration": "P365D"
    },
    "requestApprovalSettings": null,
    "requestorSettings": {
        "acceptRequests": true,
        "scopeType": "AllExistingDirectorySubjects",
        "allowedRequestors": []
    },
    "accessReviewSettings": null
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


