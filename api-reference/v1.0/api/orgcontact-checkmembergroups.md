---
title: 'orgContact: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada. Retorna da lista as IDs de grupo das quais o contato organizacional tem uma associação direta ou transitiva.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1dc4b89e22f2e92e1faf0762c8b56e9bf149dcb5
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945107"
---
# <a name="orgcontact-checkmembergroups"></a>orgContact: checkMemberGroups

Namespace: microsoft.graph

Verifique se há associação na lista de grupos especificada. Retorna da lista as IDs de grupo das quais o contato [organizacional](../resources/orgcontact.md) tem uma associação direta ou transitiva.

Você pode fazer check-up de no máximo 20 grupos por solicitação. Esta função dá suporte Microsoft 365 outros tipos de grupos provisionados no Azure Active Directory (Azure AD).

>[!NOTE]
>Microsoft 365 grupos não podem conter grupos. A associação em um Microsoft 365 grupo é sempre direta.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | OrgContact.Read.All e Group.Read.All, Directory.Read.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | OrgContact.Read.All e Group.Read.All, Directory.Read.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-type   | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|groupIds|Coleção de cadeias de caracteres | Uma lista de IDs de grupo a verificar. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
    "groupId-value1", "groupId-value2" 
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "groupId-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

