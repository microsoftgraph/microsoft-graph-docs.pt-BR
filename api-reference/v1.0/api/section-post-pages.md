---
title: Criar página
description: Crie uma nova página na seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 3617022652bd1e5fc0df0ed3497fb4b5f2e4f576
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915484"
---
# <a name="create-page"></a><span data-ttu-id="9ef19-103">Criar página</span><span class="sxs-lookup"><span data-stu-id="9ef19-103">Create page</span></span>

<span data-ttu-id="9ef19-104">Crie uma nova [página](../resources/page.md) na seção especificado.</span><span class="sxs-lookup"><span data-stu-id="9ef19-104">Create a new [page](../resources/page.md) in the specified section.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ef19-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ef19-105">Permissions</span></span>
<span data-ttu-id="9ef19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ef19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ef19-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ef19-108">Permission type</span></span>      | <span data-ttu-id="9ef19-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ef19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ef19-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ef19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ef19-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef19-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ef19-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ef19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ef19-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ef19-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9ef19-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ef19-114">Application</span></span> | <span data-ttu-id="9ef19-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef19-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ef19-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ef19-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="9ef19-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef19-117">Request headers</span></span>
| <span data-ttu-id="9ef19-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9ef19-118">Name</span></span>       | <span data-ttu-id="9ef19-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ef19-119">Type</span></span> | <span data-ttu-id="9ef19-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ef19-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ef19-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ef19-121">Authorization</span></span>  | <span data-ttu-id="9ef19-122">string</span><span class="sxs-lookup"><span data-stu-id="9ef19-122">string</span></span>  | <span data-ttu-id="9ef19-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ef19-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ef19-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ef19-125">Content-Type</span></span> | <span data-ttu-id="9ef19-126">string</span><span class="sxs-lookup"><span data-stu-id="9ef19-126">string</span></span> | <span data-ttu-id="9ef19-p103">`text/html`ou `application/xhtml+xml` para o conteúdo HTML, inclusive para a parte obrigatória "Apresentação" de solicitações com várias partes. As solicitações com várias partes usam o tipo de conteúdo `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="9ef19-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ef19-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef19-129">Request body</span></span>
<span data-ttu-id="9ef19-130">No corpo da solicitação, forneça a página HTML do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9ef19-130">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="9ef19-p104">O corpo pode conter HTML colocado diretamente no corpo da solicitação ou pode conter um formato de mensagem com várias partes conforme mostrado no exemplo. Se você estiver enviando dados binários, envie uma solicitação com várias partes.</span><span class="sxs-lookup"><span data-stu-id="9ef19-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="9ef19-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ef19-133">Response</span></span>

<span data-ttu-id="9ef19-134">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o novo objeto [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ef19-134">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ef19-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ef19-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ef19-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef19-136">Request</span></span>
<span data-ttu-id="9ef19-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ef19-137">Here is an example of the request.</span></span>

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
##### <a name="response"></a><span data-ttu-id="9ef19-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ef19-138">Response</span></span>
<span data-ttu-id="9ef19-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ef19-139">Here is an example of the response.</span></span> <span data-ttu-id="9ef19-140">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="9ef19-140">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="9ef19-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ef19-141">All of the properties will be returned from an actual call.</span></span>
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
