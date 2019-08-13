---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Baixar um arquivo
localization_priority: Priority
ms.prod: sharepoint
description: Baixar o conteúdo do fluxo principal (arquivo) de um DriveItem. Somente driveItems com a propriedade file podem ser baixados.
doc_type: apiPageType
ms.openlocfilehash: 451a324e930c01d569e8028f61a4b795a5a83a1e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375062"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="a09d1-104">Baixe o conteúdo de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="a09d1-104">Download the contents of a DriveItem</span></span>

<span data-ttu-id="a09d1-105">Baixar o conteúdo do fluxo principal (arquivo) de um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="a09d1-105">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="a09d1-106">Somente driveItems com a propriedade **file** podem ser baixados.</span><span class="sxs-lookup"><span data-stu-id="a09d1-106">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="a09d1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a09d1-107">Permissions</span></span>

<span data-ttu-id="a09d1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a09d1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a09d1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a09d1-110">Permission type</span></span>      | <span data-ttu-id="a09d1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a09d1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a09d1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a09d1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a09d1-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09d1-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a09d1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a09d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a09d1-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09d1-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a09d1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a09d1-116">Application</span></span> | <span data-ttu-id="a09d1-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09d1-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a09d1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a09d1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="a09d1-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a09d1-119">Optional request headers</span></span>

| <span data-ttu-id="a09d1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a09d1-120">Name</span></span>          | <span data-ttu-id="a09d1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a09d1-121">Value</span></span>  | <span data-ttu-id="a09d1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a09d1-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a09d1-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="a09d1-123">if-none-match</span></span> | <span data-ttu-id="a09d1-124">String</span><span class="sxs-lookup"><span data-stu-id="a09d1-124">String</span></span> | <span data-ttu-id="a09d1-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="a09d1-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="a09d1-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a09d1-126">Example</span></span>

<span data-ttu-id="a09d1-127">Aqui está um exemplo para baixar um arquivo completo.</span><span class="sxs-lookup"><span data-stu-id="a09d1-127">Here is an example to download a complete file.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="a09d1-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="a09d1-128">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a09d1-129">C#</span><span class="sxs-lookup"><span data-stu-id="a09d1-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a09d1-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a09d1-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a09d1-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a09d1-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a09d1-132">Java</span><span class="sxs-lookup"><span data-stu-id="a09d1-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/download-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a09d1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a09d1-133">Response</span></span>

<span data-ttu-id="a09d1-p104">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo. Esta é a mesma URL disponível por meio da propriedade `@microsoft.graph.downloadUrl` no DriveItem.</span><span class="sxs-lookup"><span data-stu-id="a09d1-p104">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="a09d1-136">Para baixar o conteúdo do arquivo, seu aplicativo precisa seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a09d1-136">To download the contents of the file your application will need to follow the `Location` header in the response.</span></span>
<span data-ttu-id="a09d1-137">Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.</span><span class="sxs-lookup"><span data-stu-id="a09d1-137">Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immediately.</span></span>

<span data-ttu-id="a09d1-138">URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="a09d1-138">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="a09d1-139">Downloads de intervalo parcial</span><span class="sxs-lookup"><span data-stu-id="a09d1-139">Partial range downloads</span></span>

<span data-ttu-id="a09d1-p106">Para baixar um intervalo parcial de bytes do arquivo, o aplicativo pode usar o cabeçalho `Range` conforme especificado em [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Observe que você deve acrescentar o cabeçalho `Range` à URL `@microsoft.graph.downloadUrl` real e não à solicitação para `/content`.</span><span class="sxs-lookup"><span data-stu-id="a09d1-p106">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="a09d1-p107">Isso retornará uma resposta `HTTP 206 Partial Content` com o intervalo de solicitação de bytes do arquivo. Se o intervalo não puder ser gerado, o cabeçalho do Intervalo poderá ser ignorado, e uma resposta `HTTP 200` será retornada com todo o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="a09d1-p107">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="a09d1-144">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="a09d1-144">Error responses</span></span>

<span data-ttu-id="a09d1-145">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="a09d1-145">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download",
  "suppressions": [
  ]
} -->
