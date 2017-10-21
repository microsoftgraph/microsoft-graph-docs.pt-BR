---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Converter em outros formatos
ms.openlocfilehash: 3031500beaec2d765075abfd925a6333f50368f9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="download-a-file-in-another-format"></a>Baixar um arquivo em outro formato

Use esta API para recuperar os conteúdos de um item em um formato específico.
Nem todos os arquivos podem ser convertidos em todos os formatos.

Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem_get_content.md).

## <a name="prerequisites"></a>Pré-requisitos

Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

### <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome            | Valor   | Descrição                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida. |


### <a name="query-string-parameters"></a>Parâmetros de cadeia de caracteres de consulta

| Name      | Valor  | Descrição                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| _format_  | string | Especifique o formato em que o conteúdo do item deve ser baixado. |


Os seguintes valores são válidos para o parâmetro **convert**:

| Valor   | Descrição                        | Extensões de origem com suporte |
|:--------|:-----------------------------------|-----------------------------|
| **pdf** | Converte o item em formato PDF. | csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx | 

### <a name="example"></a>Exemplo

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
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

### <a name="error-responses"></a>Respostas de erro

Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
