---
title: Lista groupSettingTemplates
description: Recupere uma lista de objetos groupSettingTemplates disponíveis.
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a190f42e65a974907bcaa2ff657b8bd1090ebb8b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209314"
---
# <a name="list-groupsettingtemplates"></a>Lista groupSettingTemplates

Namespace: microsoft.graph

Os modelos de configuração de grupo representam um conjunto de modelos dos quais as configurações de grupo podem ser criadas e usadas em um locatário. Essa operação recupera a lista de objetos groupSettingTemplates disponíveis.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Directory.Read.All, Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /groupSettingTemplates
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

> **Observação:** $filter não é suportado.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplates-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplates-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplates-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplates-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettingtemplates-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettingtemplates-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta

Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
  "value": [
    {
      "id": "08d542b9-071f-4e16-94b0-74abb372e3d9",
      "deletedDateTime": null,
      "displayName": "Group.Unified.Guest",
      "description": "Settings for a specific Unified Group",
      "values": [
        {
          "name": "AllowToAddGuests",
          "type": "System.Boolean",
          "defaultValue": "true",
          "description": "Flag indicating if guests are allowed in a specific Unified Group."
        }
      ]
    },
    {
      "id": "80661d51-be2f-4d46-9713-98a2fcaec5bc",
      "deletedDateTime": null,
      "displayName": "Prohibited Names Settings",
      "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for managing tenant-wide prohibited names settings.",
      "values": [
        {
          "name": "CustomBlockedSubStringsList",
          "type": "System.String",
          "defaultValue": "",
          "description": "A comma delimited list of substring reserved words to block for application display names."
        },
        {
          "name": "CustomBlockedWholeWordsList",
          "type": "System.String",
          "defaultValue": "",
          "description": "A comma delimited list of reserved words to block for application display names."
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
