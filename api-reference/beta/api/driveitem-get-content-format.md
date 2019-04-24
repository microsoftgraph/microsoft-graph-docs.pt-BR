---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Converter em outros formatos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c3761525d0acbd5613a71519d9ebd56ab8475f03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454423"
---
# <a name="download-a-file-in-another-format"></a>Baixar um arquivo em outro formato

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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


Os seguintes valores são válidos para o parâmetro **format**:

| Valor | Descrição                        | Extensões de origem com suporte
|:------|:-----------------------------------|---------------------------------
| glb   | Converte o item no formato GLB  | Cool, FBX, obj, estrato, STL, 3mf
| HTML  | Converte o item em formato HTML | EML, MD, msg
| jpg   | Converte o item em formato JPG  | 3G2, 3GP, 3GP2, 3GPP, 3mf, ai, ARW, ASF, AVI, Bas, Bash, bat, BMP, c CBL, cmd, cool, CPP, CR2, CRW, cs, CSS, CSV, CUR, DCM,, DIC, DICM, DICOM, DNG, Doc, docx,, o EPI, o, o EPSF, o, o EPSI, o , HEIC, HEIF, htm, HTML, ICO, Icon, Java, JFIF, JPEG, jpg, js, JSON, Key, log, M2TS, M4A, M4V, reparation, MD, MEF, MOV, o filme, mp3, o MRW, o NEF, o NRW, o (a), o, o, o formato de página, o, o png, o , potm, potx, PPS, ppsx, ppsxm, ppt, pptm, pptx, PS, ps1, PSB, PSD, py, RAW, RB, RTF, RW1, RW2, sh, esboço, SQL, SR2, STL, TIF, TIFF,, txt, webm, XBM,. WMA, XCF,, XPM, YAML, yml
| pdf   | Converte o item em formato PDF  | Doc, docx, ePub, EML, htm, HTML, MD, MSG, odp, ODS, odt, PPS, ppsx, XL, pptx, RTF, TIF, TIFF, xls, xlsm, xlsx

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Name            | Valor   | Descrição                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida. |

## <a name="example"></a>Exemplo

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

Confira [Respostas de erro][error-response] para saber mais sobre como os erros retornam.

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!--
{
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
