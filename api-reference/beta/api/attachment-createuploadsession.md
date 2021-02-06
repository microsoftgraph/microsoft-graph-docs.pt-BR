---
title: 'attachment: createUploadSession'
description: Crie uma sessão de upload para carregar iterativamente intervalos de um arquivo para anexar o arquivo à mensagem especificada.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a6856799c8532f3a0bf428dc7d417f9f29e921a9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128929"
---
# <a name="attachment-createuploadsession"></a>attachment: createUploadSession

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma sessão de upload que permita que um aplicativo carregue iterativamente intervalos de um arquivo, para anexar o arquivo a um item do Outlook. O item pode ser uma [mensagem ou](../resources/message.md) um [evento.](../resources/event.md)

Use essa abordagem para anexar um arquivo se o tamanho do arquivo estiver entre 3 MB e 150 MB. Para anexar um arquivo menor que 3 MB, faça uma operação na propriedade de navegação de anexos do item do Outlook; veja como fazer isso para uma mensagem ou para `POST` [um evento.](event-post-attachments.md)  [](message-post-attachments.md) 

Como parte da resposta, essa ação retorna uma URL de carregamento que você pode usar em consultas `PUT` sequenciais subsequentes. Os headers de solicitação `PUT` para cada operação permitem que você especifique o intervalo exato de bytes a serem carregados. Isso permite que a transferência seja retomada, caso a conexão de rede seja retirada durante o upload. 

Veja a seguir as etapas para anexar um arquivo a um item do Outlook usando uma sessão de upload:

1. Crie uma sessão de upload.
2. Dentro dessa sessão de carregamento, carregue iterativamente intervalos de bytes (até 4 MB a cada vez) até que todos os bytes do arquivo tenham sido carregados e o arquivo seja anexado ao item especificado.
3. Salve a ID do anexo para acesso futuro.
4. Opcional: excluir a sessão de carregamento.

Veja [anexar arquivos grandes a mensagens ou eventos do Outlook](/graph/outlook-large-attachments) para ver um exemplo.

> [!TIP]
> O Exchange Online permite que os administradores personalizem o limite de tamanho de mensagens para caixas de correio do Microsoft 365, incluindo anexos de mensagens. Por padrão, esse limite de tamanho de mensagem é de 35 MB. Descubra como personalizar o [tamanho máximo da mensagem para](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) suportar anexos maiores do que o limite padrão para seu locatário. 

> [!IMPORTANT] 
> Esteja ciente de um [problema](/graph/known-issues#attaching-large-files-to-messages) conhecido se estiver anexando um arquivo grande a uma mensagem ou evento em uma caixa de correio compartilhada ou delegada.


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Mail.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Mail.ReadWrite |
| Aplicativo                            | Mail.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP

Para criar uma sessão de upload para anexar um arquivo a um **evento:** 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

Para criar uma sessão de upload para anexar um arquivo a uma **mensagem:** 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | Portador {token} |


## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|AttachmentItem|[attachmentItem](../resources/attachmentitem.md)|Representa atributos do item a ser carregado e anexado. No mínimo, especifique o tipo de anexo ( `file` ), um nome e o tamanho do arquivo.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um novo objeto `201 Created` [uploadSession](../resources/uploadsession.md) no corpo da resposta.

>**Observação**: 
>
>A **propriedade uploadUrl** retornada como parte do objeto de resposta **uploadSession** é uma URL opaca para consultas subsequentes para carregar intervalos de `PUT` byte do arquivo. Ele contém o token de autorização apropriado para consultas `PUT` subsequentes que expiram **por expirationDateTime**. Não personalize essa URL.
>
>A **propriedade nextExpectedRanges** especifica o próximo local de byte do arquivo a ser carregado, por exemplo, `"NextExpectedRanges":["2097152"]` . Você deve carregar os bytes em um arquivo na ordem.

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como criar uma sessão de upload que você pode usar nas operações subsequentes de carregamento de arquivo para a mensagem especificada.

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower", 
    "size": 3483322
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment: createUploadSession",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


