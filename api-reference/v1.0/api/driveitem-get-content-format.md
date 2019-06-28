---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Converter em outros formatos
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e0486012bbc9b4ba3fe019f69872dbdf8ab9724b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279076"
---
# <a name="download-a-file-in-another-format"></a>Baixar um arquivo em outro formato

Use esta API para recuperar os conteúdos de um item em um formato específico.
Nem todos os arquivos podem ser convertidos em todos os formatos.

Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem-get-content.md).

## <a name="prerequisites"></a>Pré-requisitos

Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a>Parâmetros de consulta

| Parâmetro      | Tipo  | Descrição                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| _format_  | string | Especifique o formato em que o conteúdo do item deve ser baixado. |


### <a name="format-options"></a>Opções de formato

Os seguintes valores são válidos para o parâmetro **format**:

| Valor de format | Descrição                        | Extensões de origem com suporte
|:-------------|:-----------------------------------|----------------------------
| pdf          | Converte o item em formato PDF. | csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome            | Valor   | Descrição                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida. |

## <a name="example"></a>Exemplo

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```

## <a name="response"></a>Resposta

Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo convertido.

Para baixar o arquivo convertido, seu aplicativo deve seguir o cabeçalho `Location` na resposta.

As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/convert-item-content-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/convert-item-content-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/convert-item-content-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-responses"></a>Respostas de erros

Confira [Respostas de Erros][error-response] para saber mais sobre como os erros retornam.

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
