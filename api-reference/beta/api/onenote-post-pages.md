---
title: Criar página
description: Crie uma nova página do OneNote na seção padrão do bloco de anotações padrão.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 6c6c464d500e1b05974a81662d4eb99c2ce7c360
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456527"
---
# <a name="create-page"></a><span data-ttu-id="51b79-103">Criar página</span><span class="sxs-lookup"><span data-stu-id="51b79-103">Create page</span></span>

<span data-ttu-id="51b79-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="51b79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b79-105">Crie uma nova página do OneNote na seção padrão do bloco de anotações padrão.</span><span class="sxs-lookup"><span data-stu-id="51b79-105">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="51b79-106">Para criar uma página em uma seção diferente no bloco de anotações padrão, você pode usar `sectionName` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="51b79-106">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.</span></span>  <span data-ttu-id="51b79-107">Exemplo: `../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="51b79-107">Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="51b79-108">A `POST /onenote/pages` operação é usada apenas para criar páginas no bloco de anotações padrão do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="51b79-108">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook.</span></span> <span data-ttu-id="51b79-109">Se você estiver direcionando outros blocos de anotações, poderá [criar páginas em uma seção especificada](../api/section-post-pages.md).</span><span class="sxs-lookup"><span data-stu-id="51b79-109">If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>      

> <span data-ttu-id="51b79-110">**Observação:** Há um limite para o número de páginas que podem ser adicionadas a uma seção usando essa API.</span><span class="sxs-lookup"><span data-stu-id="51b79-110">**Note:** There is a limit to the number of pages that can be added to a section using this API.</span></span> <span data-ttu-id="51b79-111">Para obter detalhes, consulte [criar páginas do OneNote](/graph/onenote-create-page) para todas as limitações com esta API.</span><span class="sxs-lookup"><span data-stu-id="51b79-111">For details, see [Create OneNote pages](/graph/onenote-create-page) for all limitations with this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="51b79-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="51b79-112">Permissions</span></span>
<span data-ttu-id="51b79-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51b79-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51b79-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51b79-115">Permission type</span></span>      | <span data-ttu-id="51b79-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51b79-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51b79-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51b79-117">Delegated (work or school account)</span></span> | <span data-ttu-id="51b79-118">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51b79-118">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="51b79-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51b79-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51b79-120">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51b79-120">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="51b79-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51b79-121">Application</span></span> | <span data-ttu-id="51b79-122">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51b79-122">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51b79-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51b79-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="51b79-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51b79-124">Request headers</span></span>  
| <span data-ttu-id="51b79-125">Nome</span><span class="sxs-lookup"><span data-stu-id="51b79-125">Name</span></span>       | <span data-ttu-id="51b79-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="51b79-126">Type</span></span> | <span data-ttu-id="51b79-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="51b79-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51b79-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="51b79-128">Authorization</span></span>  | <span data-ttu-id="51b79-129">string</span><span class="sxs-lookup"><span data-stu-id="51b79-129">string</span></span>  | <span data-ttu-id="51b79-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51b79-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51b79-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51b79-132">Content-Type</span></span> | <span data-ttu-id="51b79-133">string</span><span class="sxs-lookup"><span data-stu-id="51b79-133">string</span></span> | <span data-ttu-id="51b79-p106">`text/html`ou `application/xhtml+xml` para o conteúdo HTML, inclusive para a parte obrigatória "Apresentação" de solicitações com várias partes. As solicitações com várias partes usam o tipo de conteúdo `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="51b79-p106">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51b79-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51b79-136">Request body</span></span>
<span data-ttu-id="51b79-137">No corpo da solicitação, forneça o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="51b79-137">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="51b79-p107">O corpo pode conter HTML colocado diretamente no corpo da solicitação ou pode conter um formato de mensagem com várias partes conforme mostrado no exemplo. Se você estiver enviando dados binários, envie uma solicitação com várias partes.</span><span class="sxs-lookup"><span data-stu-id="51b79-p107">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="51b79-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="51b79-140">Response</span></span>

<span data-ttu-id="51b79-141">Se tiver êxito, este método retornará `201 Created` um código de resposta e o novo objeto [OneNotePage](../resources/onenotepage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51b79-141">If successful, this method returns a `201 Created` response code and the new [onenotepage](../resources/onenotepage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51b79-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51b79-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51b79-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51b79-143">Request</span></span>
<span data-ttu-id="51b79-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51b79-144">Here is an example of the request.</span></span>

<span data-ttu-id="51b79-145">No `../onenote/pages` caminho, você pode usar o `sectionName` parâmetro de consulta para criar uma página em uma seção específica no bloco de anotações padrão.</span><span class="sxs-lookup"><span data-stu-id="51b79-145">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook.</span></span> <span data-ttu-id="51b79-146">Exemplo: `../onenote/pages?sectionName=My%20section`.</span><span class="sxs-lookup"><span data-stu-id="51b79-146">Example: `../onenote/pages?sectionName=My%20section`.</span></span> <span data-ttu-id="51b79-147">Se a seção não existir (ou tiver sido renomeada), a API criará uma nova seção.</span><span class="sxs-lookup"><span data-stu-id="51b79-147">If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

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
##### <a name="response"></a><span data-ttu-id="51b79-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="51b79-148">Response</span></span>
<span data-ttu-id="51b79-p109">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51b79-p109">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
