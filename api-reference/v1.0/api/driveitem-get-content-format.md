---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Converter em outros formatos
localization_priority: Priority
ms.prod: sharepoint
description: Use esta API para recuperar os conteúdos de um item em um formato específico.
doc_type: apiPageType
ms.openlocfilehash: 811c0ae25666d23fd597b5d584e5b00e50a00e93
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726330"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="70a7d-103">Baixar um arquivo em outro formato</span><span class="sxs-lookup"><span data-stu-id="70a7d-103">Download a file in another format</span></span>

<span data-ttu-id="70a7d-104">Use esta API para recuperar os conteúdos de um item em um formato específico.</span><span class="sxs-lookup"><span data-stu-id="70a7d-104">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="70a7d-105">Nem todos os arquivos podem ser convertidos em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="70a7d-105">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="70a7d-106">Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="70a7d-106">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70a7d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70a7d-107">Prerequisites</span></span>

<span data-ttu-id="70a7d-108">Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.</span><span class="sxs-lookup"><span data-stu-id="70a7d-108">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="70a7d-109">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70a7d-109">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="70a7d-110">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="70a7d-110">Query parameters</span></span>

| <span data-ttu-id="70a7d-111">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="70a7d-111">Parameter</span></span>      | <span data-ttu-id="70a7d-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="70a7d-112">Type</span></span>  | <span data-ttu-id="70a7d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a7d-113">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="70a7d-114">_format_</span><span class="sxs-lookup"><span data-stu-id="70a7d-114">_format_</span></span>  | <span data-ttu-id="70a7d-115">string</span><span class="sxs-lookup"><span data-stu-id="70a7d-115">string</span></span> | <span data-ttu-id="70a7d-116">Especifique o formato em que o conteúdo do item deve ser baixado.</span><span class="sxs-lookup"><span data-stu-id="70a7d-116">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="70a7d-117">Opções de formato</span><span class="sxs-lookup"><span data-stu-id="70a7d-117">Format options</span></span>

<span data-ttu-id="70a7d-118">Os seguintes valores são válidos para o parâmetro **format**:</span><span class="sxs-lookup"><span data-stu-id="70a7d-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="70a7d-119">Valor de format</span><span class="sxs-lookup"><span data-stu-id="70a7d-119">Format value</span></span> | <span data-ttu-id="70a7d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a7d-120">Description</span></span>                        | <span data-ttu-id="70a7d-121">Extensões de origem com suporte</span><span class="sxs-lookup"><span data-stu-id="70a7d-121">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="70a7d-122">pdf</span><span class="sxs-lookup"><span data-stu-id="70a7d-122">pdf</span></span>          | <span data-ttu-id="70a7d-123">Converte o item em formato PDF.</span><span class="sxs-lookup"><span data-stu-id="70a7d-123">Converts the item into PDF format.</span></span> | <span data-ttu-id="70a7d-124">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="70a7d-124">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="70a7d-125">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="70a7d-125">Optional request headers</span></span>

| <span data-ttu-id="70a7d-126">Nome</span><span class="sxs-lookup"><span data-stu-id="70a7d-126">Name</span></span>            | <span data-ttu-id="70a7d-127">Valor</span><span class="sxs-lookup"><span data-stu-id="70a7d-127">Value</span></span>   | <span data-ttu-id="70a7d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a7d-128">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="70a7d-129">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="70a7d-129">_if-none-match_</span></span> | <span data-ttu-id="70a7d-130">String</span><span class="sxs-lookup"><span data-stu-id="70a7d-130">String</span></span>  | <span data-ttu-id="70a7d-131">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="70a7d-131">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="70a7d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70a7d-132">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70a7d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="70a7d-133">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70a7d-134">C#</span><span class="sxs-lookup"><span data-stu-id="70a7d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70a7d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70a7d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70a7d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70a7d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="70a7d-137">Java</span><span class="sxs-lookup"><span data-stu-id="70a7d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="70a7d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="70a7d-138">Response</span></span>

<span data-ttu-id="70a7d-139">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo convertido.</span><span class="sxs-lookup"><span data-stu-id="70a7d-139">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="70a7d-140">Para baixar o arquivo convertido, seu aplicativo deve seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="70a7d-140">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="70a7d-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="70a7d-141">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="70a7d-142">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="70a7d-142">Error responses</span></span>

<span data-ttu-id="70a7d-143">Confira [Respostas de Erros][error-response] para saber mais sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="70a7d-143">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
  ]
} -->
