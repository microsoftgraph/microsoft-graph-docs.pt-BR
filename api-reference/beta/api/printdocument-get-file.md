---
title: Baixar o arquivo binário printDocument
description: Baixe o arquivo binário associado ao documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 590b97c01623cba26407ca0a39ad7d0b3b7a1ca3
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034230"
---
# <a name="download-printdocument-binary-file"></a>Baixar o arquivo binário printDocument

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Baixe o arquivo binário associado a [um printDocument](../resources/printdocument.md). Chamar esse método gera uma resposta de redirecionamento com uma URL pré-autenticada que pode ser usada para baixar a carga.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda acesso à [impressora.](printer-get.md)

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                  |
| :------------------------------------- | :----------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                               |
| Aplicativo                            | PrintJob.Read.All, PrintJob.ReadWrite.All                    |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna e a `302 Found` URL de download previamente autenticada no título De localização.

## <a name="examples"></a>Exemplos
O exemplo a seguir mostra como chamar essa API para adquirir uma URL de download pré-autenticada. Para iniciar o download, siga a URL de redirecionamento na resposta.

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-document-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-document-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-document-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-document-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
