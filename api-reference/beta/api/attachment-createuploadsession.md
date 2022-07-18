---
title: 'attachment: createUploadSession'
description: Crie uma sessão de carregamento para carregar iterativamente intervalos de um arquivo para anexar o arquivo à mensagem especificada.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3a36f5e3e41caebdde8f1c8f80356980d1a470e5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340369"
---
# <a name="attachment-createuploadsession"></a>attachment: createUploadSession

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma sessão de carregamento que permita que um aplicativo carregue de forma iterativa intervalos de um arquivo, de modo a anexar o arquivo a um Outlook item. O item pode ser uma [mensagem](../resources/message.md) ou [evento](../resources/event.md).

Use essa abordagem para anexar um arquivo se o tamanho do arquivo estiver entre 3 MB e 150 MB. Para anexar um arquivo menor que 3 MB, `POST` faça uma operação na propriedade de navegação **anexos** do item Outlook; consulte como fazer isso para uma mensagem ou para um [evento](event-post-attachments.md).[](message-post-attachments.md) 

Como parte da resposta, essa ação retorna uma URL de carregamento que você pode usar em consultas sequenciais subsequentes `PUT` . Os headers de solicitação para cada `PUT` operação permitem especificar o intervalo exato de bytes a serem carregados. Isso permite que a transferência seja retomada, caso a conexão de rede seja largada durante o carregamento. 

Veja a seguir as etapas para anexar um arquivo a um item Outlook usando uma sessão de carregamento:

1. Criar uma sessão de carregamento.
2. Dentro dessa sessão de carregamento, carrega iterativamente intervalos de bytes (até 4 MB cada vez) até que todos os bytes do arquivo tenham sido carregados e o arquivo seja anexado ao item especificado.
3. Salve a ID do anexo para acesso futuro.
4. Opcional: exclua a sessão de carregamento.

Consulte [anexar arquivos grandes Outlook mensagens ou eventos](/graph/outlook-large-attachments) para um exemplo.

> [!TIP]
> Exchange Online permite que os administradores personalizem o limite de tamanho da mensagem para Microsoft 365 caixas de correio, incluindo quaisquer anexos de mensagem. Por padrão, esse limite de tamanho de mensagem é de 35 MB. Saiba como personalizar [o tamanho máximo da](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) mensagem para dar suporte a anexos maiores do que o limite padrão para seu locatário. 

> [!IMPORTANT] 
> Esteja ciente de um [problema](/graph/known-issues#attaching-large-files-to-messages) conhecido se você estiver anexando um arquivo grande a uma mensagem ou evento em uma caixa de correio compartilhada ou delegada.


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Mail.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Mail.ReadWrite |
| Aplicativo                            | Mail.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP

Para criar uma sessão de carregamento para anexar um arquivo a um **evento**: 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

Para criar uma sessão de carregamento para anexar um arquivo a uma **mensagem**: 

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
|AttachmentItem|[attachmentItem](../resources/attachmentitem.md)|Representa atributos do item a ser carregado e anexado. No mínimo, especifique o tipo de anexo (`file`), um nome e o tamanho do arquivo.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo [objeto uploadSession](../resources/uploadsession.md) no corpo da resposta.

>**Observação**: 
>
>A **propriedade uploadUrl** retornada como parte do **objeto de resposta uploadSession** é uma URL `PUT` opaca para consultas subsequentes para carregar intervalos de byte do arquivo. Ele contém o token de auth apropriado para consultas `PUT` subsequentes que expiram por **expirationDateTime**. Não personalize essa URL.
>
>A **propriedade nextExpectedRanges** especifica o próximo local de byte de arquivo a ser carregado, por exemplo, `"NextExpectedRanges":["2097152"]`. Você deve carregar os bytes em um arquivo na ordem.

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a>Exemplos

### <a name="example-1-create-an-upload-session-to-add-a-large-attachment-to-a-draft-message"></a>Exemplo 1: Criar uma sessão de carregamento para adicionar um anexo grande a uma mensagem de rascunho
O exemplo a seguir mostra como criar uma sessão de carregamento que você pode usar nas operações subsequentes de carregamento de arquivo para a mensagem especificada.

#### <a name="request"></a>Solicitação

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/attachment-createuploadsession-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/attachment-createuploadsession-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

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

### <a name="example-2-create-an-upload-session-to-add-a-large-in-line-attachment-to-a-draft-message"></a>Exemplo 2: Criar uma sessão de carregamento para adicionar um anexo em linha grande a uma mensagem de rascunho

O exemplo a seguir mostra como criar uma sessão de carregamento que pode ser usada para adicionar um anexo em linha grande a uma mensagem de rascunho.

Para um anexo em linha, de set _isInline_ property to `true` and use the _contentId_ property to specify a CID for the attachment as shown below. No corpo da mensagem de rascunho, use o mesmo valor CID para indicar a posição onde você deseja incluir o anexo usando uma marca de referência HTML CID, por exemplo `<img src="cid:my_inline_picture">`. Ao carregar o arquivo com êxito, a mensagem renderizada incluirá o anexo como parte do corpo da mensagem no local especificado.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession_inline",
  "sampleKeys": ["AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA="]
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "scenary", 
    "size": 7208534,
    "isInline": true,
    "contentId": "my_inline_picture"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-inline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-inline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-inline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-inline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/attachment-createuploadsession-inline-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/attachment-createuploadsession-inline-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession_inline",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/gv1.0/users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/messages('AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA=')/AttachmentSessions('AAMkAGUwNjQ4ZjIxLTAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IjFTeXQ1bXdXYVh5UFJ",
    "expirationDateTime": "2021-12-27T14:20:12.9708933Z",
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


