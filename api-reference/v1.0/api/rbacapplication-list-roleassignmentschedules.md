---
title: Listar roleAssignmentSchedules
description: Obtenha os agendamentos para operações de atribuição de função ativa.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3a15def5103e2371a968afca6a40ccde7ca43e98
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133875"
---
# <a name="list-roleassignmentschedules"></a>Listar roleAssignmentSchedules
Namespace: microsoft.graph

Obtenha os agendamentos para operações de atribuição de função ativa.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory   |
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte aos `$select`parâmetros de consulta , `$filter`e `$expand` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção de [objetos unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedule"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentSchedules
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentSchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentSchedules",
    "value": [
        {
            "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
            "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
            "directoryScopeId": "/",
            "appScopeId": null,
            "createdUsing": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
            "createdDateTime": "2022-04-11T11:50:06.343Z",
            "modifiedDateTime": null,
            "status": "Provisioned",
            "assignmentType": "Assigned",
            "memberType": "Direct",
            "scheduleInfo": {
                "startDateTime": "2022-04-11T11:50:06.343Z",
                "recurrence": null,
                "expiration": {
                    "type": "noExpiration",
                    "endDateTime": null,
                    "duration": null
                }
            }
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEAWz5Gtet_xOv8wxvTtTpfg-1",
            "principalId": "6be4b305-b75e-4efc-bfcc-31bd3b53a5f8",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "directoryScopeId": "/",
            "appScopeId": null,
            "createdUsing": null,
            "createdDateTime": null,
            "modifiedDateTime": null,
            "status": "Provisioned",
            "assignmentType": "Assigned",
            "memberType": "Direct",
            "scheduleInfo": {
                "startDateTime": "2022-04-11T17:11:50.8825697Z",
                "recurrence": null,
                "expiration": {
                    "type": "noExpiration",
                    "endDateTime": null,
                    "duration": null
                }
            }
        }
    ]
}
```

