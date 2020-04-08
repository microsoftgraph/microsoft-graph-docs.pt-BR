---
title: 'Documento de documentos: uploadData'
description: Carregar um único segmento binário do documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 10bf87d66126d85bdc52c69659647c7728084ac5
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948085"
---
# <a name="printdocument-uploaddata"></a>Documento de documentos: uploadData

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Carregar um único segmento binário do **documento**.

É possível carregar o arquivo inteiro ou dividir o arquivo em vários intervalos de bytes, desde que nenhuma solicitação seja maior do que 1 MB.

Os segmentos do arquivo podem ser carregados em qualquer ordem e podem ser carregados em paralelo, com até quatro solicitações simultâneas. Quando todos os segmentos binários do documento são carregados, o arquivo binário é vinculado ao **printJob**.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Users. Read. All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Intervalo | bytes = {startByteIndex}-{endByteIndex}  |
| Content-Length | ContentLength  |
| Content-type  | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
O corpo da solicitação é um blob binário contendo os bytes do documento que são especificados como um intervalo de bytes inclusivo `Range` no cabeçalho. 

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará uma das seguintes respostas. Não retorna nada no corpo da resposta.

| Condição     | Código da resposta |
|:--------------|:--------------|
| Um ou mais segmentos binários ainda precisam ser carregados | `202 Accepted` |
| Todos os segmentos binários foram carregados com êxito | `201 Created` |

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API para carregar os primeiros 72797 bytes de um documento.
##### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta

Um ou mais segmentos ausentes:
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

Todos os segmentos recebidos:
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```
