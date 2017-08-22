# <a name="create-page"></a><span data-ttu-id="a0afb-101">Criar página</span><span class="sxs-lookup"><span data-stu-id="a0afb-101">Create page</span></span>

<span data-ttu-id="a0afb-102">Crie uma nova [página](../resources/page.md) na seção especificado.</span><span class="sxs-lookup"><span data-stu-id="a0afb-102">Create a new [page](../resources/page.md) in the specified section.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0afb-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0afb-103">Prerequisites</span></span>
<span data-ttu-id="a0afb-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="a0afb-104">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="a0afb-105">Notes.Create, Notes.ReadWrite ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0afb-105">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="a0afb-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0afb-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="a0afb-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0afb-107">Request headers</span></span>
| <span data-ttu-id="a0afb-108">Nome</span><span class="sxs-lookup"><span data-stu-id="a0afb-108">Name</span></span>       | <span data-ttu-id="a0afb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0afb-109">Type</span></span> | <span data-ttu-id="a0afb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0afb-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a0afb-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0afb-111">Authorization</span></span>  | <span data-ttu-id="a0afb-112">string</span><span class="sxs-lookup"><span data-stu-id="a0afb-112">string</span></span>  | <span data-ttu-id="a0afb-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0afb-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0afb-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0afb-115">Content-Type</span></span> | <span data-ttu-id="a0afb-116">string</span><span class="sxs-lookup"><span data-stu-id="a0afb-116">string</span></span> | <span data-ttu-id="a0afb-p102">`text/html`ou `application/xhtml+xml` para o conteúdo HTML, inclusive para a parte obrigatória "Apresentação" de solicitações com várias partes. As solicitações com várias partes usam o tipo de conteúdo `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="a0afb-p102">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0afb-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0afb-119">Request body</span></span>
<span data-ttu-id="a0afb-120">No corpo da solicitação, forneça a página HTML do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a0afb-120">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="a0afb-p103">O corpo pode conter HTML colocado diretamente no corpo da solicitação ou pode conter um formato de mensagem com várias partes conforme mostrado no exemplo. Se você estiver enviando dados binários, envie uma solicitação com várias partes.</span><span class="sxs-lookup"><span data-stu-id="a0afb-p103">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="a0afb-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0afb-123">Response</span></span>

<span data-ttu-id="a0afb-124">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o novo objeto [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0afb-124">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0afb-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0afb-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0afb-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0afb-126">Request</span></span>
<span data-ttu-id="a0afb-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0afb-127">Here is an example of the request.</span></span>

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
    <img src="http://..." alt="an image on the page" width="500" />
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
##### <a name="response"></a><span data-ttu-id="a0afb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0afb-128">Response</span></span>
<span data-ttu-id="a0afb-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0afb-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
