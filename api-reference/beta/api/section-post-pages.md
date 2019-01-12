---
title: Criar página
description: Crie uma nova página na seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8957609ffd3768edb456835b522dbbb7a145b6bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912789"
---
# <a name="create-page"></a><span data-ttu-id="96b63-103">Criar página</span><span class="sxs-lookup"><span data-stu-id="96b63-103">Create page</span></span>

> <span data-ttu-id="96b63-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="96b63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96b63-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="96b63-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96b63-106">Crie uma nova [página](../resources/page.md) na seção especificado.</span><span class="sxs-lookup"><span data-stu-id="96b63-106">Create a new [page](../resources/page.md) in the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="96b63-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="96b63-107">Permissions</span></span>
<span data-ttu-id="96b63-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96b63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96b63-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96b63-110">Permission type</span></span>      | <span data-ttu-id="96b63-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96b63-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96b63-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96b63-112">Delegated (work or school account)</span></span> | <span data-ttu-id="96b63-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96b63-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="96b63-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96b63-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96b63-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96b63-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="96b63-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96b63-116">Application</span></span> | <span data-ttu-id="96b63-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96b63-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96b63-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96b63-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="96b63-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96b63-119">Request headers</span></span>
| <span data-ttu-id="96b63-120">Nome</span><span class="sxs-lookup"><span data-stu-id="96b63-120">Name</span></span>       | <span data-ttu-id="96b63-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="96b63-121">Type</span></span> | <span data-ttu-id="96b63-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="96b63-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96b63-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96b63-123">Authorization</span></span>  | <span data-ttu-id="96b63-124">string</span><span class="sxs-lookup"><span data-stu-id="96b63-124">string</span></span>  | <span data-ttu-id="96b63-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96b63-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96b63-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96b63-127">Content-Type</span></span> | <span data-ttu-id="96b63-128">string</span><span class="sxs-lookup"><span data-stu-id="96b63-128">string</span></span> | <span data-ttu-id="96b63-p104">`text/html`ou `application/xhtml+xml` para o conteúdo HTML, inclusive para a parte obrigatória "Apresentação" de solicitações com várias partes. As solicitações com várias partes usam o tipo de conteúdo `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="96b63-p104">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96b63-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96b63-131">Request body</span></span>
<span data-ttu-id="96b63-132">No corpo da solicitação, forneça a página HTML do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="96b63-132">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="96b63-p105">O corpo pode conter HTML colocado diretamente no corpo da solicitação ou pode conter um formato de mensagem com várias partes conforme mostrado no exemplo. Se você estiver enviando dados binários, envie uma solicitação com várias partes.</span><span class="sxs-lookup"><span data-stu-id="96b63-p105">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="96b63-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="96b63-135">Response</span></span>

<span data-ttu-id="96b63-136">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o novo objeto [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96b63-136">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96b63-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96b63-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96b63-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96b63-138">Request</span></span>
<span data-ttu-id="96b63-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96b63-139">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/pages
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
##### <a name="response"></a><span data-ttu-id="96b63-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="96b63-140">Response</span></span>
<span data-ttu-id="96b63-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96b63-141">Here is an example of the response.</span></span> <span data-ttu-id="96b63-142">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="96b63-142">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="96b63-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96b63-143">All of the properties will be returned from an actual call.</span></span>
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
