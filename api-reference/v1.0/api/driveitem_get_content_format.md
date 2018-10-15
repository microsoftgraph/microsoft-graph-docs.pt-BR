---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Converter em outros formatos
ms.openlocfilehash: 7798905363217d366caabbdd9c82559f578c01aa
ms.sourcegitcommit: 809748ea18943f5fd1d99c4c65a9b964f39a5f25
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/08/2018
ms.locfileid: "23893295"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="ecd4c-102">Baixar um arquivo em outro formato</span><span class="sxs-lookup"><span data-stu-id="ecd4c-102">Download a file in another format</span></span>

<span data-ttu-id="ecd4c-103">Use esta API para recuperar os conteúdos de um item em um formato específico.</span><span class="sxs-lookup"><span data-stu-id="ecd4c-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="ecd4c-104">Nem todos os arquivos podem ser convertidos em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="ecd4c-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="ecd4c-105">Para baixar o item no formato original, confira [Baixar o conteúdo de um item](driveitem_get_content.md).</span><span class="sxs-lookup"><span data-stu-id="ecd4c-105">To download the item in it's original format, see [download an item's contents](driveitem_get_content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecd4c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecd4c-106">Prerequisites</span></span>

<span data-ttu-id="ecd4c-107">Para chamar esta API, o usuário deve ter concedido acesso de leitura ao aplicativo para o arquivo que o aplicativo deseja converter.</span><span class="sxs-lookup"><span data-stu-id="ecd4c-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="ecd4c-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecd4c-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="ecd4c-109">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="ecd4c-109">Query parameters</span></span>

| <span data-ttu-id="ecd4c-110">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ecd4c-110">Parameter</span></span>      | <span data-ttu-id="ecd4c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecd4c-111">Type</span></span>  | <span data-ttu-id="ecd4c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecd4c-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="ecd4c-113">_formato_</span><span class="sxs-lookup"><span data-stu-id="ecd4c-113">_format_</span></span>  | <span data-ttu-id="ecd4c-114">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecd4c-114">string</span></span> | <span data-ttu-id="ecd4c-115">Especifique o formato em que o conteúdo do item deve ser baixado.</span><span class="sxs-lookup"><span data-stu-id="ecd4c-115">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="ecd4c-116">Opções de formato</span><span class="sxs-lookup"><span data-stu-id="ecd4c-116">Format options</span></span>

<span data-ttu-id="ecd4c-117">Os seguintes valores são válidos para o parâmetro de **formato**:</span><span class="sxs-lookup"><span data-stu-id="ecd4c-117">The following values are valid for the **convert** parameter:</span></span>

| <span data-ttu-id="ecd4c-118">Valor de formato</span><span class="sxs-lookup"><span data-stu-id="ecd4c-118">Format value</span></span> | <span data-ttu-id="ecd4c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecd4c-119">Description</span></span>                        | <span data-ttu-id="ecd4c-120">Extensões de origem com suporte</span><span class="sxs-lookup"><span data-stu-id="ecd4c-120">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="ecd4c-121">pdf</span><span class="sxs-lookup"><span data-stu-id="ecd4c-121">pdf</span></span>          | <span data-ttu-id="ecd4c-122">Converte o item em formato PDF.</span><span class="sxs-lookup"><span data-stu-id="ecd4c-122">Converts the item into PDF format.</span></span> | <span data-ttu-id="ecd4c-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="ecd4c-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="ecd4c-124">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ecd4c-124">Optional request headers</span></span>

| <span data-ttu-id="ecd4c-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ecd4c-125">Name</span></span>            | <span data-ttu-id="ecd4c-126">Valor</span><span class="sxs-lookup"><span data-stu-id="ecd4c-126">Value</span></span>   | <span data-ttu-id="ecd4c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecd4c-127">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ecd4c-128">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="ecd4c-128">_if-none-match_</span></span> | <span data-ttu-id="ecd4c-129">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecd4c-129">String</span></span>  | <span data-ttu-id="ecd4c-130">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="ecd4c-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="ecd4c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecd4c-131">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="ecd4c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecd4c-132">Response</span></span>

<span data-ttu-id="ecd4c-133">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo convertido.</span><span class="sxs-lookup"><span data-stu-id="ecd4c-133">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="ecd4c-134">Para baixar o arquivo convertido, seu aplicativo deve seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ecd4c-134">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="ecd4c-135">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="ecd4c-135">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="ecd4c-136">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="ecd4c-136">Error responses</span></span>

<span data-ttu-id="ecd4c-137">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="ecd4c-137">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
