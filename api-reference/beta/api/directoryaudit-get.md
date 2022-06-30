---
title: Obter directoryAudit
description: Descreve o método get do recurso directoryAudit (entidade) do Microsoft API do Graph (versão beta).
ms.localizationpriority: medium
author: SarahBar
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: bc17537c2eafaf53855c65291296c03670d4842a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445705"
---
# <a name="get-directoryaudit"></a>Obter directoryAudit

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha um item de log de auditoria específico do Azure Active Directory. Isso inclui um item de log de auditoria gerado por vários serviços no Azure Active Directory, como usuário, aplicativo, gerenciamento de dispositivos e grupos, PIM (privileged identity management), revisões de acesso, termos de uso, proteção de identidade, gerenciamento de senha (redefinições de senha de administrador e autoatendimento), gerenciamento de grupo de autoatendimento e assim por diante.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | AuditLog.Read.All e Directory.Read.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte   |
|Aplicativo | AuditLog.Read.All e Directory.Read.All | 

> [!IMPORTANT]
> Essa API tem um [problema conhecido](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports) e atualmente requer consentimento para as permissões **AuditLog.Read.All** e **Directory.Read.All** .

Além disso, os aplicativos devem ser [corretamente registrados](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta. Para obter detalhes sobre como usar esses parâmetros, consulte [parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e [um objeto directoryAudit](../resources/directoryaudit.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryaudit-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-directoryaudit-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Directory_504a302a-8f2d-418d-b7df-bf77de6ed831_M1N6X_27777783",
    "category": "UserManagement",
    "correlationId": "504a302a-8f2d-418d-b7df-bf77de6ed831",
    "result": "success",
    "resultReason": "",
    "activityDisplayName": "Update user",
    "activityDateTime": "2022-06-21T23:25:00.1458248Z",
    "loggedByService": "Core Directory",
    "operationType": "Update",
    "userAgent": null,
    "initiatedBy": {
        "app": null,
        "user": {
            "id": "2c940657-1026-4386-bcfd-3176637ba01f",
            "displayName": "Test Admin",
            "userPrincipalName": "tadmin@contoso.com",
            "ipAddress": "",
            "userType": "Member",
            "homeTenantId": null,
            "homeTenantName": null
        }
    },
    "targetResources": [
        {
            "id": "2c940657-1026-4386-bcfd-3176637ba01f",
            "displayName": "Test User",
            "type": "User",
            "userPrincipalName": "tuser@contoso.com",
            "groupType": null,
            "modifiedProperties": [
                {
                    "displayName": "StrongAuthenticationMethod",
                    "oldValue": "[{\"MethodType\":6,\"Default\":true},{\"MethodType\":7,\"Default\":false}]",
                    "newValue": "[{\"MethodType\":7,\"Default\":false},{\"MethodType\":6,\"Default\":true},{\"MethodType\":0,\"Default\":false},{\"MethodType\":5,\"Default\":false}]"
                },
                {
                    "displayName": "Included Updated Properties",
                    "oldValue": null,
                    "newValue": "\"StrongAuthenticationMethod\""
                },
                {
                    "displayName": "TargetId.UserType",
                    "oldValue": null,
                    "newValue": "\"Member\""
                }
            ]
        }
    ],
    "additionalDetails": [
        {
            "key": "UserType",
            "value": "Member"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
