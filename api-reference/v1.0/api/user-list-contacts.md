---
title: Listar contatos
description: Obter uma coleção de contatos da pasta padrão de contatos do usuário conectado.
author: kevinbellinger
ms.localizationpriority: high
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 125c0b509e5d93e1b4e36adcb014a5d346f11d75
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025696"
---
# <a name="list-contacts"></a>Listar contatos

Namespace: microsoft.graph

Obter uma coleção de contatos da pasta padrão de contatos do usuário conectado.

Há duas situações em que um aplicativo pode obter contatos na pasta de contatos de outro usuário:

* Se o aplicativo tiver permissões de aplicativo ou
* Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de contato com esse usuário ou se tiver concedido acesso delegado a esse usuário. Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Contacts.Read, Contacts.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Contacts.Read, Contacts.ReadWrite    |
|Aplicativo | Contacts.Read, Contacts.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP

Para obter todos os contatos na caixa de correio do usuário:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

Para obter os contatos em uma pasta específica na caixa de correio do usuário:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolders/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Você pode usar o `$filter`parâmetro de consulta para filtrar contatos com base em seus endereços de email:

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

Observe que você pode usar `$filter`, `any`, e o `eq` operador apenas na subpropriedade de **endereço** das instâncias em uma coleção **emailAddresses**. Ou seja, você não pode filtrar o **nome** ou qualquer outra subpropriedade de uma instância de **emailAddresses**, nem pode aplicar qualquer outro operador ou função com `filter`, como `ne`, `le` e `startswith()`.

Para obter informações gerais sobre o `$filter`parâmetro de consulta, acesse [Parâmetros de consulta OData](/graph/query-parameters).



## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contacts
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a>Resposta
Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

