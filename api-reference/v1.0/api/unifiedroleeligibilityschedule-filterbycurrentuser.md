---
title: 'unifiedRoleEligibilitySchedule: filterByCurrentUser'
description: Recupere os agendamentos de eligibilidades de função para as quais o usuário conectado é a entidade de segurança.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3b4825281952ff636a9a79c5a08d1ac49f16e3b1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439120"
---
# <a name="unifiedroleeligibilityschedule-filterbycurrentuser"></a>unifiedRoleEligibilitySchedule: filterByCurrentUser
Namespace: microsoft.graph

Recupere os agendamentos de eligibilidades de função para as quais o usuário conectado é a entidade de segurança.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory |
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a>Parâmetros de função
Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|on|roleAssignmentScheduleFilterByCurrentUserOptions| Os valores possíveis são `principal`, `unknownFutureValue`.|

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte aos `$select`parâmetros de consulta , `$filter`e `$expand` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).


## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma [coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedulethis.filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser(on='principal')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleeligibilityschedulethisfilterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleeligibilityschedulethisfilterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleeligibilityschedulethisfilterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleeligibilityschedulethisfilterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/unifiedroleeligibilityschedulethisfilterbycurrentuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/unifiedroleeligibilityschedulethisfilterbycurrentuser-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilitySchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(unifiedRoleEligibilitySchedule)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.unifiedRoleEligibilitySchedule",
            "id": "77f71919-62f3-4d0c-9f88-0a0391b665cd",
            "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
            "directoryScopeId": "/",
            "appScopeId": null,
            "createdUsing": "77f71919-62f3-4d0c-9f88-0a0391b665cd",
            "createdDateTime": "2022-04-12T14:44:50.287Z",
            "modifiedDateTime": "0001-01-01T08:00:00Z",
            "status": "Provisioned",
            "memberType": "Direct",
            "scheduleInfo": {
                "startDateTime": "2022-04-12T14:44:50.287Z",
                "recurrence": null,
                "expiration": {
                    "type": "afterDateTime",
                    "endDateTime": "2024-04-10T00:00:00Z",
                    "duration": null
                }
            }
        }
    ]
}
```

