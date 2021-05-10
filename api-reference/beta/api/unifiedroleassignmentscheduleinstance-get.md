---
title: Obter unifiedRoleAssignmentScheduleInstance
description: Leia as propriedades e as relações de um objeto unifiedRoleAssignmentScheduleInstance.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b56dcc6f0171a203a426e88c8c01a81e71a10986
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299094"
---
# <a name="get-unifiedroleassignmentscheduleinstance"></a>Obter unifiedRoleAssignmentScheduleInstance
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleInstance.](../resources/unifiedroleassignmentscheduleinstance.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|PrivilegedAccess.ReadWrite.AzureAD|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|PrivilegedAccess.Read.AzureAD|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstancesId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/unifiedRoleAssignmentScheduleInstances/eb18c026-c026-eb18-26c0-18eb26c018eb
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "principalId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "roleDefinitionId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "directoryScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "appScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "startDateTime": "2020-09-09T21:35:27.91Z",
    "endDateTime": "2020-09-09T21:35:27.91Z",
    "assignmentType": "eligible",
    "memberType": "direct",
    "roleAssignmentOriginId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "roleAssignmentScheduleId": "eb18c026-c026-eb18-26c0-18eb26c018eb"
  }
}
```

