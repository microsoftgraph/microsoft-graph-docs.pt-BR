---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Converter em outros formatos
localization_priority: Priority
ms.prod: sharepoint
description: Use esta API para recuperar os conteúdos de um item em um formato específico.
doc_type: apiPageType
ms.openlocfilehash: 3b9e07ed5e1bbe44c89cb307e73c6741f23fe8e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517752"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="c02c8-103">Baixar um arquivo em outro formato</span><span class="sxs-lookup"><span data-stu-id="c02c8-103">Download a file in another format</span></span>

<span data-ttu-id="c02c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c02c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c02c8-105">Use esta API para recuperar os conteúdos de um item em um formato específico.</span><span class="sxs-lookup"><span data-stu-id="c02c8-105">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="c02c8-106">Nem todos os arquivos podem ser convertidos em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="c02c8-106">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="c02c8-107">Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="c02c8-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c02c8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c02c8-108">Prerequisites</span></span>

<span data-ttu-id="c02c8-109">Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.</span><span class="sxs-lookup"><span data-stu-id="c02c8-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="c02c8-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c02c8-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="c02c8-111">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="c02c8-111">Query parameters</span></span>

| <span data-ttu-id="c02c8-112">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c02c8-112">Parameter</span></span>      | <span data-ttu-id="c02c8-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="c02c8-113">Type</span></span>  | <span data-ttu-id="c02c8-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="c02c8-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="c02c8-115">_format_</span><span class="sxs-lookup"><span data-stu-id="c02c8-115">_format_</span></span>  | <span data-ttu-id="c02c8-116">string</span><span class="sxs-lookup"><span data-stu-id="c02c8-116">string</span></span> | <span data-ttu-id="c02c8-117">Especifique o formato em que o conteúdo do item deve ser baixado.</span><span class="sxs-lookup"><span data-stu-id="c02c8-117">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="c02c8-118">Opções de formato</span><span class="sxs-lookup"><span data-stu-id="c02c8-118">Format options</span></span>

<span data-ttu-id="c02c8-119">Os seguintes valores são válidos para o parâmetro **format**:</span><span class="sxs-lookup"><span data-stu-id="c02c8-119">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="c02c8-120">Valor de format</span><span class="sxs-lookup"><span data-stu-id="c02c8-120">Format value</span></span> | <span data-ttu-id="c02c8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c02c8-121">Description</span></span>                        | <span data-ttu-id="c02c8-122">Extensões de origem com suporte</span><span class="sxs-lookup"><span data-stu-id="c02c8-122">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="c02c8-123">pdf</span><span class="sxs-lookup"><span data-stu-id="c02c8-123">pdf</span></span>          | <span data-ttu-id="c02c8-124">Converte o item em formato PDF.</span><span class="sxs-lookup"><span data-stu-id="c02c8-124">Converts the item into PDF format.</span></span> | <span data-ttu-id="c02c8-125">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="c02c8-125">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="c02c8-126">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c02c8-126">Optional request headers</span></span>

| <span data-ttu-id="c02c8-127">Nome</span><span class="sxs-lookup"><span data-stu-id="c02c8-127">Name</span></span>            | <span data-ttu-id="c02c8-128">Valor</span><span class="sxs-lookup"><span data-stu-id="c02c8-128">Value</span></span>   | <span data-ttu-id="c02c8-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c02c8-129">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c02c8-130">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="c02c8-130">_if-none-match_</span></span> | <span data-ttu-id="c02c8-131">String</span><span class="sxs-lookup"><span data-stu-id="c02c8-131">String</span></span>  | <span data-ttu-id="c02c8-132">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="c02c8-132">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="c02c8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c02c8-133">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="c02c8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c02c8-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[<span data-ttu-id="c02c8-135">C#</span><span class="sxs-lookup"><span data-stu-id="c02c8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c02c8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c02c8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c02c8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c02c8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c02c8-138">Java</span><span class="sxs-lookup"><span data-stu-id="c02c8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="c02c8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c02c8-139">Response</span></span>

<span data-ttu-id="c02c8-140">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo convertido.</span><span class="sxs-lookup"><span data-stu-id="c02c8-140">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="c02c8-141">Para baixar o arquivo convertido, seu aplicativo deve seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c02c8-141">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="c02c8-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="c02c8-142">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="c02c8-143">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="c02c8-143">Error responses</span></span>

<span data-ttu-id="c02c8-144">Confira [Respostas de Erros][error-response] para saber mais sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="c02c8-144">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
