---
title: Criar página
description: Crie uma nova página na seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 8df217f4ebc84eebaa0ff938028ef3b571058808
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067661"
---
# <a name="create-page"></a><span data-ttu-id="04329-103">Criar página</span><span class="sxs-lookup"><span data-stu-id="04329-103">Create page</span></span>

<span data-ttu-id="04329-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04329-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04329-105">Crie uma nova [página](../resources/onenotepage.md) na seção especificado.</span><span class="sxs-lookup"><span data-stu-id="04329-105">Create a new [page](../resources/onenotepage.md) in the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="04329-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="04329-106">Permissions</span></span>
<span data-ttu-id="04329-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04329-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04329-109">Permission type</span></span>      | <span data-ttu-id="04329-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04329-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04329-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04329-111">Delegated (work or school account)</span></span> | <span data-ttu-id="04329-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04329-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="04329-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04329-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04329-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04329-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="04329-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04329-115">Application</span></span> | <span data-ttu-id="04329-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04329-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04329-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04329-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="04329-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04329-118">Request headers</span></span>
| <span data-ttu-id="04329-119">Nome</span><span class="sxs-lookup"><span data-stu-id="04329-119">Name</span></span>       | <span data-ttu-id="04329-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="04329-120">Type</span></span> | <span data-ttu-id="04329-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="04329-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04329-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="04329-122">Authorization</span></span>  | <span data-ttu-id="04329-123">string</span><span class="sxs-lookup"><span data-stu-id="04329-123">string</span></span>  | <span data-ttu-id="04329-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04329-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04329-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04329-126">Content-Type</span></span> | <span data-ttu-id="04329-127">string</span><span class="sxs-lookup"><span data-stu-id="04329-127">string</span></span> | <span data-ttu-id="04329-p103">`text/html`ou `application/xhtml+xml` para o conteúdo HTML, inclusive para a parte obrigatória "Apresentação" de solicitações com várias partes. As solicitações com várias partes usam o tipo de conteúdo `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="04329-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04329-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04329-130">Request body</span></span>
<span data-ttu-id="04329-131">No corpo da solicitação, forneça a página HTML do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="04329-131">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="04329-p104">O corpo pode conter HTML colocado diretamente no corpo da solicitação ou pode conter um formato de mensagem com várias partes conforme mostrado no exemplo. Se você estiver enviando dados binários, envie uma solicitação com várias partes.</span><span class="sxs-lookup"><span data-stu-id="04329-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="04329-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="04329-134">Response</span></span>

<span data-ttu-id="04329-135">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o novo objeto [onenotePage](../resources/onenotepage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04329-135">If successful, this method returns `201 Created` response code and the new [onenotePage](../resources/onenotepage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04329-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04329-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04329-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04329-137">Request</span></span>
<span data-ttu-id="04329-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04329-138">Here is an example of the request.</span></span>

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
##### <a name="response"></a><span data-ttu-id="04329-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="04329-139">Response</span></span>
<span data-ttu-id="04329-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04329-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


