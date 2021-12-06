---
title: Listar configurações de grupo
description: Recupere uma lista de objetos de configuração de grupo.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: af51f4fd21e1d17316b08b0ea99f87d315431e57
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027716"
---
# <a name="list-group-settings"></a>Listar configurações de grupo

Namespace: microsoft.graph

Recupere uma lista de objetos de configuração de grupo.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->

Listar configurações de grupo ou de locatários.

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

>**Observação:** $filter não é suportado.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome | Descrição |
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.
## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta

Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings",
  "value": [
    {
      "id": "f0b2d6f5-097d-4177-91af-a24e530b53cc",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

