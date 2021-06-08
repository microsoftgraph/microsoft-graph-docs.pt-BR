---
author: JeremyKelley
ms.date: 09/10/2017
title: Converter em outros formatos
localization_priority: Priority
ms.prod: sharepoint
description: Use esta API para recuperar os conteúdos de um item em um formato específico.
doc_type: apiPageType
ms.openlocfilehash: 38b87b43f137fe291be31d98d97ea9a9448e6c9a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787804"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="1127a-103">Baixar um arquivo em outro formato</span><span class="sxs-lookup"><span data-stu-id="1127a-103">Download a file in another format</span></span>

<span data-ttu-id="1127a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1127a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1127a-p101">Use esta API para recuperar os conteúdos de um item em um formato específico. Nem todos os arquivos podem ser convertidos em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="1127a-p101">Use this API to retrieve the contents of an item in a specific format. Not all files can be converted into all formats.</span></span>

<span data-ttu-id="1127a-107">Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="1127a-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1127a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1127a-108">Prerequisites</span></span>

<span data-ttu-id="1127a-109">Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.</span><span class="sxs-lookup"><span data-stu-id="1127a-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="1127a-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1127a-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="1127a-111">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="1127a-111">Query parameters</span></span>

| <span data-ttu-id="1127a-112">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1127a-112">Parameter</span></span>      | <span data-ttu-id="1127a-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="1127a-113">Type</span></span>  | <span data-ttu-id="1127a-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="1127a-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="1127a-115">_format_</span><span class="sxs-lookup"><span data-stu-id="1127a-115">_format_</span></span>  | <span data-ttu-id="1127a-116">string</span><span class="sxs-lookup"><span data-stu-id="1127a-116">string</span></span> | <span data-ttu-id="1127a-117">Especifique o formato em que o conteúdo do item deve ser baixado.</span><span class="sxs-lookup"><span data-stu-id="1127a-117">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="1127a-118">Opções de formato</span><span class="sxs-lookup"><span data-stu-id="1127a-118">Format options</span></span>

<span data-ttu-id="1127a-119">Os seguintes valores são válidos para o parâmetro **format**:</span><span class="sxs-lookup"><span data-stu-id="1127a-119">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="1127a-120">Valor de format</span><span class="sxs-lookup"><span data-stu-id="1127a-120">Format value</span></span> | <span data-ttu-id="1127a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1127a-121">Description</span></span>                        | <span data-ttu-id="1127a-122">Extensões de origem com suporte</span><span class="sxs-lookup"><span data-stu-id="1127a-122">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="1127a-123">pdf</span><span class="sxs-lookup"><span data-stu-id="1127a-123">pdf</span></span>          | <span data-ttu-id="1127a-124">Converte o item em formato PDF.</span><span class="sxs-lookup"><span data-stu-id="1127a-124">Converts the item into PDF format.</span></span> | <span data-ttu-id="1127a-125">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="1127a-125">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="1127a-126">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="1127a-126">Optional request headers</span></span>

| <span data-ttu-id="1127a-127">Nome</span><span class="sxs-lookup"><span data-stu-id="1127a-127">Name</span></span>            | <span data-ttu-id="1127a-128">Valor</span><span class="sxs-lookup"><span data-stu-id="1127a-128">Value</span></span>   | <span data-ttu-id="1127a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="1127a-129">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1127a-130">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="1127a-130">_if-none-match_</span></span> | <span data-ttu-id="1127a-131">String</span><span class="sxs-lookup"><span data-stu-id="1127a-131">String</span></span>  | <span data-ttu-id="1127a-132">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="1127a-132">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="1127a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1127a-133">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="1127a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1127a-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[<span data-ttu-id="1127a-135">C#</span><span class="sxs-lookup"><span data-stu-id="1127a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1127a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1127a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1127a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1127a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1127a-138">Java</span><span class="sxs-lookup"><span data-stu-id="1127a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="1127a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1127a-139">Response</span></span>

<span data-ttu-id="1127a-140">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo convertido.</span><span class="sxs-lookup"><span data-stu-id="1127a-140">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="1127a-141">Para baixar o arquivo convertido, seu aplicativo deve seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1127a-141">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="1127a-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="1127a-142">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="1127a-143">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="1127a-143">Error responses</span></span>

<span data-ttu-id="1127a-144">Confira [Respostas de Erros][error-response] para saber mais sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="1127a-144">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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

