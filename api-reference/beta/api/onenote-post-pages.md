---
title: Criar página
description: Crie uma nova página do OneNote na seção padrão do bloco de anotações padrão.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 4e70a113cd3a5f43e7a904d49a00840708bb4333
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992651"
---
# <a name="create-page"></a><span data-ttu-id="6187a-103">Criar página</span><span class="sxs-lookup"><span data-stu-id="6187a-103">Create page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6187a-104">Crie uma nova página do OneNote na seção padrão do bloco de anotações padrão.</span><span class="sxs-lookup"><span data-stu-id="6187a-104">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="6187a-105">Para criar uma página em uma seção diferente no bloco de anotações padrão, você pode usar `sectionName` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="6187a-105">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.</span></span>  <span data-ttu-id="6187a-106">Exemplo: `../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="6187a-106">Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="6187a-107">A `POST /onenote/pages` operação é usada apenas para criar páginas no bloco de anotações padrão do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="6187a-107">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook.</span></span> <span data-ttu-id="6187a-108">Se você estiver direcionando outros blocos de anotações, poderá [criar páginas em uma seção especificada](../api/section-post-pages.md).</span><span class="sxs-lookup"><span data-stu-id="6187a-108">If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>           
## <a name="permissions"></a><span data-ttu-id="6187a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6187a-109">Permissions</span></span>
<span data-ttu-id="6187a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6187a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6187a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6187a-112">Permission type</span></span>      | <span data-ttu-id="6187a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6187a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6187a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6187a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6187a-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6187a-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6187a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6187a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6187a-117">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6187a-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6187a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6187a-118">Application</span></span> | <span data-ttu-id="6187a-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6187a-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6187a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6187a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="6187a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6187a-121">Request headers</span></span>  
| <span data-ttu-id="6187a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6187a-122">Name</span></span>       | <span data-ttu-id="6187a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="6187a-123">Type</span></span> | <span data-ttu-id="6187a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6187a-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6187a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6187a-125">Authorization</span></span>  | <span data-ttu-id="6187a-126">string</span><span class="sxs-lookup"><span data-stu-id="6187a-126">string</span></span>  | <span data-ttu-id="6187a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6187a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6187a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6187a-129">Content-Type</span></span> | <span data-ttu-id="6187a-130">string</span><span class="sxs-lookup"><span data-stu-id="6187a-130">string</span></span> | <span data-ttu-id="6187a-p105">`text/html`ou `application/xhtml+xml` para o conteúdo HTML, inclusive para a parte obrigatória "Apresentação" de solicitações com várias partes. As solicitações com várias partes usam o tipo de conteúdo `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="6187a-p105">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6187a-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6187a-133">Request body</span></span>
<span data-ttu-id="6187a-134">No corpo da solicitação, forneça o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="6187a-134">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="6187a-p106">O corpo pode conter HTML colocado diretamente no corpo da solicitação ou pode conter um formato de mensagem com várias partes conforme mostrado no exemplo. Se você estiver enviando dados binários, envie uma solicitação com várias partes.</span><span class="sxs-lookup"><span data-stu-id="6187a-p106">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="6187a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6187a-137">Response</span></span>

<span data-ttu-id="6187a-138">Se tiver êxito, este método retornará `201 Created` um código de resposta e o novo objeto [OneNotePage](../resources/onenotepage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6187a-138">If successful, this method returns a `201 Created` response code and the new [onenotepage](../resources/onenotepage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6187a-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6187a-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6187a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6187a-140">Request</span></span>
<span data-ttu-id="6187a-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6187a-141">Here is an example of the request.</span></span>

<span data-ttu-id="6187a-142">No `../onenote/pages` caminho, você pode usar o `sectionName` parâmetro de consulta para criar uma página em uma seção específica no bloco de anotações padrão.</span><span class="sxs-lookup"><span data-stu-id="6187a-142">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook.</span></span> <span data-ttu-id="6187a-143">Exemplo: `../onenote/pages?sectionName=My%20section`.</span><span class="sxs-lookup"><span data-stu-id="6187a-143">Example: `../onenote/pages?sectionName=My%20section`.</span></span> <span data-ttu-id="6187a-144">Se a seção não existir (ou tiver sido renomeada), a API criará uma nova seção.</span><span class="sxs-lookup"><span data-stu-id="6187a-144">If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages
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
##### <a name="response"></a><span data-ttu-id="6187a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6187a-145">Response</span></span>
<span data-ttu-id="6187a-p108">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6187a-p108">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
  "content": "content-value",
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
