---
title: Listar roleAssignmentScheduleInstances
description: Obtenha as instâncias de atribuições de função ativas em seu locatário.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a2a6c8f8458e396423fce589c42c196cb766997f
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133892"
---
# <a name="list-roleassignmentscheduleinstances"></a>Listar roleAssignmentScheduleInstances
Namespace: microsoft.graph

Obtenha as instâncias de atribuições de função ativas em seu locatário. As atribuições ativas incluem aquelas feitas por meio de [atribuições e solicitações](rbacapplication-post-roleassignmentschedulerequests.md) de ativação e diretamente por meio da [API de atribuições de função](../resources/unifiedroleassignment.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances
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

Se bem-sucedido, este método `200 OK` retorna um código de resposta e uma coleção de [objetos unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleInstances
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleInstances",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEAWz5Gtet_xOv8wxvTtTpfg-1",
            "principalId": "6be4b305-b75e-4efc-bfcc-31bd3b53a5f8",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "directoryScopeId": "/",
            "appScopeId": null,
            "startDateTime": null,
            "endDateTime": null,
            "assignmentType": "Assigned",
            "memberType": "Direct",
            "roleAssignmentOriginId": "lAPpYvVpN0KRkAEhdxReEAWz5Gtet_xOv8wxvTtTpfg-1",
            "roleAssignmentScheduleId": "lAPpYvVpN0KRkAEhdxReEAWz5Gtet_xOv8wxvTtTpfg-1"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEBLS8lac5ONCgpgBiOW-8JQ-1",
            "principalId": "56f2d212-e49c-42e3-8298-0188e5bef094",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "directoryScopeId": "/",
            "appScopeId": null,
            "startDateTime": null,
            "endDateTime": null,
            "assignmentType": "Assigned",
            "memberType": "Direct",
            "roleAssignmentOriginId": "lAPpYvVpN0KRkAEhdxReEBLS8lac5ONCgpgBiOW-8JQ-1",
            "roleAssignmentScheduleId": "lAPpYvVpN0KRkAEhdxReEBLS8lac5ONCgpgBiOW-8JQ-1"
        }
    ]
}
```

