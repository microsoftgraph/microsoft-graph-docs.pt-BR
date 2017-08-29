# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="76e90-101">Baixe o conteúdo de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="76e90-101">Download the contents of a DriveItem</span></span>

<span data-ttu-id="76e90-p101">Baixe o conteúdo para um driveItem. Somente driveItem com a propriedade **file** pode ser baixada.</span><span class="sxs-lookup"><span data-stu-id="76e90-p101">Download the contents for a driveItem. Only driveItem with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="76e90-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="76e90-104">Permissions</span></span>
<span data-ttu-id="76e90-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76e90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76e90-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76e90-107">Permission type</span></span>      | <span data-ttu-id="76e90-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76e90-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76e90-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76e90-109">Delegated (work or school account)</span></span> | <span data-ttu-id="76e90-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e90-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="76e90-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76e90-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76e90-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e90-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="76e90-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76e90-113">Application</span></span> | <span data-ttu-id="76e90-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e90-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76e90-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76e90-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /drives/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
```

## <a name="request-headers"></a><span data-ttu-id="76e90-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76e90-116">Request headers</span></span>

| <span data-ttu-id="76e90-117">Nome</span><span class="sxs-lookup"><span data-stu-id="76e90-117">Name</span></span>          | <span data-ttu-id="76e90-118">Valor</span><span class="sxs-lookup"><span data-stu-id="76e90-118">Value</span></span>  | <span data-ttu-id="76e90-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="76e90-119">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="76e90-120">if-none-match</span><span class="sxs-lookup"><span data-stu-id="76e90-120">if-none-match</span></span> | <span data-ttu-id="76e90-121">String</span><span class="sxs-lookup"><span data-stu-id="76e90-121">String</span></span> | <span data-ttu-id="76e90-122">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="76e90-122">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76e90-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76e90-123">Request body</span></span>
<span data-ttu-id="76e90-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76e90-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="76e90-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76e90-125">Example</span></span>
<span data-ttu-id="76e90-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="76e90-126">Here is an example of how to call this API.</span></span>


<!-- { "blockType": "request", "name": "driveitem-download-contents" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/content
```

##### <a name="response"></a><span data-ttu-id="76e90-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="76e90-127">Response</span></span>
<span data-ttu-id="76e90-p103">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo. Esta é a mesma URL disponível por meio da propriedade `@microsoft.graph.downloadUrl` no DriveItem.</span><span class="sxs-lookup"><span data-stu-id="76e90-p103">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="76e90-p104">Para baixar o conteúdo do arquivo, seu aplicativo precisará seguir o cabeçalho `Location` na resposta. Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.</span><span class="sxs-lookup"><span data-stu-id="76e90-p104">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="76e90-132">URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="76e90-132">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="76e90-133">Downloads de intervalo parcial</span><span class="sxs-lookup"><span data-stu-id="76e90-133">Partial range downloads</span></span>

<span data-ttu-id="76e90-p105">Para baixar um intervalo parcial de bytes do arquivo, o aplicativo pode usar o cabeçalho `Range` conforme especificado em [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Observe que você deve acrescentar o cabeçalho `Range` à URL `@microsoft.graph.downloadUrl` real e não à solicitação para `/content`.</span><span class="sxs-lookup"><span data-stu-id="76e90-p105">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "name": "driveitem-get-partial-content" } -->
```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="76e90-p106">Isso retornará uma resposta `HTTP 206 Partial Content` com o intervalo de solicitação de bytes do arquivo. Se o intervalo não puder ser gerado, o cabeçalho do Intervalo poderá ser ignorado, e uma resposta `HTTP 200` será retornada com todo o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="76e90-p106">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Download item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Download file"
}-->
