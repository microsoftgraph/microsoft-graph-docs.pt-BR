---
author: JeremyKelley
description: Use esta API para recuperar os conteúdos de um item em um formato específico.
ms.date: 09/10/2017
title: Converter em outros formatos
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f6343e3b0ce7ba9eb114e6eeadc6040341fb5c47
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786815"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="748f4-103">Baixar um arquivo em outro formato</span><span class="sxs-lookup"><span data-stu-id="748f4-103">Download a file in another format</span></span>

<span data-ttu-id="748f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="748f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="748f4-p101">Use esta API para recuperar os conteúdos de um item em um formato específico. Nem todos os arquivos podem ser convertidos em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="748f4-p101">Use this API to retrieve the contents of an item in a specific format. Not all files can be converted into all formats.</span></span>

<span data-ttu-id="748f4-107">Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="748f4-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="748f4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="748f4-108">Prerequisites</span></span>

<span data-ttu-id="748f4-109">Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.</span><span class="sxs-lookup"><span data-stu-id="748f4-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="748f4-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="748f4-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="748f4-111">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="748f4-111">Query parameters</span></span>

| <span data-ttu-id="748f4-112">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="748f4-112">Parameter</span></span>      | <span data-ttu-id="748f4-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="748f4-113">Type</span></span>  | <span data-ttu-id="748f4-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="748f4-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="748f4-115">_format_</span><span class="sxs-lookup"><span data-stu-id="748f4-115">_format_</span></span>  | <span data-ttu-id="748f4-116">string</span><span class="sxs-lookup"><span data-stu-id="748f4-116">string</span></span> | <span data-ttu-id="748f4-117">Especifique o formato em que o conteúdo do item deve ser baixado.</span><span class="sxs-lookup"><span data-stu-id="748f4-117">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="748f4-118">Os seguintes valores são válidos para o parâmetro **format**:</span><span class="sxs-lookup"><span data-stu-id="748f4-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="748f4-119">Valor</span><span class="sxs-lookup"><span data-stu-id="748f4-119">Value</span></span> | <span data-ttu-id="748f4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="748f4-120">Description</span></span>                        | <span data-ttu-id="748f4-121">Extensões de origem com suporte</span><span class="sxs-lookup"><span data-stu-id="748f4-121">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="748f4-122">glb</span><span class="sxs-lookup"><span data-stu-id="748f4-122">glb</span></span>   | <span data-ttu-id="748f4-123">Converte o item ao formato GLB</span><span class="sxs-lookup"><span data-stu-id="748f4-123">Converts the item into GLB format</span></span>  | <span data-ttu-id="748f4-124">cool, fbx, obj, ply, stl, 3mf</span><span class="sxs-lookup"><span data-stu-id="748f4-124">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="748f4-125">HTML</span><span class="sxs-lookup"><span data-stu-id="748f4-125">html</span></span>  | <span data-ttu-id="748f4-126">Converte o item ao formato HTML</span><span class="sxs-lookup"><span data-stu-id="748f4-126">Converts the item into HTML format</span></span> | <span data-ttu-id="748f4-127">eml, md, msg</span><span class="sxs-lookup"><span data-stu-id="748f4-127">eml, md, msg</span></span>
| <span data-ttu-id="748f4-128">jpg</span><span class="sxs-lookup"><span data-stu-id="748f4-128">jpg</span></span>   | <span data-ttu-id="748f4-129">Converte o item ao formato JPG</span><span class="sxs-lookup"><span data-stu-id="748f4-129">Converts the item into JPG format</span></span>  | <span data-ttu-id="748f4-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span><span class="sxs-lookup"><span data-stu-id="748f4-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="748f4-131">pdf</span><span class="sxs-lookup"><span data-stu-id="748f4-131">pdf</span></span>   | <span data-ttu-id="748f4-132">Converte o item ao formato PDF</span><span class="sxs-lookup"><span data-stu-id="748f4-132">Converts the item into PDF format</span></span>  | <span data-ttu-id="748f4-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span><span class="sxs-lookup"><span data-stu-id="748f4-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="748f4-134">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="748f4-134">Optional request headers</span></span>

| <span data-ttu-id="748f4-135">Nome</span><span class="sxs-lookup"><span data-stu-id="748f4-135">Name</span></span>            | <span data-ttu-id="748f4-136">Valor</span><span class="sxs-lookup"><span data-stu-id="748f4-136">Value</span></span>   | <span data-ttu-id="748f4-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="748f4-137">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="748f4-138">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="748f4-138">_if-none-match_</span></span> | <span data-ttu-id="748f4-139">String</span><span class="sxs-lookup"><span data-stu-id="748f4-139">String</span></span>  | <span data-ttu-id="748f4-140">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="748f4-140">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="748f4-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="748f4-141">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="748f4-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="748f4-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[<span data-ttu-id="748f4-143">C#</span><span class="sxs-lookup"><span data-stu-id="748f4-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="748f4-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="748f4-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="748f4-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="748f4-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="748f4-146">Java</span><span class="sxs-lookup"><span data-stu-id="748f4-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="748f4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="748f4-147">Response</span></span>

<span data-ttu-id="748f4-148">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo convertido.</span><span class="sxs-lookup"><span data-stu-id="748f4-148">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="748f4-149">Para baixar o arquivo convertido, seu aplicativo deve seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="748f4-149">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="748f4-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="748f4-150">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="748f4-151">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="748f4-151">Error responses</span></span>

<span data-ttu-id="748f4-152">Confira [Respostas de Erros][error-response] para saber mais sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="748f4-152">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
  ]
}
-->


