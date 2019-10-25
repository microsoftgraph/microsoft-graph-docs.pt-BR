---
title: 'Anexo: createUploadSession'
description: Crie uma sessão de upload para carregar de forma iterativa os intervalos de um arquivo para anexar o arquivo à mensagem especificada.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 541173547ba8222ca5b64cb3396e972be5b017fc
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "37719450"
---
# <a name="attachment-createuploadsession"></a>Anexo: createUploadSession

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de um arquivo de forma iterativa, para anexar o arquivo à [mensagem](../resources/message.md)especificada.

Use essa abordagem para anexar arquivos de tamanhos entre 3 MB e 150 MB a uma **mensagem**. Para anexar arquivos de tamanhos abaixo de 4 MB, basta [postar na propriedade de navegação Attachments](message-post-attachments.md). 

Como parte da resposta, esta ação retorna uma URL de upload que você pode usar em consultas sequenciais `PUT` subsequentes. Os cabeçalhos de solicitação `PUT` para cada operação permitem que você especifique o intervalo exato de bytes a serem carregados. Isso permite que a transferência seja retomada, caso a conexão de rede seja interrompida durante o carregamento. 

A seguir estão as etapas para anexar um arquivo usando uma sessão de carregamento:

1. Criar uma sessão de upload
2. Dentro dessa sessão de upload, carregue de forma iterativa os intervalos de bytes (até 4 MB cada vez) até que todos os bytes do arquivo tenham sido carregados e o arquivo seja anexado à mensagem especificada
3. Salvar a ID do anexo para acesso futuro
4. Opcional: excluir a sessão de upload 

Consulte [anexar arquivos grandes às mensagens do Outlook](/graph/outlook-large-attachments) para obter um exemplo.

> [!TIP]
> O Exchange Online permite que os administradores personalizem o limite de tamanho de mensagens de caixas de correio do Office 365, incluindo qualquer anexo de mensagem. Por padrão, esse limite de tamanho de mensagem é de 35 MB. Descubra como [Personalizar o tamanho máximo da mensagem](https://www.microsoft.com/en-us/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) para dar suporte a anexos maiores que o limite padrão para o seu locatário. 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Mail.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Mail.ReadWrite |
| Aplicativo                            | Mail.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP

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
|AttachmentItem|[attachmentItem](../resources/attachmentitem.md)|Representa os atributos do item a ser carregado e anexado. Especifique, no mínimo, o tipo de`file`anexo (), um nome e o tamanho do arquivo.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [uploadSession](../resources/uploadsession.md) no corpo da resposta.

>**Observação**: 
>
>A propriedade **uploadUrl** retornada como parte do objeto de resposta **UPLOADSESSION** é uma URL opaca para consultas `PUT` subsequentes para carregar intervalos de bytes do arquivo. Ele contém o token de autenticação apropriado para `PUT` consultas subsequentes que expiram pelo **expirationDateTime**. Não Personalize esta URL.
>
>A propriedade **nextExpectedRanges** especifica o próximo local de byte de arquivo para carregar, por exemplo `"NextExpectedRanges":["2097152"]`,. Você deve carregar bytes em um arquivo na ordem.

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a>Exemplos

Veja a seguir um exemplo de como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

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
