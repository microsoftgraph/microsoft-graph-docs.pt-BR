---
title: Adicionar imagens, vídeos e arquivos a páginas do OneNote
description: " Blocos de anotações empresariais no Microsoft 365"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: b601495db396d136a1181c81431f70c025475d45
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474901"
---
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="f3626-103">Adicionar imagens, vídeos e arquivos a páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="f3626-103">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="f3626-104">**Aplica-se a** Notebooks de consumidores no OneDrive | Notebooks corporativos no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f3626-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="f3626-105">Você pode usar os elementos **img**, **object** e **iframe** para adicionar imagens, vídeos e arquivos à página do OneNote quando você [criar](onenote-create-page.md) ou [atualizar](onenote-update-page.md) a página.</span><span class="sxs-lookup"><span data-stu-id="f3626-105">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote-update-page.md) the page.</span></span> 

- <span data-ttu-id="f3626-106">Use **img** para renderizar uma imagem na página.</span><span class="sxs-lookup"><span data-stu-id="f3626-106">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="f3626-107">Use **iframe** para inserir um vídeo na página.</span><span class="sxs-lookup"><span data-stu-id="f3626-107">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="f3626-108">Use **object** para adicionar um anexo de arquivo na página.</span><span class="sxs-lookup"><span data-stu-id="f3626-108">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>

## <a name="adding-images"></a><span data-ttu-id="f3626-109">Adicionar imagens</span><span class="sxs-lookup"><span data-stu-id="f3626-109">Adding images</span></span>

<span data-ttu-id="f3626-110">Imagens podem ser adicionadas por referência de URL ou enviando dados brutos.</span><span class="sxs-lookup"><span data-stu-id="f3626-110">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="f3626-111">Os seguintes métodos de adição de imagens, logotipos e fotos para páginas do OneNote são compatíveis com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f3626-111">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="f3626-112">Adicionar uma imagem pública da Web</span><span class="sxs-lookup"><span data-stu-id="f3626-112">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)

<span data-ttu-id="f3626-113">Use `img` com `src="https://image-url"` e especifique a URL de uma imagem acessível ao público.</span><span class="sxs-lookup"><span data-stu-id="f3626-113">Use `img` with `src="https://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="f3626-114">Renderiza a imagem na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-114">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="f3626-115">Adicionar uma imagem usando dados binários</span><span class="sxs-lookup"><span data-stu-id="f3626-115">Add an image using binary data</span></span>](#add-an-image-using-binary-data)

<span data-ttu-id="f3626-116">Use `img` com `src="name:image-block-name"` e envie o arquivo de imagem em uma parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="f3626-116">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="f3626-117">Renderiza a imagem na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-117">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="f3626-118">Adicionar um instantâneo de página da Web</span><span class="sxs-lookup"><span data-stu-id="f3626-118">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)

<span data-ttu-id="f3626-119">Use `img` com `data-render-src="https://webpage-url"` e especifique a URL de uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="f3626-119">Use `img` with `data-render-src="https://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="f3626-120">Renderiza um instantâneo da página da Web inteira na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-120">Renders a snapshot of the whole webpage on the OneNote page.</span></span>

[<span data-ttu-id="f3626-121">Adicionar uma imagem renderizada de HTML</span><span class="sxs-lookup"><span data-stu-id="f3626-121">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)

<span data-ttu-id="f3626-122">Use `img` com `data-render-src="name:html-block-name"` e envie HTML na parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="f3626-122">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="f3626-123">Renderiza o HTML como uma imagem na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-123">Renders the HTML as an image on the OneNote page.</span></span>

[<span data-ttu-id="f3626-124">Adicionar imagens de conteúdos de arquivo PDF</span><span class="sxs-lookup"><span data-stu-id="f3626-124">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="f3626-125">Use `<img data-render-src="name:part-name" />` e envie o arquivo PDF na parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="f3626-125">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="f3626-126">Renderiza cada página do PDF como uma imagem separada na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-126">Renders each PDF page as a separate image on the OneNote page.</span></span>

[<span data-ttu-id="f3626-127">Adicionar um arquivo de imagem como um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="f3626-127">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)

<span data-ttu-id="f3626-128">Use `object` com `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` e envie um arquivo de imagem em uma parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="f3626-128">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="f3626-129">Adiciona um anexo de arquivo à página do OneNote e exibe um ícone de arquivo.</span><span class="sxs-lookup"><span data-stu-id="f3626-129">Adds a file attachment to the OneNote page and displays a file icon.</span></span>


> <span data-ttu-id="f3626-130">**Observação:** para inserir imagens em uma página do OneNote, primeiro envie uma [solicitação GET para o conteúdo da página](onenote-get-content.md#page-html-content).</span><span class="sxs-lookup"><span data-stu-id="f3626-130">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="f3626-131">Isso retornará as URLs para recursos de imagem na página.</span><span class="sxs-lookup"><span data-stu-id="f3626-131">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="f3626-132">Em seguida, separe as [solicitações GET dos recursos de imagem](onenote-get-content.md#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="f3626-132">You then separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


#### <a name="image-attributes"></a><span data-ttu-id="f3626-133">Atributos de imagem</span><span class="sxs-lookup"><span data-stu-id="f3626-133">Image attributes</span></span> 

<span data-ttu-id="f3626-134">Um elemento **img** pode incluir opcionalmente atributos **alt**, **height** e **width** e os atributos de estilo **max-width** e **max-height**.</span><span class="sxs-lookup"><span data-stu-id="f3626-134">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

#### <a name="image-media-types"></a><span data-ttu-id="f3626-135">Tipos de mídia de imagem</span><span class="sxs-lookup"><span data-stu-id="f3626-135">Image media types</span></span>

<span data-ttu-id="f3626-136">O Microsoft Graph é compatível com os tipos de imagem TIFF, PNG, GIF, JPEG e BMP.</span><span class="sxs-lookup"><span data-stu-id="f3626-136">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="f3626-137">Para capturar uma imagem que usa um formato diferente que você não quer converter, [envie dados binários](#add-an-image-using-binary-data) em uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="f3626-137">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="f3626-138">Não é necessário usar Base64 ou codificar os dados binários que você enviar.</span><span class="sxs-lookup"><span data-stu-id="f3626-138">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="f3626-139">**Observação:** a API detecta o tipo de imagem de entrada e o retorna como o atributo **data-fullres-src-type** no [HTML de saída](onenote-input-output-html.md#output-html).</span><span class="sxs-lookup"><span data-stu-id="f3626-139">**Note:** The API detects the original input image type, and returns it as the **data-fullres-src-type** attribute in the [output HTML](onenote-input-output-html.md#output-html).</span></span> <span data-ttu-id="f3626-140">A API também retorna o tipo de imagem da imagem otimizada em **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="f3626-140">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="f3626-141">Ver [limitações](#size-limitations-for-post-pages-requests) que se aplicam ao criar páginas que contém mídia.</span><span class="sxs-lookup"><span data-stu-id="f3626-141">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>

### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="f3626-142">Adicionar uma imagem pública da Web</span><span class="sxs-lookup"><span data-stu-id="f3626-142">Add a public image from the web</span></span>

<span data-ttu-id="f3626-143">No HTML de entrada da sua solicitação, inclua `<img src="https://..." />` e especifique a URL de uma imagem publicamente acessível para o atributo **src**.</span><span class="sxs-lookup"><span data-stu-id="f3626-143">In the input HTML of your request, include `<img src="https://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Public URL</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image from the web.</p>
    <img src="https://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>

### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="f3626-144">Adicionar uma imagem usando dados binários</span><span class="sxs-lookup"><span data-stu-id="f3626-144">Add an image using binary data</span></span>

<span data-ttu-id="f3626-145">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<img src="name:part-name" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de imagem binária.</span><span class="sxs-lookup"><span data-stu-id="f3626-145">In the input HTML of your request's **Presentation** part, include `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="f3626-146">Basta enviar dados binários, não use Base64 ou codifique.</span><span class="sxs-lookup"><span data-stu-id="f3626-146">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Image binary data</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the uploaded image.</p>
    <img src="name:image-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="MyAppPictureId"
Content-Type: image/jpeg

... image binary data ...

--MyAppPartBoundary--  
```


<a name="image-img-url-data-render-src"></a>

### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="f3626-147">Adicionar um instantâneo de página da Web</span><span class="sxs-lookup"><span data-stu-id="f3626-147">Add a webpage snapshot</span></span>

<span data-ttu-id="f3626-148">Você pode usar o Microsoft Graph para fazer instantâneos inteiros de páginas da Web e inseri-los em novas páginas.</span><span class="sxs-lookup"><span data-stu-id="f3626-148">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="f3626-149">Esse método é útil para arquivar páginas da Web ou capturar páginas da Web complexas que possuem recursos não compatíveis com o OneNote (como algumas CSS).</span><span class="sxs-lookup"><span data-stu-id="f3626-149">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="f3626-150">No HTML de entrada da sua solicitação, inclua `<img src="https://..." />` e especifique a URL de uma página da Web que você quer inserir para o atributo **src**.</span><span class="sxs-lookup"><span data-stu-id="f3626-150">In the input HTML of your request, include `<img src="https://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Webpage capture</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image of the webpage.</p>
    <img data-render-src="https://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>

### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="f3626-151">Adicionar uma imagem renderizada de HTML</span><span class="sxs-lookup"><span data-stu-id="f3626-151">Add an image rendered from HTML</span></span>

<span data-ttu-id="f3626-152">Quando você passar o HTML como um bloco de dados, certifique-se de que não haja conteúdo ativo que exija credenciais de usuário ou um plug-in de navegador pré-carregado.</span><span class="sxs-lookup"><span data-stu-id="f3626-152">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="f3626-153">O mecanismo que o Microsoft Graph usa para renderizar a página HTML em uma imagem não tem a capacidade de fazer logon de um usuário e não inclui plug-ins como Adobe Flash, Apple QuickTime entre outros.</span><span class="sxs-lookup"><span data-stu-id="f3626-153">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so on.</span></span> <span data-ttu-id="f3626-154">Isso também significa que o conteúdo carregado dinamicamente, que pode vir com um script AJAX, não será exibido se a obtenção dos dados exigir credenciais de logon do usuário ou cookies.</span><span class="sxs-lookup"><span data-stu-id="f3626-154">That also means that dynamically-loaded content, such as might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="f3626-155">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<img data-render-src="name:part-name" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém o HTML.</span><span class="sxs-lookup"><span data-stu-id="f3626-155">In the input HTML of your request's **Presentation** part, include `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>


```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: HTML block</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the block of HTML as an image.</p>
    <img data-render-src="name:html-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="html-block-name"
Content-Type: text/html

<html>
<body>
<h1>This HTML will render as an image</h1>
<p><b>Don't</b> try to embed another <i>data-render-src</i> type-image inside the HTML part--
it won't work. Instead, use URL-based real images like this:</p>
<img src="https://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>

### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="f3626-156">Adicionar um arquivo de imagem como um anexo</span><span class="sxs-lookup"><span data-stu-id="f3626-156">Add an image file as an attachment</span></span>

<span data-ttu-id="f3626-157">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de imagem binária.</span><span class="sxs-lookup"><span data-stu-id="f3626-157">In the input HTML of your request's **Presentation** part, include `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="f3626-158">Basta enviar dados binários, não use Base64 ou codifique.</span><span class="sxs-lookup"><span data-stu-id="f3626-158">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Binary image data as file attachment</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page contains the image as a file attachment.</p>
    <object data-attachment="image-file.jpg" data="name:image-block-name" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```

<span data-ttu-id="f3626-159">Saiba mais sobre [tipos de mídia de arquivos](#file-media-types).</span><span class="sxs-lookup"><span data-stu-id="f3626-159">Learn more about [file media types](#file-media-types).</span></span>



<a name="adding-videos"></a>

## <a name="adding-videos"></a><span data-ttu-id="f3626-160">Adicionar vídeos</span><span class="sxs-lookup"><span data-stu-id="f3626-160">Adding videos</span></span>

<span data-ttu-id="f3626-161">Você pode inserir vídeos em páginas do OneNote usando `<iframe data-original-src="https://..." />` no HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="f3626-161">You can embed videos in OneNote pages using `<iframe data-original-src="https://..." />` in the input HTML.</span></span> 

### <a name="supported-video-sites"></a><span data-ttu-id="f3626-162">Sites de vídeo compatíveis</span><span class="sxs-lookup"><span data-stu-id="f3626-162">Supported video sites</span></span>

- <span data-ttu-id="f3626-163">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="f3626-163">Dailymotion</span></span>
- <span data-ttu-id="f3626-164">Office Mix</span><span class="sxs-lookup"><span data-stu-id="f3626-164">Office Mix</span></span>
- <span data-ttu-id="f3626-165">Sway</span><span class="sxs-lookup"><span data-stu-id="f3626-165">Sway</span></span>
- <span data-ttu-id="f3626-166">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="f3626-166">Sketchfab</span></span>
- <span data-ttu-id="f3626-167">TED</span><span class="sxs-lookup"><span data-stu-id="f3626-167">TED</span></span>
- <span data-ttu-id="f3626-168">YouTube</span><span class="sxs-lookup"><span data-stu-id="f3626-168">YouTube</span></span>
- <span data-ttu-id="f3626-169">Vimeo</span><span class="sxs-lookup"><span data-stu-id="f3626-169">Vimeo</span></span>
- <span data-ttu-id="f3626-170">Vine</span><span class="sxs-lookup"><span data-stu-id="f3626-170">Vine</span></span>

### <a name="iframe-attributes"></a><span data-ttu-id="f3626-171">atributos de iframe</span><span class="sxs-lookup"><span data-stu-id="f3626-171">iframe attributes</span></span>

#### <a name="data-original-src"></a><span data-ttu-id="f3626-172">data-original-src</span><span class="sxs-lookup"><span data-stu-id="f3626-172">data-original-src</span></span>

<span data-ttu-id="f3626-173">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3626-173">Required.</span></span> <span data-ttu-id="f3626-174">A URL do vídeo.</span><span class="sxs-lookup"><span data-stu-id="f3626-174">The URL of the video.</span></span>

<span data-ttu-id="f3626-175">Exemplo: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="f3626-175">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span>

#### <a name="width"></a><span data-ttu-id="f3626-176">width</span><span class="sxs-lookup"><span data-stu-id="f3626-176">width</span></span>

<span data-ttu-id="f3626-177">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f3626-177">Optional.</span></span> <span data-ttu-id="f3626-178">A largura do iframe que contém o vídeo.</span><span class="sxs-lookup"><span data-stu-id="f3626-178">The width of the iframe that contains the video.</span></span> <span data-ttu-id="f3626-179">O padrão é 480.</span><span class="sxs-lookup"><span data-stu-id="f3626-179">Default is 480.</span></span>

<span data-ttu-id="f3626-180">Exemplo: `width="300"`</span><span class="sxs-lookup"><span data-stu-id="f3626-180">Example: `width="300"`</span></span>

#### <a name="height"></a><span data-ttu-id="f3626-181">height</span><span class="sxs-lookup"><span data-stu-id="f3626-181">height</span></span>

<span data-ttu-id="f3626-182">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f3626-182">Optional.</span></span> <span data-ttu-id="f3626-183">A altura do iframe que contém o vídeo.</span><span class="sxs-lookup"><span data-stu-id="f3626-183">The height of the iframe that contains the video.</span></span> <span data-ttu-id="f3626-184">O padrão é 360.</span><span class="sxs-lookup"><span data-stu-id="f3626-184">Default is 360.</span></span>

<span data-ttu-id="f3626-185">Exemplo: `height="300"`</span><span class="sxs-lookup"><span data-stu-id="f3626-185">Example: `height="300"`</span></span>

### <a name="example"></a><span data-ttu-id="f3626-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3626-186">Example</span></span>

<span data-ttu-id="f3626-187">No HTML de entrada da sua solicitação, inclua `<iframe data-original-src="https://..." />` e especifique a URL do vídeo para o atributo **data-original-src**.</span><span class="sxs-lookup"><span data-stu-id="f3626-187">In the input HTML of your request, include `<iframe data-original-src="https://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
    <head>
        <title>A page with an embedded video</title>
    </head>
    <body>
        <iframe data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" width="340" height="280"/>
    </body>
</html>

--MyAppPartBoundary--
```


<a name="adding-files"></a>

## <a name="adding-files"></a><span data-ttu-id="f3626-188">Adicionar arquivos</span><span class="sxs-lookup"><span data-stu-id="f3626-188">Adding files</span></span>

<span data-ttu-id="f3626-189">Você pode adicionar anexos de arquivo a páginas do OneNote usando um elemento **object** de HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="f3626-189">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="f3626-190">Se você estiver adicionando um arquivo PDF, você pode usar um elemento de **img** para renderizar as páginas de PDF como imagens.</span><span class="sxs-lookup"><span data-stu-id="f3626-190">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="f3626-191">Adicionar um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="f3626-191">Add a file attachment</span></span>](#add-a-file-attachment)

<span data-ttu-id="f3626-192">Use `<object .../>` e envie o arquivo na parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="f3626-192">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="f3626-193">Adiciona um anexo de arquivo que exibe um ícone de arquivo na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-193">Adds a file attachment that displays a file icon on the OneNote page.</span></span>

[<span data-ttu-id="f3626-194">Adicionar imagens de conteúdos de arquivo PDF</span><span class="sxs-lookup"><span data-stu-id="f3626-194">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="f3626-195">Use `<img data-render-src="name:part-name" />` e envie um arquivo PDF na parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="f3626-195">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="f3626-196">Renderiza cada página do PDF como uma imagem separada na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-196">Renders each PDF page as a separate image on the OneNote page.</span></span>

#### <a name="file-attributes"></a><span data-ttu-id="f3626-197">Atributos de arquivo</span><span class="sxs-lookup"><span data-stu-id="f3626-197">File attributes</span></span>

<span data-ttu-id="f3626-198">O elemento **object** requer os seguintes atributos.</span><span class="sxs-lookup"><span data-stu-id="f3626-198">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="f3626-199">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="f3626-199">**data-attachment**</span></span>

<span data-ttu-id="f3626-200">O nome e a extensão do arquivo para exibir na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-200">The file name and extension to display on the OneNote page.</span></span>

<span data-ttu-id="f3626-201">Exemplo: `data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="f3626-201">Example: `data-attachment="filename.docx"`</span></span>

<span data-ttu-id="f3626-202">**data**</span><span class="sxs-lookup"><span data-stu-id="f3626-202">**data**</span></span>

<span data-ttu-id="f3626-203">O nome da parte do corpo na solicitação de várias partes que contém os dados de arquivo binário.</span><span class="sxs-lookup"><span data-stu-id="f3626-203">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="f3626-204">O Microsoft Graph não é compatível com a passagem de uma referência de URL aqui.</span><span class="sxs-lookup"><span data-stu-id="f3626-204">Microsoft Graph does not support passing a URL reference here.</span></span>

<span data-ttu-id="f3626-205">Exemplo: `data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="f3626-205">Example: `data="name:part-name"`</span></span>

<span data-ttu-id="f3626-206">**type**</span><span class="sxs-lookup"><span data-stu-id="f3626-206">**type**</span></span>

<span data-ttu-id="f3626-207">O tipo de mídia de arquivo, usado para determinar o ícone de arquivo a ser usado na página e qual aplicativo é iniciado quando o usuário ativa o arquivo no dispositivo a partir do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-207">The file media type, used to determine the file icon to use on the page, and which application starts when the user activates the file on the device from OneNote.</span></span>

<span data-ttu-id="f3626-208">Exemplo: `type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="f3626-208">Example: `type="application/pdf"`</span></span>


<a name="file-media-types"></a>

#### <a name="file-media-types"></a><span data-ttu-id="f3626-209">Tipos de mídia de arquivo</span><span class="sxs-lookup"><span data-stu-id="f3626-209">File media types</span></span>  

<span data-ttu-id="f3626-210">O Microsoft Graph usa o ícone de tipos de arquivo predefinido para arquivos anexos ou um ícone genérico quando a API não reconhece o tipo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="f3626-210">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="f3626-211">A tabela a seguir mostra alguns tipos de arquivos comuns reconhecidos pela API.</span><span class="sxs-lookup"><span data-stu-id="f3626-211">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="f3626-212">application/pdf</span><span class="sxs-lookup"><span data-stu-id="f3626-212">application/pdf</span></span>  
- <span data-ttu-id="f3626-213">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="f3626-213">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="f3626-214">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="f3626-214">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="f3626-215">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="f3626-215">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="f3626-216">image/png</span><span class="sxs-lookup"><span data-stu-id="f3626-216">image/png</span></span>
- <span data-ttu-id="f3626-217">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="f3626-217">image/jpeg</span></span>
- <span data-ttu-id="f3626-218">image/gif</span><span class="sxs-lookup"><span data-stu-id="f3626-218">image/gif</span></span>
- <span data-ttu-id="f3626-219">audio/wav</span><span class="sxs-lookup"><span data-stu-id="f3626-219">audio/wav</span></span>
- <span data-ttu-id="f3626-220">video/mp4</span><span class="sxs-lookup"><span data-stu-id="f3626-220">video/mp4</span></span>
- <span data-ttu-id="f3626-221">application/msword</span><span class="sxs-lookup"><span data-stu-id="f3626-221">application/msword</span></span>
- <span data-ttu-id="f3626-222">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="f3626-222">application/mspowerpoint</span></span>
- <span data-ttu-id="f3626-223">application/excel</span><span class="sxs-lookup"><span data-stu-id="f3626-223">application/excel</span></span>

<span data-ttu-id="f3626-224">Ver [limitações](#size-limitations-for-post-pages-requests) que se aplicam ao criar páginas que contém mídia.</span><span class="sxs-lookup"><span data-stu-id="f3626-224">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>

### <a name="add-a-file-attachment"></a><span data-ttu-id="f3626-225">Adicionar um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="f3626-225">Add a file attachment</span></span>

<span data-ttu-id="f3626-226">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de arquivo binário.</span><span class="sxs-lookup"><span data-stu-id="f3626-226">In the input HTML of your request's **Presentation** part, include `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="f3626-227">Basta enviar dados binários, não use Base64 ou codifique.</span><span class="sxs-lookup"><span data-stu-id="f3626-227">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image file attachment</title>
  </head>
  <body>
    <p>This is an image file attachment.</p>
    <object data-attachment="Logo.jpg" data="name:logo1-file" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```


<a name="file-binary-data-render-src"></a>

### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="f3626-228">Adicionar imagens de conteúdos de arquivo PDF</span><span class="sxs-lookup"><span data-stu-id="f3626-228">Add images of PDF file contents</span></span>

<span data-ttu-id="f3626-229">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<img data-render-src="name:part-name" ... />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de arquivo binário.</span><span class="sxs-lookup"><span data-stu-id="f3626-229">In the input HTML of your request's **Presentation** part, include `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="f3626-230">Basta enviar dados binários, não use Base64 ou codifique.</span><span class="sxs-lookup"><span data-stu-id="f3626-230">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with images of the pages of a PDF file</title>
  </head>
  <body>
    <p>The pages of this PDF file render as images.</p>
    <img data-render-src="name:file-part" alt="PDF file as images" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="file-part"
Content-Type: application/pdf

... binary file data ...

--MyAppPartBoundary--  
```


<a name="size-limits"></a>

## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="f3626-231">Limitações de tamanho para solicitações de páginas de POSTAGEM</span><span class="sxs-lookup"><span data-stu-id="f3626-231">Size limitations for POST pages requests</span></span>

<span data-ttu-id="f3626-232">Ao enviar a imagem e arquivo de dados, esteja ciente dessas limitações:</span><span class="sxs-lookup"><span data-stu-id="f3626-232">When sending image and file data, be aware of these limitations:</span></span> <!--TODO: check these-->

- <span data-ttu-id="f3626-233">A API REST do Microsoft Graph tem um limite de solicitação de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="f3626-233">The Microsoft Graph REST API has a 4 MB request limit.</span></span> <span data-ttu-id="f3626-234">Qualquer item maior que isso falhará com a mensagem de erro "solicitação muito grande (413)".</span><span class="sxs-lookup"><span data-stu-id="f3626-234">Anything above this will fail with the error message "request too large (413)".</span></span> 

- <span data-ttu-id="f3626-235">O limite de solicitação da subjacentes API REST do OneNote é maior, mas não pode ser acessada usando a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f3626-235">The request limit of the underlying OneNote REST API is higher, but you cannot access it via the Microsoft Graph API.</span></span> 
  - <span data-ttu-id="f3626-236">O limite de tamanho da POSTAGEM total é de aproximadamente 70 MB, incluindo imagens, arquivos e outros dados.</span><span class="sxs-lookup"><span data-stu-id="f3626-236">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="f3626-237">O limite real é afetado pela codificação downstream, portanto, não há um limite de número de bytes fixo.</span><span class="sxs-lookup"><span data-stu-id="f3626-237">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="f3626-238">As solicitações que excederem o limite podem gerar resultados não confiáveis.</span><span class="sxs-lookup"><span data-stu-id="f3626-238">Requests that exceed the limit might produce unreliable results.</span></span>
  - <span data-ttu-id="f3626-239">O limite de cada parte de dados é de 25 MB, incluindo os cabeçalhos das partes.</span><span class="sxs-lookup"><span data-stu-id="f3626-239">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="f3626-240">Partes de dados que excedem o limite são rejeitadas pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f3626-240">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="f3626-241">O número máximo de imagens por página é 150.</span><span class="sxs-lookup"><span data-stu-id="f3626-241">The maximum number of images per page is 150.</span></span> <span data-ttu-id="f3626-242">Ao usar o atributo `src="https://..."`, a API ignora rótulos **img** que ultrapassam o limite.</span><span class="sxs-lookup"><span data-stu-id="f3626-242">When using the `src="https://..."` attribute, the API ignores **img** tags beyond the limit.</span></span>

- <span data-ttu-id="f3626-243">O número máximo de partes de dados é 6 por POSTAGEM, incluindo a parte obrigatória **Apresentação**.</span><span class="sxs-lookup"><span data-stu-id="f3626-243">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="f3626-p129">Cada pedido pode conter até cinco elementos **img** que usam **data-render-src** um elemento **object** que usa **data-render-src**. Outras referências de imagem e arquivo são ignoradas.</span><span class="sxs-lookup"><span data-stu-id="f3626-p129">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="f3626-246">O número máximo de imagens em uma POSTAGEM única é 30, não importa qual o método usado para enviá-las para a API.</span><span class="sxs-lookup"><span data-stu-id="f3626-246">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="f3626-247">Imagens adicionais são ignoradas.</span><span class="sxs-lookup"><span data-stu-id="f3626-247">Additional images are ignored.</span></span> <span data-ttu-id="f3626-248">Se quiser capturar uma página da Web que contém muitas imagens, considere [capturar toda a página como um instantâneo](#add-a-webpage-snapshot).</span><span class="sxs-lookup"><span data-stu-id="f3626-248">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="f3626-249">Quando usar HTML ou data-render-src</span><span class="sxs-lookup"><span data-stu-id="f3626-249">When to use HTML versus data-render-src</span></span> 

<span data-ttu-id="f3626-250">Para decidir entre colocar HTML diretamente na página do OneNote em vez de usar o atributo **data-render-src**, considere o seguinte:</span><span class="sxs-lookup"><span data-stu-id="f3626-250">When trying to decide between putting HTML directly onto the OneNote page instead of using the **data-render-src** attribute, consider the following:</span></span>

- <span data-ttu-id="f3626-251">Provavelmente, a melhor maneira de enviar HTML complexo para o mecanismo de renderização é por meio de **data-render-src**, em vez de tentar modificar o HTML para caber naquilo que o Microsoft Graph aceita.</span><span class="sxs-lookup"><span data-stu-id="f3626-251">Complex HTML is probably best sent to the rendering engine via **data-render-src**, rather than attempting to modify the HTML to fit into what Microsoft Graph can accept.</span></span> <span data-ttu-id="f3626-252">Isso também ocorre quando o HTML inclui rótulos sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3626-252">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="f3626-253">Provavelmente, a melhor maneira de fazer a renderização de página com precisão para preservar o layout e a aparência da página é com o mecanismo de renderização por meio do **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="f3626-253">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="f3626-254">Geralmente, a melhor maneira de acrescentar texto diretamente editável é inserindo HTML diretamente na página.</span><span class="sxs-lookup"><span data-stu-id="f3626-254">Directly-editable text is often best done with inserting the HTML directly onto the page.</span></span> <span data-ttu-id="f3626-255">As imagens renderizadas são examinadas por um sistema de reconhecimento óptico de caracteres (OCR), mas não é a mesma coisa.</span><span class="sxs-lookup"><span data-stu-id="f3626-255">The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="f3626-256">Normalmente, a melhor maneira de fazer um instantâneo no tempo para fins de histórico ou arquivamento é com o método **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="f3626-256">Snapshot-in-time for historical or archival purposes is usually best done with the **data-render-src** method.</span></span>

- <span data-ttu-id="f3626-257">O **data-render-src** realmente se destaca pela funcionalidade de marcação do design da página da Web para revisões.</span><span class="sxs-lookup"><span data-stu-id="f3626-257">Marking-up a web page design for revisions is one place the **data-render-src** truly shines.</span></span> <span data-ttu-id="f3626-258">Com as funcionalidades de escrita à tinta do OneNote, é possível desenhar na imagem para indicar alterações ou destacar áreas importantes.</span><span class="sxs-lookup"><span data-stu-id="f3626-258">Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas.</span></span> <span data-ttu-id="f3626-259">Com a página da Web como uma imagem fica muito mais fácil.</span><span class="sxs-lookup"><span data-stu-id="f3626-259">Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="f3626-260">As imagens muito grandes ou as imagens nos formatos que o OneNote não aceita diretamente podem, às vezes, ser transformadas em miniaturas e convertidas com o atributo **data-render-src** mais facilmente do que se isso for feito em seu próprio código.</span><span class="sxs-lookup"><span data-stu-id="f3626-260">Very large images, or images in formats that OneNote doesn't directly accept, can sometimes be thumbnailed and converted with the **data-render-src** attribute more easily than by doing it in your own code.</span></span> <span data-ttu-id="f3626-261">Mesmo que a imagem também esteja disponível online, inserir os dados em sua POSTAGEM pode às vezes disponibilizar antes a página selecionada para os usuários do OneNote, reduzindo o número total de procedimentos necessários para criar a página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3626-261">Even if the image is also available online, embedding the data in your POST can sometimes make the captured page available to OneNote users sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="f3626-262">Às vezes, a melhor maneira para determinar qual método funciona melhor para os usuários é experimentar as duas formas conforme você desenvolve seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3626-262">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="f3626-263">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3626-263">Permissions</span></span>

<span data-ttu-id="f3626-264">Para criar ou atualizar páginas do OneNote, solicite permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="f3626-264">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="f3626-265">Escolha o nível mais baixo que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="f3626-265">Choose the lowest level that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="f3626-266">Permissões para páginas POST</span><span class="sxs-lookup"><span data-stu-id="f3626-266">Permissions for POST pages</span></span>

- <span data-ttu-id="f3626-267">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="f3626-267">Notes.Create</span></span>
- <span data-ttu-id="f3626-268">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3626-268">Notes.ReadWrite</span></span>
- <span data-ttu-id="f3626-269">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3626-269">Notes.ReadWrite.All</span></span> 

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="f3626-270">Permissões para páginas PATCH</span><span class="sxs-lookup"><span data-stu-id="f3626-270">Permissions for PATCH pages</span></span>

- <span data-ttu-id="f3626-271">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3626-271">Notes.ReadWrite</span></span>
- <span data-ttu-id="f3626-272">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3626-272">Notes.ReadWrite.All</span></span>

<span data-ttu-id="f3626-273">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="f3626-273">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="f3626-274">Confira também</span><span class="sxs-lookup"><span data-stu-id="f3626-274">See also</span></span>

- [<span data-ttu-id="f3626-275">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="f3626-275">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="f3626-276">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="f3626-276">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="f3626-277">Perguntas de desenvolvimento do OneNote no Microsoft Q&A</span><span class="sxs-lookup"><span data-stu-id="f3626-277">OneNote development questions on Microsoft Q&A</span></span>](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="f3626-278">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="f3626-278">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  
