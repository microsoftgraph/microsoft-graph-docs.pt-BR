---
title: Obter groupSetting
description: Recupere as propriedades de um objeto de configuração de grupo específico.
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 885408ec1e6cfad786d7c07f422f8e975955c3dc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209377"
---
# <a name="get-groupsetting"></a>Obter groupSetting

Namespace: microsoft.graph

Recupere as propriedades de um objeto de configuração de grupo específico. A configuração pode ser uma configuração específica de grupo ou nível de locatário.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="list-tenant-wide-settings"></a>Listar configurações de todo o locatário

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Directory.Read.All, Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Directory.Read.All, Directory.ReadWrite.All |

### <a name="list-group-specific-settings"></a>Listar configurações específicas do grupo

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Group.Read.All, Group.ReadWrite.All         |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Group.Read.All, Group.ReadWrite.All         |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

Obtenha uma configuração de todo o locatário.

```http
GET /groupSettings/{groupSettingId}
```

<!-- { "blockType": "ignored" } -->

Obter uma configuração específica do grupo.

```http
GET /groups/{groupId}/settings/{groupSettingId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e [um objeto groupSetting](../resources/groupsetting.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-a-group-setting-for-a-specific-group"></a>Exemplo 1: Obter uma configuração de grupo para um grupo específico

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/05aa6a98-956a-45c0-b13b-88076a23f2cd/settings/a06fa228-3042-4662-bd09-33e298da1afe
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings/$entity",
    "id": "a06fa228-3042-4662-bd09-33e298da1afe",
    "displayName": "Group.Unified.Guest",
    "templateId": "08d542b9-071f-4e16-94b0-74abb372e3d9",
    "values": [
        {
            "name": "AllowToAddGuests",
            "value": "false"
        }
    ]
}
```

### <a name="example-2-get-the-group-settings-for-all-microsoft-365-groups"></a>Exemplo 2: Obter as configurações de grupo para todos os Microsoft 365 grupos

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_groupsettings_tenantwide"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings/84af2ca5-c274-41bf-86e4-6e374ec4def6
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-tenantwide-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-tenantwide-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-tenantwide-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-tenantwide-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-tenantwide-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-tenantwide-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-tenantwide-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-tenantwide-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-tenantwide-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-tenantwide-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings/$entity",
    "id": "84af2ca5-c274-41bf-86e4-6e374ec4def6",
    "displayName": "Group.Unified",
    "templateId": "62375ab9-6b52-47ed-826b-58e47e0e304b",
    "values": [
        {
            "name": "EnableMIPLabels",
            "value": "true"
        },
        {
            "name": "CustomBlockedWordsList",
            "value": ""
        },
        {
            "name": "EnableMSStandardBlockedWords",
            "value": "true"
        },
        {
            "name": "ClassificationDescriptions",
            "value": ""
        },
        {
            "name": "DefaultClassification",
            "value": ""
        },
        {
            "name": "PrefixSuffixNamingRequirement",
            "value": "[Contoso-][GroupName]"
        },
        {
            "name": "AllowGuestsToBeGroupOwner",
            "value": "false"
        },
        {
            "name": "AllowGuestsToAccessGroups",
            "value": "true"
        },
        {
            "name": "GuestUsageGuidelinesUrl",
            "value": "https://privacy.contoso.com/privacystatement"
        },
        {
            "name": "GroupCreationAllowedGroupId",
            "value": ""
        },
        {
            "name": "AllowToAddGuests",
            "value": "true"
        },
        {
            "name": "UsageGuidelinesUrl",
            "value": ""
        },
        {
            "name": "ClassificationList",
            "value": ""
        },
        {
            "name": "EnableGroupCreation",
            "value": "true"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
