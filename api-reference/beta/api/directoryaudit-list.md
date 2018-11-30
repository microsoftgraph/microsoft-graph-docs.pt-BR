---
title: Lista directoryAudits
description: Fornece a lista de logs de auditoria gerados pelo Windows Azure Active Directory. Inclui os logs de auditoria gerados por vários serviços dentro do Azure Active Directory como usuário, aplicativo, dispositivo e gerenciamento do grupo, privilegiado Identity Management, avaliações de acesso, termos de uso, proteção de identidade, gerenciamento de senhas (SSPR e Admin redefinições de senha ), Etc. de gerenciamento do grupo de auto-atendimento …
ms.openlocfilehash: e607d866443a07f1405260b02a630276951ce310
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033023"
---
# <a name="list-directoryaudits"></a>Lista directoryAudits

Fornece a lista de logs de auditoria gerados pelo Windows Azure Active Directory. Inclui os logs de auditoria gerados por vários serviços dentro do Azure Active Directory como usuário, aplicativo, dispositivo e gerenciamento do grupo, privilegiado Identity Management, avaliações de acesso, termos de uso, proteção de identidade, gerenciamento de senhas (SSPR e Admin redefinições de senha ), Etc. de gerenciamento do grupo de auto-atendimento …

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | AuditLog.Read.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte   |
|Aplicativo | AuditLog.Read.All | 

Além disso, os aplicativos devem ser [registrado corretamente](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para o Windows Azure AD.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos seguintes Parâmetros de consulta OData para ajudar a personalizar a resposta. Verifique [Os parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para como usar esses parâmetros.

|Nome     |Descrição                            |Exemplo|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|Filtra os resultados (linhas). |/`auditLogs/directoryAudits?&$filter=createdDateTime le 2018-01-24`
|[$top](/graph/query-parameters#top-parameter)|Define o tamanho de página de resultados.|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|Recupera que a próxima página de resultados do resultado define que ocupar várias páginas.|`auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>Lista de atributos suportados pelo parâmetro $filter
|Nome do atributo |Operadores com suporte|
|:----------------|:------|
|activityDisplayName| EQ, startswith|
|activityDateTime| EQ, ge, le|
|loggedByService|eq|
|id/de usuário de initiatedBy|eq|
|displayName/de usuário de initiatedBy| eq|
|initiatedBy/usuário/userPrincipalName| EQ, startswith|
|initiatedBy/app/appId| eq|
|initiatedBy/app/appDisplayName| eq|
|targetResources/any(t: t/id)| eq|
|targetResources/any(t:t/displayName)| EQ, startswith|
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [directoryAudit](../resources/directoryaudit.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "get_directoryaudits"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 271
```
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryAudits
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
                "id": "7283X9ae-1a37-4937-9aex-e35d964db09b",
                "displayName": "Jamie Doe",
                "userPrincipalName": "jdoe@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "@odata.type": "#microsoft.graph.TargetResourceGroup",
            "id": "ef7x527d-6x92-42x4-8x6d-cfxfdfx57f95",
            "displayName": "Lynda.com",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"
            }],
            "groupType": "unifiedGroups"
        }, {
            "@odata.type": "#microsoft.graph.targetResourceUser",
            "id": "1f0ex8f5-3x61-4x6b-9x50-d4xx572f2bb7",
            "displayName": null,
            "modifiedProperties": [],
            "userPrincipalName": "jdoe@contoso.com"
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
  "tocPath": ""
}-->