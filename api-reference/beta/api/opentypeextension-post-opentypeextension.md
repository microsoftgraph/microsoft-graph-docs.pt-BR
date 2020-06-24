---
title: Criar extensão aberta
description: Criar uma extensão aberta (objeto openTypeExtension) e adicionar propriedades personalizadas
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: d6c06370494e9e89fa77d40a0889819f47f21d2c
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863366"
---
# <a name="create-open-extension"></a>Criar extensão aberta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma extensão aberta (objeto[openTypeExtension](../resources/opentypeextension.md) ) e adicione Propriedades personalizadas em uma instância nova ou existente de um recurso com suporte.

> **Observação:** Se você estiver criando extensões abertas em recursos do Outlook, confira **considerações específicas do Outlook** no [tipo de recurso openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).

## <a name="permissions"></a>Permissões

Dependendo do recurso para o qual você está criando a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Recurso com suporte | Delegada (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Application |
|:-----|:-----|:-----|:-----|
| [device](../resources/device.md) | Directory.AccessAsUser.All | Sem suporte | Device.ReadWrite.All |
| [evento](../resources/event.md) | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| [grupo](../resources/group.md) | Group.ReadWrite.All | Sem suporte | Group.ReadWrite.All |
| [evento de grupo](../resources/event.md) | Group.ReadWrite.All | Sem suporte | Sem suporte |
| [postagem de grupo](../resources/post.md) | Group.ReadWrite.All | Sem suporte | Group.ReadWrite.All |
| [mensagem](../resources/message.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite | 
| [organização](../resources/organization.md) | Organization.ReadWrite.All | Sem suporte | Organization.ReadWrite.All |
| [contato pessoal](../resources/contact.md) | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [user](../resources/user.md) | User.ReadWrite | User.ReadWrite | User.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

### <a name="create-an-extension-in-a-new-resource-instance"></a>Crie uma extensão em uma nova instância de recurso

Use a mesma solicitação REST usada para criar a instância.

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

>**Observação:** Esta sintaxe acima mostra algumas maneiras comuns de criar as instâncias de recursos com suporte. Todas as outras sintaxes POST que permitem criar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.

Confira a seção [Solicitar corpo](#request-body) sobre a inclusão de propriedades da nova instância do recurso _e a extensão_ no corpo da solicitação.

### <a name="create-an-extension-in-an-existing-resource-instance"></a>Crie uma extensão em uma instância de recurso existente

Identifique a instância do recurso na solicitação e faça um `POST` para a propriedade de navegação **extensions**.

<!-- { "blockType": "ignored" } -->
```http
POST /administrativeunits/{id}/extensions
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

>**Observação:** Esta sintaxe mostra algumas maneiras comuns de identificar uma instância do recurso, para criar uma extensão nele. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.

Confira a seção [Solicitar corpo](#request-body) sobre como incluir _a extensão_ no corpo da solicitação.

## <a name="path-parameters"></a>Parâmetros do caminho

|**Parâmetro**|**Tipo**|**Descrição**|
|:-----|:-----|:-----|
|id|string|A unique identifier for an object in the corresponding collection. Required.|

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Valor |
|:---------------|:----------|
| Autorização | Bearer {token}. Required. |
| Content-Type | application/json |

## <a name="request-body"></a>Corpo da solicitação

Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.

| Name       | Valor |
|:---------------|:----------|
| @odata.type | microsoft.graph.openTypeExtension |
| extensionName | %unique_string% |

Ao criar uma extensão em uma _nova_ instância de recursos, além de novos objetos **openTypeExtension**, fornecem uma representação JSON das propriedades relevantes para criar uma instância de recurso deste tipo.

## <a name="response"></a>Resposta

### <a name="response-code"></a>Código da resposta

Dependendo da operação, o código de resposta pode ser `201 Created` ou `202 Accepted`.

Quando você cria uma extensão usando a mesma operação usada para criar uma instância de recurso, a operação retorna o mesmo código de resposta retornado quando você usa a operação para criar a instância do recurso sem a extensão.
Consulte os tópicos correspondentes para criar a instância conforme listado [cima](#create-an-extension-in-a-new-resource-instance).

### <a name="response-body"></a>Corpo da resposta

| Cenário       | Recurso  | Corpo da resposta |
|:---------------|:----------|:--------------|
| Criar uma extensão ao criar explicitamente uma _nova_ instância de recurso | [contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md) | Inclui a nova instância expandida com o objeto [openTypeExtension](../resources/opentypeextension.md). |
| Criando uma extensão ao criar implicitamente uma instância de recursos | [postagem](../resources/post.md) | A resposta inclui somente um código de resposta, mas não um corpo de resposta. |
| Criar uma extensão em uma instância de recurso _existente_ | Todos os recursos com suporte | Inclui o objeto **openTypeExtension**. |

## <a name="example"></a>Exemplo

### <a name="request-1"></a>Solicitação 1

The first example creates a message and an extension in the same call. The request body includes the following:

- As propriedades **subject**, **body** e **toRecipients** típicas de uma nova mensagem.
- E para a extensão:

  - O tipo `microsoft.graph.openTypeExtension`.
  - O nome da extensão "Com.Contoso.Referral".
  - Dados adicionais a serem armazenados como três propriedades personalizadas no conteúdo JSON: `companyName`, `expirationDate` e `dealValue`.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-Type: application/json

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a>Resposta 1

Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:

- A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.
- A propriedade padrão **extensionName** especificada na solicitação.
- Os dados personalizados especificados na solicitação, armazenados como 3 propriedades personalizadas.

Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#microsoft.graph.openTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
      "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a>Solicitação 2

The second example creates an extension in the specified message. The request body includes the following for the extension:

- O tipo `microsoft.graph.openTypeExtension`.
- O nome da extensão "Com.Contoso.Referral".
- Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions
Content-Type: application/json

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a>Resposta 2

Here is the response for the second example. The response body includes the following for the new extension:

- A propriedade padrão **extensionName**.
- A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.
- Os dados personalizados a serem armazenados.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a>Solicitação 3

The third example creates an extension in the specified group event. The request body includes the following for the extension:

- O tipo `microsoft.graph.openTypeExtension`.
- O nome da extensão "Com.Contoso.Deal".
- Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions
Content-type: application/json

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a>Resposta 3

Veja a seguir a resposta da terceira solicitação de exemplo.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a>Solicitação 4

The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:

- O tipo `microsoft.graph.openTypeExtension`.
- O nome da extensão "Com.Contoso.HR".
- Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-4"></a>Resposta 4

Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```

****

### <a name="request-5"></a>Solicitação 5

The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:

- O tipo `microsoft.graph.openTypeExtension`.
- O nome da extensão "Com.Contoso.HR".
- Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations
Content-type: application/json

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "microsoft.graph.openTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-5"></a>Resposta 5

Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.

Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
