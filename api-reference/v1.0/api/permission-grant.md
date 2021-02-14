---
author: learafa
title: Conceder permissão
description: Conceder uma lista de usuários acesso para usar o link especificado
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9a2ce74ff01293f6546c34d91a0545e2a228bc96
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238642"
---
# <a name="permission-grant"></a>permission: grant

Namespace: microsoft.graph

Conceda aos usuários acesso a um link representado por uma [permissão.][]

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
| destinatários         | Collection([driveRecipient][]) | Uma coleção de destinatários que receberão acesso.
| funções              | Collection(String)             | Se o link for um link de "acesso existente", especifica as funções a serem concedidas aos usuários. Caso contrário, deve corresponder à função do link.

Para uma lista de funções disponíveis, consulte valores [de propriedade de funções.](../resources/permission.md#roles-property-values)

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção [de][] permissões no corpo da resposta.

Uma [permissão][] que representa o link atualizado sempre será retornada no conjunto de resultados de sucesso. O link atualizado pode ser identificado pela presença de uma faceta 'link' contendo a propriedade 'scope'. Em alguns casos, pode ser possível que o link atualizado tenha uma URL diferente do link original, caso em que a nova URL deve ser usada.

Leia o tópico [Respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.


## <a name="example"></a>Exemplo

Este exemplo concede aos usuários john@contoso.com e ryan@external.com acesso a um link de compartilhamento sem modificar outras permissões existentes no link.

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "permission-grant", "scopes": "files.readwrite", "target": "action" } -->

```json
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

---


### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
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

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

Se o link for um link [de acesso](../resources/permission.md) existente, permissões adicionais serão retornadas representando o seguinte:

- Permissões de tipo de usuário que representam destinatários que tiveram acesso concedido com êxito. Eles podem ser identificados pela presença da **propriedade grantedTo.**
- Permissões de tipo de link que representam convites que precisam ser enviados a usuários externos não reconhecedos para que eles tenham acesso. Eles podem ser identificados pela presença de uma [faceta](../resources/sharinginvitation.md) de convite. Essas entradas conterão um [link][sharing-link] com a URL do convite, e a coleção grantedToIdentities indicará os usuários para os quais o link deve ser enviado.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
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

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.



[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[permission]: ../resources/permission.md
[sharing-link]: ../resources/sharinglink.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->

