---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Converter em outros formatos
ms.openlocfilehash: fef327291310b8355c28478185e285217fe99886
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034268"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="883d8-102">Baixar um arquivo em outro formato</span><span class="sxs-lookup"><span data-stu-id="883d8-102">Download a file in another format</span></span>

> <span data-ttu-id="883d8-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="883d8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="883d8-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="883d8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="883d8-105">Use esta API para recuperar os conteúdos de um item em um formato específico.</span><span class="sxs-lookup"><span data-stu-id="883d8-105">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="883d8-106">Nem todos os arquivos podem ser convertidos em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="883d8-106">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="883d8-107">Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="883d8-107">To download the item in it's original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="883d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="883d8-108">Prerequisites</span></span>

<span data-ttu-id="883d8-109">Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.</span><span class="sxs-lookup"><span data-stu-id="883d8-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="883d8-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="883d8-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="883d8-111">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="883d8-111">Query parameters</span></span>

| <span data-ttu-id="883d8-112">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="883d8-112">Parameter</span></span>      | <span data-ttu-id="883d8-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="883d8-113">Type</span></span>  | <span data-ttu-id="883d8-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="883d8-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="883d8-115">_format_</span><span class="sxs-lookup"><span data-stu-id="883d8-115">_format_</span></span>  | <span data-ttu-id="883d8-116">string</span><span class="sxs-lookup"><span data-stu-id="883d8-116">string</span></span> | <span data-ttu-id="883d8-117">Especifique o formato em que o conteúdo do item deve ser baixado.</span><span class="sxs-lookup"><span data-stu-id="883d8-117">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="883d8-118">Os seguintes valores são válidos para o parâmetro **format** :</span><span class="sxs-lookup"><span data-stu-id="883d8-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="883d8-119">Valor</span><span class="sxs-lookup"><span data-stu-id="883d8-119">Value</span></span> | <span data-ttu-id="883d8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="883d8-120">Description</span></span>                        | <span data-ttu-id="883d8-121">Extensões de origem com suporte</span><span class="sxs-lookup"><span data-stu-id="883d8-121">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="883d8-122">glb</span><span class="sxs-lookup"><span data-stu-id="883d8-122">glb</span></span>   | <span data-ttu-id="883d8-123">Converte o item no formato de GLB</span><span class="sxs-lookup"><span data-stu-id="883d8-123">Converts the item into GLB format</span></span>  | <span data-ttu-id="883d8-124">legal, fbx, objetivo, módulo, stl, 3mf</span><span class="sxs-lookup"><span data-stu-id="883d8-124">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="883d8-125">HTML</span><span class="sxs-lookup"><span data-stu-id="883d8-125">html</span></span>  | <span data-ttu-id="883d8-126">Converte o item em formato HTML</span><span class="sxs-lookup"><span data-stu-id="883d8-126">Converts the item into HTML format</span></span> | <span data-ttu-id="883d8-127">EML, md, msg</span><span class="sxs-lookup"><span data-stu-id="883d8-127">eml, md, msg</span></span>
| <span data-ttu-id="883d8-128">JPG</span><span class="sxs-lookup"><span data-stu-id="883d8-128">jpg</span></span>   | <span data-ttu-id="883d8-129">Converte o item em formato JPG</span><span class="sxs-lookup"><span data-stu-id="883d8-129">Converts the item into JPG format</span></span>  | <span data-ttu-id="883d8-130">3G 2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, legal, cpp, cr2, crw, cs, css, csv, atual, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, FUNERRO, fbx, fppx, gif, glb, h, hcp , heic, heif, htm, html, ico, ícone, java, jfif, jpeg, jpg, js, json, chave, log, m2ts, m4a, m4v, redução, md, mef, mov, filme, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, números, objetivo, odp, odt, ogg, orf, páginas, pano, pdf, pef, php, pict, pl, módulo, png, pot , potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, Aj, bruto, rb, rtf, rw1, rw2, MOS, Esboce, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, fonte xcf, xd, xml, xpm, yaml, yml</span><span class="sxs-lookup"><span data-stu-id="883d8-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="883d8-131">pdf</span><span class="sxs-lookup"><span data-stu-id="883d8-131">pdf</span></span>   | <span data-ttu-id="883d8-132">Converte o item em formato PDF</span><span class="sxs-lookup"><span data-stu-id="883d8-132">Converts the item into PDF format</span></span>  | <span data-ttu-id="883d8-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span><span class="sxs-lookup"><span data-stu-id="883d8-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="883d8-134">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="883d8-134">Optional request headers</span></span>

| <span data-ttu-id="883d8-135">Nome</span><span class="sxs-lookup"><span data-stu-id="883d8-135">Name</span></span>            | <span data-ttu-id="883d8-136">Valor</span><span class="sxs-lookup"><span data-stu-id="883d8-136">Value</span></span>   | <span data-ttu-id="883d8-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="883d8-137">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="883d8-138">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="883d8-138">_if-none-match_</span></span> | <span data-ttu-id="883d8-139">String</span><span class="sxs-lookup"><span data-stu-id="883d8-139">String</span></span>  | <span data-ttu-id="883d8-140">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="883d8-140">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="883d8-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="883d8-141">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="883d8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="883d8-142">Response</span></span>

<span data-ttu-id="883d8-143">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo convertido.</span><span class="sxs-lookup"><span data-stu-id="883d8-143">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="883d8-144">Para baixar o arquivo convertido, seu aplicativo deve seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="883d8-144">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="883d8-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="883d8-145">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="883d8-146">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="883d8-146">Error responses</span></span>

<span data-ttu-id="883d8-147">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="883d8-147">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
