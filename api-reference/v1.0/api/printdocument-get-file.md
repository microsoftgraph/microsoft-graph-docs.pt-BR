---
title: Baixar arquivo binário printDocument
description: Baixe o arquivo binário associado ao documento.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7bde42e03af509f101515dc847283fc1e354c478
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517025"
---
# <a name="download-printdocument-binary-file"></a>Baixar arquivo binário printDocument

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Baixe o arquivo binário associado a [um printDocument](../resources/printdocument.md). Chamar esse método gera uma resposta de redirecionamento com uma URL pré-autenticada que pode ser usada para baixar a carga.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda concessões obter acesso [à](printer-get.md) impressora.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                  |
| :------------------------------------- | :----------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                               |
| Aplicativo                            | PrintJob.Read.All, PrintJob.ReadWrite.All                    |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará e a `302 Found` URL de download pré-autenticada no header Location.

## <a name="examples"></a>Exemplos
O exemplo a seguir mostra como chamar essa API para adquirir uma URL de download pré-autenticada. Para iniciar o download, siga a URL de redirecionamento na resposta.

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Found
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
