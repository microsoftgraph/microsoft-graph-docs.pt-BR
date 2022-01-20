---
title: Criar contato
description: Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3d3f7f2ff6789b292f72cb5711c82c63da299089
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101373"
---
# <a name="create-contact"></a>Criar contato

Namespace: microsoft.graph

Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Contacts.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Contacts.ReadWrite    |
|Aplicativo | Contacts.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-contact-from-contactfolder-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-contact-from-contactfolder-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. 

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

