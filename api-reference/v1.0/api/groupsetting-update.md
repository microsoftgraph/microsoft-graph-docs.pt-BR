---
title: Atualizar groupSetting
description: Atualize as propriedades de um objeto de configuração de grupo específico.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 693b1bc0fe65c79defef73589a92554ab651bd28
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63670513"
---
# <a name="update-groupsetting"></a>Atualizar groupSetting

Namespace: microsoft.graph

Atualize as propriedades de um [objeto groupSetting](../resources/groupsetting.md) para configurações [](../resources/group.md) de grupo em todo o locatário ou uma configuração de grupo específica.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
Atualize uma configuração de todo o locatário.
```http
PATCH /groupSettings/{groupSettingId}
```

<!-- { "blockType": "ignored" } -->
Atualize uma configuração específica do grupo.
```http
PATCH /groups/{groupId}/settings/{groupSettingId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome | Descrição |
|:-----------|:-----------|
| Autorização  | {token}. Obrigatório. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. 

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| values | [coleção settingValue](../resources/settingvalue.md) | O conjunto atualizado de valores. Você deve incluir todo o conjunto de coleções. Não é possível atualizar um único conjunto de valores. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-a-tenant-wide-group-setting"></a>Exemplo 1: atualizar uma configuração de grupo em todo o locatário

Neste exemplo, é `84af2ca5-c274-41bf-86e4-6e374ec4def6` o identificador do objeto **groupSetting** em todo o locatário.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenant_groupsetting"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/groupSettings/84af2ca5-c274-41bf-86e4-6e374ec4def6
Content-type: application/json

{
    "values": [
        {
            "name": "AllowToAddGuests",
            "value": "false"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-tenant-groupsetting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a>Exemplo 2: Atualizar uma configuração de grupo específica

Neste exemplo, é `0167b5af-f3d1-4910-82d2-398747fa381c` o identificador do grupo e `fa6df613-159b-4f94-add2-7093f961900b` é o identificador do objeto groupSetting.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/groups/0167b5af-f3d1-4910-82d2-398747fa381c/settings/fa6df613-159b-4f94-add2-7093f961900b
Content-type: application/json

{
  "values": [
    {
      "name": "AllowToAddGuests",
      "value": "true"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-groupsetting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

