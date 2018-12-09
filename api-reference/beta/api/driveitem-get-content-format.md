---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Converter em outros formatos
ms.openlocfilehash: 70558e7c0497c71f620481ff67b7d07cc255cd95
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209716"
---
# <a name="download-a-file-in-another-format"></a>Baixar um arquivo em outro formato

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Use esta API para recuperar os conteúdos de um item em um formato específico.
Nem todos os arquivos podem ser convertidos em todos os formatos.

Para baixar o item no formato original, consulte [fazer o download de conteúdo de um item](driveitem-get-content.md).

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


Os seguintes valores são válidos para o parâmetro **format** :

| Valor | Descrição                        | Extensões de origem com suporte
|:------|:-----------------------------------|---------------------------------
| glb   | Converte o item no formato de GLB  | legal, fbx, objetivo, módulo, stl, 3mf
| HTML  | Converte o item em formato HTML | EML, md, msg
| JPG   | Converte o item em formato JPG  | 3G 2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, legal, cpp, cr2, crw, cs, css, csv, atual, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, FUNERRO, fbx, fppx, gif, glb, h, hcp , heic, heif, htm, html, ico, ícone, java, jfif, jpeg, jpg, js, json, chave, log, m2ts, m4a, m4v, redução, md, mef, mov, filme, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, números, objetivo, odp, odt, ogg, orf, páginas, pano, pdf, pef, php, pict, pl, módulo, png, pot , potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, Aj, bruto, rb, rtf, rw1, rw2, MOS, Esboce, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, fonte xcf, xd, xml, xpm, yaml, yml
| pdf   | Converte o item em formato PDF  | doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome            | Valor   | Descrição                                                                                                                                              |
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

Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
