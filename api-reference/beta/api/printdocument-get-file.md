---
title: Baixar arquivo binário do documento
description: Baixe o arquivo binário associado ao documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7e7de914d8549472e08c23f65af25ca99542a58
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273652"
---
# <a name="download-printdocument-binary-file"></a>Baixar arquivo binário do documento

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Baixar o arquivo binário associado a um [documento](../resources/printdocument.md). Chamar esse método gera uma resposta de redirecionamento com uma URL previamente autenticada que pode ser usada para baixar a carga.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura universal de impressão ativa e ter uma permissão que conceda obter acesso à [impressora](printer-get.md) .

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                  |
| :------------------------------------- | :----------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | PrintJob. Read, PrintJob. Read. All, PrintJob. ReadWrite, PrintJob. ReadWrite. All |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                               |
| Aplicativo                            | PrintJob. Read. All, PrintJob. ReadWrite. All                    |

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
Se tiver êxito, este método retornará `302 Found` e a URL de download previamente autenticado no cabeçalho de local.

## <a name="examples"></a>Exemplos
O exemplo a seguir mostra como chamar essa API para adquirir uma URL de download previamente autenticado. Para iniciar o download, siga a URL de redirecionamento na resposta.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
