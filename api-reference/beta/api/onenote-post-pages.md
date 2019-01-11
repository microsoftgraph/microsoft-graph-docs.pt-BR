---
title: Criar página
description: Crie uma nova página do OneNote na seção padrão do bloco de anotações padrão.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: ca5656015a79e5ee684845d12b815cb1ec5f5159
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858986"
---
# <a name="create-page"></a><span data-ttu-id="ca34d-103">Criar página</span><span class="sxs-lookup"><span data-stu-id="ca34d-103">Create page</span></span>

> <span data-ttu-id="ca34d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ca34d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca34d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ca34d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca34d-106">Crie uma nova página do OneNote na seção padrão do bloco de anotações padrão.</span><span class="sxs-lookup"><span data-stu-id="ca34d-106">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="ca34d-p102">Para criar uma página em outra seção no bloco de anotações padrão, use o parâmetro de consulta `sectionName`.  Exemplo: `../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="ca34d-p102">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.  Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="ca34d-p103">O operação `POST /onenote/pages` só é usada para criar páginas no bloco de anotações atual do usuário padrão. Se estiver direcionando para outros blocos de anotações, você pode [criar páginas em uma seção especificada](../api/section-post-pages.md).</span><span class="sxs-lookup"><span data-stu-id="ca34d-p103">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook. If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>           
## <a name="permissions"></a><span data-ttu-id="ca34d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca34d-111">Permissions</span></span>
<span data-ttu-id="ca34d-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca34d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca34d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca34d-114">Permission type</span></span>      | <span data-ttu-id="ca34d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca34d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca34d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca34d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ca34d-117">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca34d-117">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca34d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca34d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca34d-119">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca34d-119">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ca34d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca34d-120">Application</span></span> | <span data-ttu-id="ca34d-121">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca34d-121">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca34d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca34d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="ca34d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca34d-123">Request headers</span></span>  
| <span data-ttu-id="ca34d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ca34d-124">Name</span></span>       | <span data-ttu-id="ca34d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca34d-125">Type</span></span> | <span data-ttu-id="ca34d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca34d-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ca34d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca34d-127">Authorization</span></span>  | <span data-ttu-id="ca34d-128">string</span><span class="sxs-lookup"><span data-stu-id="ca34d-128">string</span></span>  | <span data-ttu-id="ca34d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca34d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca34d-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca34d-131">Content-Type</span></span> | <span data-ttu-id="ca34d-132">string</span><span class="sxs-lookup"><span data-stu-id="ca34d-132">string</span></span> | <span data-ttu-id="ca34d-p106">`text/html`ou `application/xhtml+xml` para o conteúdo HTML, inclusive para a parte obrigatória "Apresentação" de solicitações com várias partes. As solicitações com várias partes usam o tipo de conteúdo `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="ca34d-p106">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca34d-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca34d-135">Request body</span></span>
<span data-ttu-id="ca34d-136">No corpo da solicitação, forneça o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="ca34d-136">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="ca34d-p107">O corpo pode conter HTML colocado diretamente no corpo da solicitação ou pode conter um formato de mensagem com várias partes conforme mostrado no exemplo. Se você estiver enviando dados binários, envie uma solicitação com várias partes.</span><span class="sxs-lookup"><span data-stu-id="ca34d-p107">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="ca34d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca34d-139">Response</span></span>

<span data-ttu-id="ca34d-140">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o novo objeto [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca34d-140">If successful, this method returns a `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca34d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca34d-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca34d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca34d-142">Request</span></span>
<span data-ttu-id="ca34d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca34d-143">Here is an example of the request.</span></span>

<span data-ttu-id="ca34d-p108">No caminho `../onenote/pages`, você pode usar o parâmetro de consulta `sectionName` para criar uma página em uma seção específica no bloco de anotações padrão. Exemplo: `../onenote/pages?sectionName=My%20section`. Se a seção não existir (ou tiver sido renomeada), a API criará uma nova seção.</span><span class="sxs-lookup"><span data-stu-id="ca34d-p108">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook. Example: `../onenote/pages?sectionName=My%20section`. If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

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
##### <a name="response"></a><span data-ttu-id="ca34d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca34d-147">Response</span></span>
<span data-ttu-id="ca34d-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca34d-148">Here is an example of the response.</span></span> <span data-ttu-id="ca34d-149">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="ca34d-149">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="ca34d-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca34d-150">All of the properties will be returned from an actual call.</span></span>
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
  "content": "content-value",
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
