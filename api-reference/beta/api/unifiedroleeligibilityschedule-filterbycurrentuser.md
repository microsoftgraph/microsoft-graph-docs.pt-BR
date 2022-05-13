---
title: 'unifiedRoleEligibilitySchedule: filterByCurrentUser'
description: Obter uma lista dos objetos unifiedRoleEligibilitySchedule e suas propriedades filtradas por uma entidade de usuário específica
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a30a813f73bcac6da31073a0e0fb9e59174a6c31
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399191"
---
# <a name="unifiedroleeligibilityschedule-filterbycurrentuser"></a>unifiedRoleEligibilitySchedule: filterByCurrentUser
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md) e suas propriedades associadas a um objeto principal específico.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory |
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser(on='principal')
```

## <a name="function-parameters"></a>Parâmetros de função
A tabela a seguir mostra os parâmetros que podem ser usados com esse método.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|on|roleEligibilityScheduleFilterByCurrentUserOptions|O usuário conectado no momento. O valor permitido é `principal`.|

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedule_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser(on='principal')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleeligibilityschedule-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleeligibilityschedule-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleeligibilityschedule-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleeligibilityschedule-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/unifiedroleeligibilityschedule-filterbycurrentuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/unifiedroleeligibilityschedule-filterbycurrentuser-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

A seguir está um exemplo da resposta que mostra um agendamento de qualificação que é por meio de uma atribuição de grupo.
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(unifiedRoleEligibilitySchedule)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.unifiedRoleEligibilitySchedule",
            "id": "6938d75d-ad66-4c7d-9028-0c9b00296945",
            "principalId": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
            "directoryScopeId": "/",
            "appScopeId": null,
            "createdUsing": "6938d75d-ad66-4c7d-9028-0c9b00296945",
            "createdDateTime": "2021-08-09T10:15:05.96Z",
            "modifiedDateTime": "0001-01-01T08:00:00Z",
            "status": "Provisioned",
            "memberType": "Direct",
            "scheduleInfo": {
                "startDateTime": "2021-08-09T10:15:05.96Z",
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

