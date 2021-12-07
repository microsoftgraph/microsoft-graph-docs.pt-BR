---
title: Lista directoryAudits
description: Descreve o método de lista do recurso directoryAudit (entidade) da API Graph Microsoft.
ms.localizationpriority: medium
author: SarahBar
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: ca9550b54061ed93c6dabe859cde5f58e0025b7a
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322013"
---
# <a name="list-directoryaudits"></a>Lista directoryAudits

Namespace: microsoft.graph

Obter a lista de logs de auditoria gerados por Azure Active Directory. Isso inclui logs de auditoria gerados por vários serviços no Azure AD, incluindo gerenciamento de usuários, aplicativos, dispositivos e grupos, PIM (gerenciamento de identidade privilegiada), análises de acesso, termos de uso, proteção de identidade, gerenciamento de senhas (redefinições de senha de autoatendados e administradores), gerenciamento de grupo de autoatendados e assim por diante.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegada (conta corporativa ou de estudante)     | AuditLog.Read.All e Directory.Read.All    |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | AuditLog.Read.All e Directory.Read.All    |

> [!IMPORTANT]
> Esta API tem um [problema conhecido](/graph//graph/known-issues#license-check-errors-for-azure-ad-activity-reports) e atualmente requer consentimento para as permissões **AuditLog.Read.All** e **Directory.Read.All.**

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/directoryaudits
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query-parameters).

| Parâmetro                                                       | Descrição                                                                   | Exemplo                                                                     |
| :--------------------------------------------------------- | :---------------------------------------------------------------------------- | :-------------------------------------------------------------------------- |
| [\$filter](/graph/query-parameters#filter-parameter)       | Filtra os resultados (linhas).                                                       | `/auditLogs/directoryAudits?&$filter=activityDateTime le 2018-01-24`         |
| [\$Início](/graph/query-parameters#top-parameter)             | Define o tamanho de página de resultados.                                                | `/auditLogs/directoryAudits?$top=1`                                         |
| [\$skiptoken](/graph/query-parameters#skiptoken-parameter) | Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. | `/auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a>Atributos suportados pelo \$ parâmetro filter

| Atributo                                                    | Operadores com suporte |
| :----------------------------------------------------------- | :------------------ |
| activityDisplayName                                          | eq, startswith      |
| activityDateTime                                             | eq, ge, le          |
| loggedByService                                              | eq                  |
| initiatedBy/user/id                                          | eq                  |
| initiatedBy/user/displayName                                 | eq                  |
| initiatedBy/user/userPrincipalName                           | eq, startswith      |
| initiatedBy/app/appId                                        | eq                  |
| initiatedBy/app/displayName                                  | eq                  |
| targetResources/any(t: t/id eq '{value}')                    | eq                  |
| targetResources/any(t:t/displayName eq '{value}')            | eq                  |
| targetResources/any(x: startswith(x/displayName, '{value}')) | startswith          |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
| :------------ | :------------ |
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos directoryAudit](../resources/directoryaudit.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudit-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudit-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudit-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudit-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryaudit-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditlogs/directoryaudits",
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "da159bfb-54fa-4092-8a38-6e1fa7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "728309ae-1a37-4937-9afe-e35d964db09b",
                "displayName": "Audry Oliver",
                "userPrincipalName": "bob@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "id": "ef7e527d-6c92-4234-8c6d-cf6fdfb57f95",
            "displayName": "Example.com",
            "Type": "Group",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"}],
            "groupType": "unifiedGroups"
            }, 
            {
            "id": "1f0e98f5-3161-4c6b-9b50-d488572f2bb7",
            "displayName": null,
            "Type": "User",
            "modifiedProperties": [],
            "userPrincipalName": "bob@contoso.com"
        }],
        "additionalDetails": [{
            "key": "Additional Detail Name",
            "value": "Additional Detail Value"
        }]
    }]
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

