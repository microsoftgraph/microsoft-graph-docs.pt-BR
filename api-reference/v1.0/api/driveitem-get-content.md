---
author: JeremyKelley
ms.date: 09/10/2017
title: Baixar um arquivo
localization_priority: Priority
ms.prod: sharepoint
description: Baixar o conteúdo do fluxo principal (arquivo) de um DriveItem. Somente driveItems com a propriedade file podem ser baixados.
doc_type: apiPageType
ms.openlocfilehash: 212f11a6d76853e3ab3a7f0e23fd4812b260b496
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240308"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="4b9f0-104">Baixe o conteúdo de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="4b9f0-104">Download the contents of a DriveItem</span></span>

<span data-ttu-id="4b9f0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b9f0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4b9f0-106">Baixar o conteúdo do fluxo principal (arquivo) de um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-106">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="4b9f0-107">Somente driveItems com a propriedade **file** podem ser baixados.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-107">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b9f0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b9f0-108">Permissions</span></span>

<span data-ttu-id="4b9f0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b9f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b9f0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b9f0-111">Permission type</span></span>      | <span data-ttu-id="4b9f0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b9f0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b9f0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b9f0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4b9f0-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b9f0-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b9f0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b9f0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b9f0-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b9f0-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b9f0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b9f0-117">Application</span></span> | <span data-ttu-id="4b9f0-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b9f0-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b9f0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b9f0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="4b9f0-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="4b9f0-120">Optional request headers</span></span>

| <span data-ttu-id="4b9f0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4b9f0-121">Name</span></span>          | <span data-ttu-id="4b9f0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b9f0-122">Value</span></span>  | <span data-ttu-id="4b9f0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b9f0-123">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4b9f0-124">if-none-match</span><span class="sxs-lookup"><span data-stu-id="4b9f0-124">if-none-match</span></span> | <span data-ttu-id="4b9f0-125">String</span><span class="sxs-lookup"><span data-stu-id="4b9f0-125">String</span></span> | <span data-ttu-id="4b9f0-126">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-126">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="4b9f0-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b9f0-127">Example</span></span>

<span data-ttu-id="4b9f0-128">Aqui está um exemplo para baixar um arquivo completo.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-128">Here is an example to download a complete file.</span></span>



# <a name="http"></a>[<span data-ttu-id="4b9f0-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b9f0-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content
```
# <a name="c"></a>[<span data-ttu-id="4b9f0-130">C#</span><span class="sxs-lookup"><span data-stu-id="4b9f0-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b9f0-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b9f0-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b9f0-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b9f0-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b9f0-133">Java</span><span class="sxs-lookup"><span data-stu-id="4b9f0-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/download-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b9f0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b9f0-134">Response</span></span>

<span data-ttu-id="4b9f0-p104">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo. Esta é a mesma URL disponível por meio da propriedade `@microsoft.graph.downloadUrl` no DriveItem.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-p104">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="4b9f0-137">Para baixar o conteúdo do arquivo, seu aplicativo precisa seguir o cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-137">To download the contents of the file your application will need to follow the `Location` header in the response.</span></span>
<span data-ttu-id="4b9f0-138">Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-138">Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immediately.</span></span>

<span data-ttu-id="4b9f0-139">URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="4b9f0-140">Downloads de intervalo parcial</span><span class="sxs-lookup"><span data-stu-id="4b9f0-140">Partial range downloads</span></span>

<span data-ttu-id="4b9f0-p106">Para baixar um intervalo parcial de bytes do arquivo, o aplicativo pode usar o cabeçalho `Range` conforme especificado em [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Observe que você deve acrescentar o cabeçalho `Range` à URL `@microsoft.graph.downloadUrl` real e não à solicitação para `/content`.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-p106">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="4b9f0-p107">Isso retornará uma resposta `HTTP 206 Partial Content` com o intervalo de solicitação de bytes do arquivo. Se o intervalo não puder ser gerado, o cabeçalho do Intervalo poderá ser ignorado, e uma resposta `HTTP 200` será retornada com todo o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="4b9f0-p107">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="4b9f0-145">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="4b9f0-145">Error responses</span></span>

<span data-ttu-id="4b9f0-146">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="4b9f0-146">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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

