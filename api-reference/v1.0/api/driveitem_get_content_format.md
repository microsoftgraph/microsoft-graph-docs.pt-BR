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
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="375ca-102">Baixar um arquivo em outro formato</span><span class="sxs-lookup"><span data-stu-id="375ca-102">Download a file in another format</span></span>

<span data-ttu-id="375ca-103">Use esta API para recuperar os conteúdos de um item em um formato específico.</span><span class="sxs-lookup"><span data-stu-id="375ca-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="375ca-104">Nem todos os arquivos podem ser convertidos em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="375ca-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="375ca-105">Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem_get_content.md).</span><span class="sxs-lookup"><span data-stu-id="375ca-105">To download the item in it's original format, see [download an item's contents](driveitem_get_content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="375ca-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="375ca-106">Prerequisites</span></span>

<span data-ttu-id="375ca-107">Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.</span><span class="sxs-lookup"><span data-stu-id="375ca-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="375ca-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="375ca-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

### <a name="optional-request-headers"></a><span data-ttu-id="375ca-109">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="375ca-109">Optional request headers</span></span>

| <span data-ttu-id="375ca-110">Nome</span><span class="sxs-lookup"><span data-stu-id="375ca-110">Name</span></span>            | <span data-ttu-id="375ca-111">Valor</span><span class="sxs-lookup"><span data-stu-id="375ca-111">Value</span></span>   | <span data-ttu-id="375ca-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="375ca-112">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="375ca-113">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="375ca-113">_if-none-match_</span></span> | <span data-ttu-id="375ca-114">String</span><span class="sxs-lookup"><span data-stu-id="375ca-114">String</span></span>  | <span data-ttu-id="375ca-115">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="375ca-115">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


### <a name="query-string-parameters"></a><span data-ttu-id="375ca-116">Parâmetros de cadeia de caracteres de consulta</span><span class="sxs-lookup"><span data-stu-id="375ca-116">Query string parameters</span></span>

| <span data-ttu-id="375ca-117">Name</span><span class="sxs-lookup"><span data-stu-id="375ca-117">Name</span></span>      | <span data-ttu-id="375ca-118">Valor</span><span class="sxs-lookup"><span data-stu-id="375ca-118">Value</span></span>  | <span data-ttu-id="375ca-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="375ca-119">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="375ca-120">_format_</span><span class="sxs-lookup"><span data-stu-id="375ca-120">_format_</span></span>  | <span data-ttu-id="375ca-121">string</span><span class="sxs-lookup"><span data-stu-id="375ca-121">string</span></span> | <span data-ttu-id="375ca-122">Especifique o formato em que o conteúdo do item deve ser baixado.</span><span class="sxs-lookup"><span data-stu-id="375ca-122">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="375ca-123">Os seguintes valores são válidos para o parâmetro **convert**:</span><span class="sxs-lookup"><span data-stu-id="375ca-123">The following values are valid for the **convert** parameter:</span></span>

| <span data-ttu-id="375ca-124">Valor</span><span class="sxs-lookup"><span data-stu-id="375ca-124">Value</span></span>   | <span data-ttu-id="375ca-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="375ca-125">Description</span></span>                        | <span data-ttu-id="375ca-126">Extensões de origem com suporte</span><span class="sxs-lookup"><span data-stu-id="375ca-126">Supported source extensions</span></span> |
|:--------|:-----------------------------------|-----------------------------|
| <span data-ttu-id="375ca-127">**pdf**</span><span class="sxs-lookup"><span data-stu-id="375ca-127">**pdf**</span></span> | <span data-ttu-id="375ca-128">Converte o item em formato PDF.</span><span class="sxs-lookup"><span data-stu-id="375ca-128">Converts the item into PDF format.</span></span> | <span data-ttu-id="375ca-129">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="375ca-129">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span> | 

### <a name="example"></a><span data-ttu-id="375ca-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="375ca-130">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="375ca-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="375ca-131">Response</span></span>

<span data-ttu-id="375ca-132">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo convertido.</span><span class="sxs-lookup"><span data-stu-id="375ca-132">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="375ca-133">Para baixar o arquivo convertido, seu aplicativo deve seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="375ca-133">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="375ca-134">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="375ca-134">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="375ca-135">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="375ca-135">Error responses</span></span>

<span data-ttu-id="375ca-136">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="375ca-136">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
