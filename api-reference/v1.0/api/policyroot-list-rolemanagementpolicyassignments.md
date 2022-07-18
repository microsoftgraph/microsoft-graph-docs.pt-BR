---
title: Listar roleManagementPolicyAssignments
description: Obtenha os detalhes de todas as atribuições de política de gerenciamento de função, incluindo as políticas e regras associadas às Azure AD funções.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b3722058c05636791087295f5f3d4aab6ccc4035
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447174"
---
# <a name="list-rolemanagementpolicyassignments"></a>Listar roleManagementPolicyAssignments
Namespace: microsoft.graph

Obtenha os detalhes de todas as atribuições de política de gerenciamento de função, incluindo as políticas e regras associadas às Azure AD funções.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments?$filter=scopeId eq 'scopeId' and scopeType eq 'scopeType'
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método requer o parâmetro `$filter` de consulta (`eq`) para definir o escopo da solicitação para **um scopeId** e **um scopeType**. Você também pode filtrar pela **roleDefinitionId** ou usar `$select` `$expand` os parâmetros de consulta e OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção de objetos [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-the-role-management-policy-assignments"></a>Exemplo 1: Recuperar as atribuições de política de gerenciamento de função

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyassignment"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicyAssignments?$filter=scopeId eq '/' and scopeType eq 'Directory'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrolemanagementpolicyassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-unifiedrolemanagementpolicyassignment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicyAssignments",
    "value": [
        {
            "id": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10",
            "policyId": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
            "scopeId": "/",
            "scopeType": "Directory",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_23b16f1a-1f8d-4891-93b1-21244cdf6115_2af84b1e-32c8-42b7-82bc-daa82404023b",
            "policyId": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_23b16f1a-1f8d-4891-93b1-21244cdf6115",
            "scopeId": "/",
            "scopeType": "Directory",
            "roleDefinitionId": "2af84b1e-32c8-42b7-82bc-daa82404023b"
        }
    ]
}
```


### <a name="example-2-retrieve-the-role-management-policy-assignments-for-an-azure-ad-role-and-expand-the-policy-and-its-associated-rules"></a>Exemplo 2: recuperar as atribuições de política de gerenciamento de função para uma função Azure AD e expandir a política e suas regras associadas

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyassignment_expand_all_relationships"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicyAssignments?$filter=scopeId eq '/' and scopeType eq 'DirectoryRole' and roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'&$expand=policy($expand=rules)
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyassignment-expand-all-relationships-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyassignment-expand-all-relationships-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyassignment-expand-all-relationships-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyassignment-expand-all-relationships-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrolemanagementpolicyassignment-expand-all-relationships-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-unifiedrolemanagementpolicyassignment-expand-all-relationships-powershell-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicyAssignments(policy(rules()))",
    "value": [
        {
            "id": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10",
            "policyId": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "policy": {
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
                },
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
        }
    ]
}
```
