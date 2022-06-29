---
title: Lista directoryAudits
description: Descreve o método de lista do recurso directoryAudit (entidade) do Microsoft API do Graph (versão beta).
ms.localizationpriority: medium
author: SarahBar
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: dd8fe4c8923dac46cd9e9d7854d64015a5319390
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437400"
---
# <a name="list-directoryaudits"></a>Lista directoryAudits

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a lista de logs de auditoria gerados pelo Azure Active Directory. Isso inclui logs de auditoria gerados por vários serviços no Azure AD, incluindo gerenciamento de usuário, aplicativo, dispositivo e grupo, PIM (privileged identity management), revisões de acesso, termos de uso, proteção de identidade, gerenciamento de senha (redefinições de senha de administrador e SSPR) e gerenciamento de grupo de autoatendimento.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | AuditLog.Read.All e Directory.Read.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | AuditLog.Read.All e Directory.Read.All | 

> [!IMPORTANT]
> Essa API tem um [problema conhecido](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports) e atualmente requer consentimento para as permissões **AuditLog.Read.All** e **Directory.Read.All** .

Além disso, os aplicativos devem ser [corretamente registrados](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter detalhes sobre como usar esses parâmetros, consulte [parâmetros de consulta OData](/graph/query-parameters).

|Parâmetro     |Descrição                            |Exemplo|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|Filtra os resultados (linhas). |`/auditLogs/directoryAudits?$filter=activityDateTime le 2018-01-24`<br>`/auditLogs/directoryAudits?$filter=targetResources/any(x: startswith(x/displayName, 'def'))` |
|[$top](/graph/query-parameters#top-parameter)|Define o tamanho de página de resultados.|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.|`/auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a>Atributos compatíveis com $filter parâmetro

|Atributo        |Operadores com suporte|
|:----------------|:------|
|activityDisplayName| eq, startswith|
|activityDateTime| eq, ge, le|
|loggedByService|eq|
|initiatedBy/user/id|eq|
|initiatedBy/user/displayName| eq|
|initiatedBy/user/userPrincipalName| eq, startswith|
|initiatedBy/app/appId| eq|
|initiatedBy/app/displayName| eq|
|targetResources/any(t: t/id)| eq|
|targetResources/any(t:t/displayName)| eq, startswith|

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryAudit](../resources/directoryaudit.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudits"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryaudits-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-directoryaudits-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
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
  "description": "List directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
