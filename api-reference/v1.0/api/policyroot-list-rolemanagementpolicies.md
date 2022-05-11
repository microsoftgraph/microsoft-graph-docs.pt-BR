---
title: Listar roleManagementPolicies
description: Obtenha políticas de gerenciamento de funções e seus detalhes.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 894eba495c2535a0af32227b83afe3ce1a3021bb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315536"
---
# <a name="list-rolemanagementpolicies"></a>Listar roleManagementPolicies
Namespace: microsoft.graph

Obtenha políticas de gerenciamento de funções e seus detalhes.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies?$filter=scopeId eq 'scopeId' and scopeType eq 'scopeType'
```

## <a name="query-parameters"></a>Parâmetros de consulta
Esse método requer o parâmetro `$filter` de consulta (`eq`) para definir o escopo da solicitação para **um scopeId** e **um scopeType**. Você também pode usar os parâmetros `$select` de `$expand` consulta e OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de [objetos unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-the-role-management-policies-that-apply-to-azure-ad-roles"></a>Exemplo 1: recuperar as políticas de gerenciamento de função que se aplicam a Azure AD funções

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicies?$filter=scopeId eq '/' and scopeType eq 'DirectoryRole'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrolemanagementpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicies",
    "value": [
        {
            "id": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
            "displayName": "DirectoryRole",
            "description": "DirectoryRole",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "lastModifiedDateTime": null,
            "lastModifiedBy": {
                "displayName": null,
                "id": null
            }
        },
        {
            "id": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_23b16f1a-1f8d-4891-93b1-21244cdf6115",
            "displayName": "DirectoryRole",
            "description": "DirectoryRole",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "lastModifiedDateTime": null,
            "lastModifiedBy": {
                "displayName": null,
                "id": null
            }
        }
    ]
}
```

### <a name="example-2-retrieve-the-role-management-policies-that-apply-to-the-directory-and-expand-the-associated-rules"></a>Exemplo 2: recuperar as políticas de gerenciamento de função que se aplicam ao diretório e expandir as regras associadas

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy_expand_rules"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicies?$filter=scopeId eq '/' and scopeType eq 'Directory'&$expand=rules
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicy-expand-rules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicy-expand-rules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicy-expand-rules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicy-expand-rules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrolemanagementpolicy-expand-rules-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicies(rules())",
    "value": [
        {
            "id": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
            "displayName": "Directory",
            "description": "Directory",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "Directory",
            "lastModifiedDateTime": "2022-04-20T16:12:29.553Z",
            "lastModifiedBy": {
                "displayName": "MOD Administrator",
                "id": null
            },
            "rules@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicies('Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448')/rules",
            "rules": [
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
                    "id": "Expiration_Admin_Eligibility",
                    "isExpirationRequired": false,
                    "maximumDuration": "P365D",
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Admin_Admin_Eligibility",
                    "notificationType": "Email",
                    "recipientType": "Admin",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Requestor_Admin_Eligibility",
                    "notificationType": "Email",
                    "recipientType": "Requestor",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Approver_Admin_Eligibility",
                    "notificationType": "Email",
                    "recipientType": "Approver",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
                    "id": "Enablement_Admin_Eligibility",
                    "enabledRules": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
                    "id": "Expiration_Admin_Assignment",
                    "isExpirationRequired": false,
                    "maximumDuration": "P180D",
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
                    "id": "Enablement_Admin_Assignment",
                    "enabledRules": [
                        "Justification"
                    ],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Admin_Admin_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Admin",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Requestor_Admin_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Requestor",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Approver_Admin_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Approver",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
                    "id": "Expiration_EndUser_Assignment",
                    "isExpirationRequired": true,
                    "maximumDuration": "PT8H",
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
                    "id": "Enablement_EndUser_Assignment",
                    "enabledRules": [
                        "MultiFactorAuthentication",
                        "Justification"
                    ],
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
                    "id": "Approval_EndUser_Assignment",
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    },
                    "setting": {
                        "isApprovalRequired": false,
                        "isApprovalRequiredForExtension": false,
                        "isRequestorJustificationRequired": true,
                        "approvalMode": "SingleStage",
                        "approvalStages": [
                            {
                                "approvalStageTimeOutInDays": 1,
                                "isApproverJustificationRequired": true,
                                "escalationTimeInMinutes": 0,
                                "isEscalationEnabled": false,
                                "primaryApprovers": [],
                                "escalationApprovers": []
                            }
                        ]
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
                    "id": "AuthenticationContext_EndUser_Assignment",
                    "isEnabled": false,
                    "claimValue": null,
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Admin_EndUser_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Admin",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Requestor_EndUser_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Requestor",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Approver_EndUser_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Approver",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                }
            ]
        }
    ]
}
```
