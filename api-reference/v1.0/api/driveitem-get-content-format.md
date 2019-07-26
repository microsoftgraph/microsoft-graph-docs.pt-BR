---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Converter em outros formatos
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e66d302c7397690f6975363f9c3785f8b620756d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890965"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="b746d-102">Baixar um arquivo em outro formato</span><span class="sxs-lookup"><span data-stu-id="b746d-102">Download a file in another format</span></span>

<span data-ttu-id="b746d-103">Use esta API para recuperar os conteúdos de um item em um formato específico.</span><span class="sxs-lookup"><span data-stu-id="b746d-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="b746d-104">Nem todos os arquivos podem ser convertidos em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="b746d-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="b746d-105">Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="b746d-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b746d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b746d-106">Prerequisites</span></span>

<span data-ttu-id="b746d-107">Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.</span><span class="sxs-lookup"><span data-stu-id="b746d-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="b746d-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b746d-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="b746d-109">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="b746d-109">Query parameters</span></span>

| <span data-ttu-id="b746d-110">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b746d-110">Parameter</span></span>      | <span data-ttu-id="b746d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b746d-111">Type</span></span>  | <span data-ttu-id="b746d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b746d-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="b746d-113">_format_</span><span class="sxs-lookup"><span data-stu-id="b746d-113">_format_</span></span>  | <span data-ttu-id="b746d-114">string</span><span class="sxs-lookup"><span data-stu-id="b746d-114">string</span></span> | <span data-ttu-id="b746d-115">Especifique o formato em que o conteúdo do item deve ser baixado.</span><span class="sxs-lookup"><span data-stu-id="b746d-115">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="b746d-116">Opções de formato</span><span class="sxs-lookup"><span data-stu-id="b746d-116">Format options</span></span>

<span data-ttu-id="b746d-117">Os seguintes valores são válidos para o parâmetro **format**:</span><span class="sxs-lookup"><span data-stu-id="b746d-117">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="b746d-118">Valor de format</span><span class="sxs-lookup"><span data-stu-id="b746d-118">Format value</span></span> | <span data-ttu-id="b746d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b746d-119">Description</span></span>                        | <span data-ttu-id="b746d-120">Extensões de origem com suporte</span><span class="sxs-lookup"><span data-stu-id="b746d-120">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="b746d-121">pdf</span><span class="sxs-lookup"><span data-stu-id="b746d-121">pdf</span></span>          | <span data-ttu-id="b746d-122">Converte o item em formato PDF.</span><span class="sxs-lookup"><span data-stu-id="b746d-122">Converts the item into PDF format.</span></span> | <span data-ttu-id="b746d-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="b746d-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="b746d-124">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b746d-124">Optional request headers</span></span>

| <span data-ttu-id="b746d-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b746d-125">Name</span></span>            | <span data-ttu-id="b746d-126">Valor</span><span class="sxs-lookup"><span data-stu-id="b746d-126">Value</span></span>   | <span data-ttu-id="b746d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b746d-127">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b746d-128">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="b746d-128">_if-none-match_</span></span> | <span data-ttu-id="b746d-129">String</span><span class="sxs-lookup"><span data-stu-id="b746d-129">String</span></span>  | <span data-ttu-id="b746d-130">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="b746d-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="b746d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b746d-131">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b746d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b746d-132">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b746d-133">C#</span><span class="sxs-lookup"><span data-stu-id="b746d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b746d-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b746d-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b746d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b746d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b746d-136">Java</span><span class="sxs-lookup"><span data-stu-id="b746d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="b746d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b746d-137">Response</span></span>

<span data-ttu-id="b746d-138">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo convertido.</span><span class="sxs-lookup"><span data-stu-id="b746d-138">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="b746d-139">Para baixar o arquivo convertido, seu aplicativo deve seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b746d-139">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="b746d-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="b746d-140">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="b746d-141">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="b746d-141">Error responses</span></span>

<span data-ttu-id="b746d-142">Confira [Respostas de Erros][error-response] para saber mais sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="b746d-142">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
