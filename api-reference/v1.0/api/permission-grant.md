---
author: learafa
title: Conceder permissão
description: Conceder uma lista de usuários acesso para usar o link especificado
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6c966424dc1358e8a41a9015d3beaed0154b7468
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978873"
---
# <a name="permission-grant"></a>permission: grant

Namespace: microsoft.graph

Conceda aos usuários acesso a um link representado por uma [permissão][].

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                   | Permissões (da com menos para a com mais privilégios)              |
|:----------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte    |
|Aplicativo | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição  |
|:------------- |:------------ |
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| Parâmetro          | Tipo                           | Descrição
|:-------------------|:-------------------------------|:-------------------------
| destinatários         | Coleção([driveRecipient][]) | Uma coleção de destinatários que receberão acesso.
| funções              | Collection(String)             | Se o link for um link de "acesso existente", especificará funções a serem concedidas aos usuários. Caso contrário, deverá corresponder à função do link.

Para ver uma lista de funções disponíveis, consulte [roles property values](../resources/permission.md#roles-property-values).

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção [de][] permissões no corpo da resposta.

Uma [permissão][] que representa o link atualizado sempre será retornada no conjunto de resultados sobre o sucesso. O link atualizado pode ser identificado pela presença de uma faceta 'link' contendo a propriedade 'escopo'. Em alguns casos, pode ser possível que o link atualizado tenha uma URL diferente do link original, nesse caso, a nova URL deve ser usada.

Leia o tópico [Respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.


## <a name="example"></a>Exemplo

Este exemplo concede aos usuários john@contoso.com e ryan@external.com acesso a um link de compartilhamento sem modificar outras permissões existentes no link.

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "permission-grant", "scopes": "files.readwrite", "target": "action" } -->

```http
POST https://graph.microsoft.com/v1.0/shares/{encoded-sharing-url}/permission/grant
Content-type: application/json

{
  "recipients": [
    {
      "email": "john@contoso.com"
    },
    {
      "email": "ryan@external.com"
    }
  ],
  "roles": ["read"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-grant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-grant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-grant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permission-grant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/permission-grant-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "5fab944a-47ec-48d0-a9b5-5178a926d00f",
      "link": {
        "preventsDownload": false,
        "scope": "users",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/design/EZexPoDjW4dMtKFUfAl6BK4BvIUuss52hLYzihBfx-PD6Q"
      },
      "roles": [
        "read"
      ]
    }
  ]
}
```

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

Se o link for um link [de acesso](../resources/permission.md) existente, permissões adicionais serão retornadas representando o seguinte:

- Permissões de tipo de usuário que representam destinatários que tiveram acesso concedido com êxito. Eles podem ser identificados pela presença da **propriedade grantedTo.**
- Permissões de tipo de link que representam convites que precisam ser enviados a usuários externos não reconhecedos para que eles obtenham acesso. Eles podem ser identificados pela presença de uma faceta [de](../resources/sharinginvitation.md) convite. Essas entradas conterão um [link][sharing-link] com a URL do convite e a coleção grantedToIdentities indicará os usuários aos quais o link deve ser enviado.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "00000000-0000-0000-0000-000000000000",
      "link": {
        "preventsDownload": false,
        "scope": "existingAccess",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/teams/design/shareddocs/Document.docx"
      },
      "roles": [
        "read"
      ]
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "John Smith",
          "email": "john@contoso.com",
          "id": "47aecee2-d061-4730-8ecb-4c61360441ae"
        }
      },
      "id": "aTowIy5mfG1lbWJlcnNoaXB8bGltaXRlZDJAa2xhbW9kYi5vbm1pY3Jvc29mdC5jb20",
      "roles": [
        "read"
      ]
    },
    {
      "grantedToIdentities": [
        {
          "user": {
            "email": "ryan@external.com"
          }
        }
      ],
      "invitation": {
        "signInRequired": true
      },
      "roles": [
        "read"
      ],
      "link": {
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/teams/design/EZexPoDjW4dMtKFUfAl6BK4Bw_F7gFH63O310A7lDtK0mQ"
      }
    }
  ]
}

```

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.



[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[permissão]: ../resources/permission.md
[sharing-link]: ../resources/sharinglink.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath&quot;: &quot;Sharing/Add permissions"
} -->

