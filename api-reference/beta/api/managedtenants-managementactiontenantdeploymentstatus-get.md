---
title: Obter managementActionTenantDeploymentStatus
description: Leia as propriedades e as relações de um objeto managementActionTenantDeploymentStatus.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 72cee53d2a1b768e13eaa778971ff026c579c741
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011902"
---
# <a name="get-managementactiontenantdeploymentstatus"></a>Obter managementActionTenantDeploymentStatus
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de [um objeto managementActionTenantDeploymentStatus.](../resources/managedtenants-managementactiontenantdeploymentstatus.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ManagedTenants.Read.All, ManagedTenants.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_managementactiontenantdeploymentstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-managementactiontenantdeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-managementactiontenantdeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-managementactiontenantdeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-managementactiontenantdeploymentstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-managementactiontenantdeploymentstatus-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionTenantDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/$entity",
    "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "statuses": [
        {
            "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
            "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
            "status": "completed",
            "workloadActionDeploymentStatuses": [
                {
                    "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                    "status": "completed",
                    "deployedPolicyId": "949e8893-68fb-4c9d-b8a0-13c229a7e397",
                    "lastDeploymentDateTime": "2021-06-22T04:09:20.3054223Z",
                    "error": null
                }
            ]
        },
        {
            "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
            "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
            "status": "completed",
            "workloadActionDeploymentStatuses": [
                {
                    "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                    "status": "completed",
                    "deployedPolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
                    "lastDeploymentDateTime": "2021-06-22T17:01:44.851214Z",
                    "error": null
                }
            ]
        }
    ]
}
```
