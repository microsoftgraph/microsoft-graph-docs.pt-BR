# <a name="create-page"></a><span data-ttu-id="3e8f8-101">Criar página</span><span class="sxs-lookup"><span data-stu-id="3e8f8-101">Create page</span></span>

<span data-ttu-id="3e8f8-102">Crie uma nova [página](../resources/page.md) na seção especificado.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-102">Create a new [page](../resources/page.md) in the specified section.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e8f8-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e8f8-103">Permissions</span></span>
<span data-ttu-id="3e8f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e8f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3e8f8-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e8f8-106">Permission type</span></span>      | <span data-ttu-id="3e8f8-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e8f8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e8f8-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e8f8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3e8f8-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e8f8-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e8f8-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e8f8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e8f8-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e8f8-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3e8f8-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e8f8-112">Application</span></span> | <span data-ttu-id="3e8f8-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e8f8-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e8f8-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e8f8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="3e8f8-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e8f8-115">Request headers</span></span>
| <span data-ttu-id="3e8f8-116">Nome</span><span class="sxs-lookup"><span data-stu-id="3e8f8-116">Name</span></span>       | <span data-ttu-id="3e8f8-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e8f8-117">Type</span></span> | <span data-ttu-id="3e8f8-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e8f8-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3e8f8-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e8f8-119">Authorization</span></span>  | <span data-ttu-id="3e8f8-120">string</span><span class="sxs-lookup"><span data-stu-id="3e8f8-120">string</span></span>  | <span data-ttu-id="3e8f8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e8f8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e8f8-123">Content-Type</span></span> | <span data-ttu-id="3e8f8-124">string</span><span class="sxs-lookup"><span data-stu-id="3e8f8-124">string</span></span> | <span data-ttu-id="3e8f8-p103">`text/html`ou `application/xhtml+xml` para o conteúdo HTML, inclusive para a parte obrigatória "Apresentação" de solicitações com várias partes. As solicitações com várias partes usam o tipo de conteúdo `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e8f8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e8f8-127">Request body</span></span>
<span data-ttu-id="3e8f8-128">No corpo da solicitação, forneça a página HTML do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-128">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="3e8f8-p104">O corpo pode conter HTML colocado diretamente no corpo da solicitação ou pode conter um formato de mensagem com várias partes conforme mostrado no exemplo. Se você estiver enviando dados binários, envie uma solicitação com várias partes.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="3e8f8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e8f8-131">Response</span></span>

<span data-ttu-id="3e8f8-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o novo objeto [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-132">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e8f8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e8f8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e8f8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e8f8-134">Request</span></span>
<span data-ttu-id="3e8f8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-135">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
Content-length: 312
Content-type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with <i>rendered</i> images and an <b>attached</b> file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an online source:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as binary data:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```
##### <a name="response"></a><span data-ttu-id="3e8f8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e8f8-136">Response</span></span>
<span data-ttu-id="3e8f8-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-137">Here is an example of the response.</span></span> <span data-ttu-id="3e8f8-138">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-138">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="3e8f8-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e8f8-139">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
