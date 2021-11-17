---
title: Listar tenantGroups
description: Obter uma lista dos objetos tenantGroup e suas propriedades.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 4c9af2b622845a596a9b2489c8b4066588b3f847
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981052"
---
# <a name="list-tenantgroups"></a>Listar tenantGroups
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos objetos [tenantGroup](../resources/managedtenants-tenantgroup.md) e suas propriedades.

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
GET /tenantRelationships/managedTenants/tenantGroups
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

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [tenantGroup](../resources/managedtenants-tenantgroup.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenantgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantGroups
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenantgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenantgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenantgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenantgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-tenantgroup-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantGroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantGroups",
    "value": [
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "displayName": "Default",
            "allTenantsIncluded": true,
            "tenantIds": [],
            "managementIntents": [
                {
                    "managementIntentId": "586895ab-8a59-4b79-be25-b06949a819bb",
                    "managementIntentDisplayName": "Default Baseline",
                    "managementTemplates": [
                        {
                            "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                            "displayName": "Baseline - Block Legacy Authentication",
                            "category": "identity"
                        },
                        {
                            "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                            "displayName": "Baseline - Require MFA for Admins",
                            "category": "identity"
                        },
                        {
                            "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                            "displayName": "Baseline - Require MFA for end users",
                            "category": "identity"
                        },
                        {
                            "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
                            "displayName": "Baseline - Enroll devices in MEM",
                            "category": "devices"
                        },
                        {
                            "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                            "displayName": "Baseline - Setup Compliance Policy for Windows 10 devices",
                            "category": "devices"
                        },
                        {
                            "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                            "displayName": "Baseline - Setup Microsoft Defender Antivirus Policy for Windows 10 devices",
                            "category": "devices"
                        }
                    ]
                }
            ],
            "managementActions": [
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b"
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5"
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2"
                },
                {
                    "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                    "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6"
                },
                {
                    "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                    "managementActionId": "55f8da1a-4eec-4fb2-9c58-4c4b3cdf7222"
                },
                {
                    "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
                    "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9"
                }
            ]
        }
    ]
}
```
