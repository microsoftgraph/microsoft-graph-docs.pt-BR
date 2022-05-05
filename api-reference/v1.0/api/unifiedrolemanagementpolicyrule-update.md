---
title: Atualizar unifiedRoleManagementPolicyRule
description: Atualize uma regra definida para uma política de gerenciamento de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a32f562a86ed72d8da728973ca6c5b5a5db7fcbb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204405"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a>Atualizar unifiedRoleManagementPolicyRule
Namespace: microsoft.graph

Atualize uma regra definida para uma política de gerenciamento de função. A regra pode ser um dos seguintes tipos derivados do objeto [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) :
+ [unifiedRoleManagementPolicyApprovalRule](../resources/unifiedrolemanagementpolicyapprovalrule.md)
+ [unifiedRoleManagementPolicyAuthenticationContextRule](../resources/unifiedrolemanagementpolicyauthenticationcontextrule.md)
+ [unifiedRoleManagementPolicyEnablementRule](../resources/unifiedrolemanagementpolicyenablementrule.md)
+ [unifiedRoleManagementPolicyExpirationRule](../resources/unifiedrolemanagementpolicyexpirationrule.md)
+ [unifiedRoleManagementPolicyNotificationRule](../resources/unifiedrolemanagementpolicynotificationrule.md)

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|claimValue|Cadeia de Caracteres|O valor da declaração de contexto de autenticação. <br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyAuthenticationContextRule** .|
|enabledRules|Coleção de cadeias de caracteres|A coleção de regras que estão habilitadas para essa regra de política. Por exemplo, `MultiFactorAuthentication`, `Ticketing`e `Justification`.<br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyEnablementRule** .|
|isDefaultRecipientsEnabled|Booliano|Indica se um destinatário padrão receberá o email de notificação.<br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyNotificationRule** .|
|isEnabled|Booliano| Se essa regra está habilitada. <br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyAuthenticationContextRule** .|
|isExpirationRequired|Boolean|Indica se a expiração é necessária ou se é uma atribuição ou qualificação permanentemente ativa. <br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyExpirationRule** .|
|maximumDuration|Duration| A duração máxima permitida para qualificação ou atribuição que não é permanente. Obrigatório quando **isExpirationRequired** é `true`. <br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyExpirationRule** . |
|Notificationlevel|Cadeia de Caracteres|O nível de notificação. Os valores possíveis são `None`, `Critical`. `All`<br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyNotificationRule** .|
|notificationRecipients|Coleção de cadeias de caracteres|A lista de destinatários das notificações por email.<br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyNotificationRule** .|
|Notificationtype|Cadeia de Caracteres|O tipo de notificação. Há `Email` suporte apenas para isso.<br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyNotificationRule** .|
|recipientType|Cadeia de Caracteres|O tipo de destinatário da notificação. Os valores possíveis são `Requestor`, `Approver`. `Admin`<br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyNotificationRule** .|
|configuração|[approvalSettings](../resources/approvalsettings.md)|As configurações para aprovação da atribuição de função. <br/><br/>Pode ser atualizado para o **tipo de regra unifiedRoleManagementPolicyApprovalRule** .|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Define detalhes do escopo direcionado pela regra de política de gerenciamento de função. Os detalhes podem incluir o tipo de entidade de segurança, o tipo de atribuição de função e as ações que afetam uma função. <br/><br/> Pode ser atualizado para todos os tipos de regra.|

>**Nota:** A `@odata.type` propriedade com um valor do tipo de regra específico deve ser incluída no corpo. Por exemplo, `"@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule"`.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

O exemplo a seguir atualiza uma regra de política de gerenciamento de função do tipo **unifiedRoleManagementPolicyExpirationRule** e com a ID é `Expiration_EndUser_Assignment`.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedrolemanagementpolicyrule"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/policies/roleManagementPolicies/DirectoryRole_84841066-274d-4ec0-a5c1-276be684bdd3_200ec19a-09e7-4e7a-9515-cf1ee64b96f9/rules/Expiration_EndUser_Assignment
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
    "id": "Expiration_EndUser_Assignment",
    "isExpirationRequired": true,
    "maximumDuration": "PT1H45M",
    "target": {
        "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
        "caller": "EndUser",
        "operations": [
            "All"
        ],
        "level": "Assignment",
        "inheritableSettings": [],
        "enforcedSettings": []
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-unifiedrolemanagementpolicyrule-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

