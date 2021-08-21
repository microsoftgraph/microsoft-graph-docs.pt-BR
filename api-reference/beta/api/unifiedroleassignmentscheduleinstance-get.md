---
title: Obter unifiedRoleAssignmentScheduleInstance
description: Leia as propriedades e as relações de um objeto unifiedRoleAssignmentScheduleInstance.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3bc31bfd1ba788c8a823114d22c1dfd0b0db2021
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453300"
---
# <a name="get-unifiedroleassignmentscheduleinstance"></a>Obter unifiedRoleAssignmentScheduleInstance
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleInstance.](../resources/unifiedroleassignmentscheduleinstance.md)

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
GET /roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstancesId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

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

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances/4-PYiFWPHkqVOpuYmLiHa_8KmpPnrkhHmG41_UYRbUY-1
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentscheduleinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentscheduleinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentscheduleinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentscheduleinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignmentScheduleInstances/$entity",
  "id": "4-PYiFWPHkqVOpuYmLiHa_8KmpPnrkhHmG41_UYRbUY-1",
  "principalId": "939a0aff-aee7-4748-986e-35fd46116d46",
  "roleDefinitionId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
  "directoryScopeId": "/",
  "appScopeId": null,
  "startDateTime": null,
  "endDateTime": null,
  "assignmentType": "Assigned",
  "memberType": "Direct",
  "roleAssignmentOriginId": "4-PYiFWPHkqVOpuYmLiHa_8KmpPnrkhHmG41_UYRbUY-1",
  "roleAssignmentScheduleId": "4-PYiFWPHkqVOpuYmLiHa_8KmpPnrkhHmG41_UYRbUY-1"
}
```

