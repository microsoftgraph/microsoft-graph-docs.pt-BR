
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="5e7d8-101">Adicionar imagens, vídeos e arquivos a páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="5e7d8-101">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="5e7d8-102">*__Aplica-se a:__ Bloco de anotações dos consumidores no OneDrive | Bloco de anotações empresariais no Office 365*</span><span class="sxs-lookup"><span data-stu-id="5e7d8-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="5e7d8-103">Você pode usar os elementos **img**, **object** e **iframe** para adicionar imagens, vídeos e arquivos à página do OneNote quando você [criar](onenote-create-page.md) ou [atualizar](onenote_update_page.md) a página.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-103">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote_update_page.md) the page.</span></span> 

- <span data-ttu-id="5e7d8-104">Use **img** para renderizar uma imagem na página.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-104">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="5e7d8-105">Use **iframe** para inserir um vídeo na página.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-105">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="5e7d8-106">Use **object** para adicionar um anexo de arquivo na página.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-106">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>
## <a name="adding-images"></a><span data-ttu-id="5e7d8-107">Adicionar imagens</span><span class="sxs-lookup"><span data-stu-id="5e7d8-107">Adding images</span></span>

<span data-ttu-id="5e7d8-108">Imagens podem ser adicionadas por referência de URL ou enviando dados brutos.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-108">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="5e7d8-109">Os seguintes métodos de adição de imagens, logotipos e fotos para páginas do OneNote são compatíveis com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-109">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="5e7d8-110">Adicionar uma imagem pública da Web</span><span class="sxs-lookup"><span data-stu-id="5e7d8-110">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)  
<span data-ttu-id="5e7d8-111">Use `img` com `src="http://image-url"` e especifique a URL de uma imagem acessível ao público.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-111">Use `img` with `src="http://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="5e7d8-112">Renderiza a imagem na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-112">Renders the image on the OneNote page.</span></span></p>
[<span data-ttu-id="5e7d8-113">Adicionar uma imagem usando dados binários</span><span class="sxs-lookup"><span data-stu-id="5e7d8-113">Add an image using binary data</span></span>](#add-an-image-using-binary-data)</p>
<span data-ttu-id="5e7d8-114">Use `img` com `src="name:image-block-name"` e envie o arquivo de imagem em uma parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-114">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="5e7d8-115">Renderiza a imagem na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-115">Renders the image on the OneNote page.</span></span></p>
[<span data-ttu-id="5e7d8-116">Adicionar um instantâneo de página da Web</span><span class="sxs-lookup"><span data-stu-id="5e7d8-116">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)</p>
<span data-ttu-id="5e7d8-117">Use `img` com `data-render-src="http://webpage-url"` e especifique a URL de uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-117">Use `img` with `data-render-src="http://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="5e7d8-118">Renderiza um instantâneo da página da Web inteira na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-118">Renders a snapshot of the whole webpage on the OneNote page.</span></span></p>
[<span data-ttu-id="5e7d8-119">Adicionar uma imagem renderizada de HTML</span><span class="sxs-lookup"><span data-stu-id="5e7d8-119">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)</p>
<span data-ttu-id="5e7d8-120">Use `img` com `data-render-src="name:html-block-name"` e envie HTML na parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-120">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="5e7d8-121">Renderiza o HTML como uma imagem na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-121">Renders the HTML as an image on the OneNote page.</span></span></p>
[<span data-ttu-id="5e7d8-122">Adicionar imagens de conteúdos de arquivo PDF</span><span class="sxs-lookup"><span data-stu-id="5e7d8-122">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)</p>
<span data-ttu-id="5e7d8-123">Use `<img data-render-src="name:part-name" />` e envie o arquivo PDF na parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-123">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="5e7d8-124">Renderiza cada página do PDF como uma imagem separada na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-124">Renders each PDF page as a separate image on the OneNote page.</span></span></p>
[<span data-ttu-id="5e7d8-125">Adicionar um arquivo de imagem como um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="5e7d8-125">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)</p>
<span data-ttu-id="5e7d8-126">Use `object` com `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` e envie um arquivo de imagem em uma parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-126">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="5e7d8-127">Adiciona um anexo de arquivo à página do OneNote e exibe um ícone de arquivo.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-127">Adds a file attachment to the OneNote page and displays a file icon.</span></span></p>

> <span data-ttu-id="5e7d8-128">**Observação:** para inserir imagens em uma página do OneNote, primeiro envie uma [solicitação GET para o conteúdo da página](onenote-get-content.md#page-html-content).</span><span class="sxs-lookup"><span data-stu-id="5e7d8-128">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="5e7d8-129">Isso retornará as URLs para recursos de imagem na página.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-129">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="5e7d8-130">Em seguida, separe as [solicitações GET dos recursos de imagem](onenote-get-content.md#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="5e7d8-130">Then you separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


<span data-ttu-id="5e7d8-131">**Atributos de imagem**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-131">**Image attributes**</span></span> 

<span data-ttu-id="5e7d8-132">Um elemento **img** pode incluir opcionalmente atributos **alt**, **height** e **width** e os atributos de estilo **max-width** e **max-height**.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-132">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

<span data-ttu-id="5e7d8-133">**Tipos de mídia de imagem**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-133">**Image media types**</span></span>

<span data-ttu-id="5e7d8-134">O Microsoft Graph é compatível com os tipos de imagem TIFF, PNG, GIF, JPEG e BMP.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-134">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="5e7d8-135">Para capturar uma imagem que usa um formato diferente que você não quer converter, [envie dados binários](#add-an-image-using-binary-data) em uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-135">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="5e7d8-136">Não é necessário usar Base64 ou codificar os dados binários que você enviar.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-136">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="5e7d8-137">**Observação:** a API detecta o tipo de imagem de entrada e o retorna como o atributo **data-fullres-src-type** no [HTML de saída](onenote_input_output_html.md#output-html).</span><span class="sxs-lookup"><span data-stu-id="5e7d8-137">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="5e7d8-138">A API também retorna o tipo de imagem da imagem otimizada em **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-138">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="5e7d8-139">Ver [limitações](#size-limitations-for-post-pages-requests) que se aplicam ao criar páginas que contém mídia.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-139">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>
### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="5e7d8-140">Adicionar uma imagem pública da Web</span><span class="sxs-lookup"><span data-stu-id="5e7d8-140">Add a public image from the web</span></span>

<span data-ttu-id="5e7d8-141">No HTML de entrada da sua solicitação, inclua `<img src="http://..." />` e especifique a URL de uma imagem publicamente acessível para o atributo **src**.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-141">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

```
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
    <img src="http://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>
### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="5e7d8-142">Adicionar uma imagem usando dados binários</span><span class="sxs-lookup"><span data-stu-id="5e7d8-142">Add an image using binary data</span></span>

<span data-ttu-id="5e7d8-143">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<img src="name:part-name" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de imagem binária.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-143">In the input HTML of your request's **Presentation** part, include  `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="5e7d8-144">Basta enviar dados binários, não use Base64 ou codifique.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-144">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```
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
### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="5e7d8-145">Adicionar um instantâneo de página da Web</span><span class="sxs-lookup"><span data-stu-id="5e7d8-145">Add a webpage snapshot</span></span>

<span data-ttu-id="5e7d8-146">Você pode usar o Microsoft Graph para fazer instantâneos inteiros de páginas da Web e inseri-los em novas páginas.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-146">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="5e7d8-147">Esse método é útil para arquivar páginas da Web ou capturar páginas da Web complexas que possuem recursos não compatíveis com o OneNote (como algumas CSS).</span><span class="sxs-lookup"><span data-stu-id="5e7d8-147">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="5e7d8-148">No HTML de entrada da sua solicitação, inclua `<img src="http://..." />` e especifique a URL de uma página da Web que você quer inserir para o atributo **src**.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-148">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

```
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
    <img data-render-src="http://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>
### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="5e7d8-149">Adicionar uma imagem renderizada de HTML</span><span class="sxs-lookup"><span data-stu-id="5e7d8-149">Add an image rendered from HTML</span></span>
<span data-ttu-id="5e7d8-150">Quando você passar o HTML como um bloco de dados, certifique-se de que não haja conteúdo ativo que exija credenciais de usuário ou um plug-in de navegador pré-carregado.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-150">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="5e7d8-151">O mecanismo que o Microsoft Graph usa para renderizar a página HTML em uma imagem não tem a capacidade de efetuar login de um usuário e não inclui plug-ins como Adobe Flash, Apple QuickTime entre outros.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-151">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so-on.</span></span> <span data-ttu-id="5e7d8-152">Isto também significa que o conteúdo carregado dinamicamente, como pode ser com um script AJAX, não será exibido se a obtenção dos dados exigir credenciais de logon do usuário ou cookies.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-152">That also means that dynamically-loaded content, like might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="5e7d8-153">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<img data-render-src="name:part-name" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém o HTML.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-153">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>

```
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
<img src="http://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>
### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="5e7d8-154">Adicionar um arquivo de imagem como um anexo</span><span class="sxs-lookup"><span data-stu-id="5e7d8-154">Add an image file as an attachment</span></span>

<span data-ttu-id="5e7d8-155">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de imagem binária.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-155">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="5e7d8-156">Basta enviar dados binários, não use Base64 ou codifique.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-156">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```
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

<span data-ttu-id="5e7d8-157">Saiba mais sobre [tipos de mídia de arquivos](#file-media-types).</span><span class="sxs-lookup"><span data-stu-id="5e7d8-157">Learn more about [file media types](#file-media-types).</span></span>



<a name="videos"></a>
## <a name="adding-videos"></a><span data-ttu-id="5e7d8-158">Adicionar vídeos</span><span class="sxs-lookup"><span data-stu-id="5e7d8-158">Adding videos</span></span>

<span data-ttu-id="5e7d8-159">Você pode inserir vídeos em páginas do OneNote usando `<iframe data-original-src="http://..." />` no HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-159">You can embed videos in OneNote pages using `<iframe data-original-src="http://..." />` in the input HTML.</span></span> 

<span data-ttu-id="5e7d8-160">**Sites de vídeo compatíveis**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-160">**Supported video sites**</span></span>

- <span data-ttu-id="5e7d8-161">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="5e7d8-161">Dailymotion</span></span>
- <span data-ttu-id="5e7d8-162">Office Mix</span><span class="sxs-lookup"><span data-stu-id="5e7d8-162">Office Mix</span></span>
- <span data-ttu-id="5e7d8-163">Sway</span><span class="sxs-lookup"><span data-stu-id="5e7d8-163">Sway</span></span>
- <span data-ttu-id="5e7d8-164">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="5e7d8-164">Sketchfab</span></span>
- <span data-ttu-id="5e7d8-165">TED</span><span class="sxs-lookup"><span data-stu-id="5e7d8-165">TED</span></span>
- <span data-ttu-id="5e7d8-166">YouTube</span><span class="sxs-lookup"><span data-stu-id="5e7d8-166">YouTube</span></span>
- <span data-ttu-id="5e7d8-167">Vimeo</span><span class="sxs-lookup"><span data-stu-id="5e7d8-167">Vimeo</span></span>
- <span data-ttu-id="5e7d8-168">Vine</span><span class="sxs-lookup"><span data-stu-id="5e7d8-168">Vine</span></span>

<span data-ttu-id="5e7d8-169">**atributos de iframe**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-169">**iframe attributes**</span></span>

<span data-ttu-id="5e7d8-170">**data-original-src**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-170">**data-original-src**</span></span></p>
<span data-ttu-id="5e7d8-171">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-171">Required.</span></span> <span data-ttu-id="5e7d8-172">A URL do vídeo.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-172">The URL of the video source.</span></span><br /><span data-ttu-id="5e7d8-173">Exemplo: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="5e7d8-173">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span></p>
<span data-ttu-id="5e7d8-174">**width**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-174">**width**</span></span></p>
<span data-ttu-id="5e7d8-175">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-175">Optional.</span></span> <span data-ttu-id="5e7d8-176">A largura do iframe que contém o vídeo.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-176">The width of the iframe that contains the video.</span></span> <span data-ttu-id="5e7d8-177">O padrão é 480.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-177">Default is 480.</span></span><br /><span data-ttu-id="5e7d8-178">Exemplo: `width="300"`</span><span class="sxs-lookup"><span data-stu-id="5e7d8-178">Example: `width="300"`</span></span></p>
<span data-ttu-id="5e7d8-179">**height**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-179">**height**</span></span></p>
<span data-ttu-id="5e7d8-180">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-180">Optional.</span></span> <span data-ttu-id="5e7d8-181">A altura do iframe que contém o vídeo.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-181">The height of the iframe that contains the video.</span></span> <span data-ttu-id="5e7d8-182">O padrão é 360.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-182">Default is 360.</span></span><br /><span data-ttu-id="5e7d8-183">Exemplo: `height="300"`</span><span class="sxs-lookup"><span data-stu-id="5e7d8-183">Example: `height="300"`</span></span></p>

<span data-ttu-id="5e7d8-184">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-184">**Example**</span></span>

<span data-ttu-id="5e7d8-185">No HTML de entrada da sua solicitação, inclua `<iframe data-original-src="http://..." />` e especifique a URL do vídeo para o atributo **data-original-src**.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-185">In the input HTML of your request, include `<iframe data-original-src="http://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

```
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


<a name="files"></a>
## <a name="adding-files"></a><span data-ttu-id="5e7d8-186">Adicionar arquivos</span><span class="sxs-lookup"><span data-stu-id="5e7d8-186">Adding files</span></span>

<span data-ttu-id="5e7d8-187">Você pode adicionar anexos de arquivo a páginas do OneNote usando um elemento **object** de HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-187">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="5e7d8-188">Se você estiver adicionando um arquivo PDF, você pode usar um elemento de **img** para renderizar as páginas de PDF como imagens.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-188">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="5e7d8-189">Adicionar um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="5e7d8-189">Add a file attachment</span></span>](#add-a-file-attachment)</p>
<span data-ttu-id="5e7d8-190">Use `<object .../>` e envie o arquivo na parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-190">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="5e7d8-191">Adiciona um anexo de arquivo que exibe um ícone de arquivo na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-191">Adds a file attachment that displays a file icon on the OneNote page.</span></span></p>
[<span data-ttu-id="5e7d8-192">Adicionar imagens de conteúdos de arquivo PDF</span><span class="sxs-lookup"><span data-stu-id="5e7d8-192">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)</p>
<span data-ttu-id="5e7d8-193">Use `<img data-render-src="name:part-name" />` e envie um arquivo PDF na parte de dados de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-193">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="5e7d8-194">Renderiza cada página do PDF como uma imagem separada na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-194">Renders each PDF page as a separate image on the OneNote page.</span></span></p>

<span data-ttu-id="5e7d8-195">**Atributos de arquivo**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-195">**File attributes**</span></span>

<span data-ttu-id="5e7d8-196">O elemento **object** requer os seguintes atributos.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-196">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="5e7d8-197">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-197">**data-attachment**</span></span></p>
<span data-ttu-id="5e7d8-198">O nome e a extensão do arquivo para exibir na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-198">The file name and extension to display on the OneNote page.</span></span><br /><span data-ttu-id="5e7d8-199">Exemplo: `data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="5e7d8-199">Example: `data-attachment="filename.docx"`</span></span></p>
<span data-ttu-id="5e7d8-200">**data**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-200">**Data**</span></span></p>
<span data-ttu-id="5e7d8-201">O nome da parte do corpo na solicitação de várias partes que contém os dados de arquivo binário.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-201">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="5e7d8-202">O Microsoft Graph não é compatível com a passagem de uma referência de URL aqui.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-202">Microsoft Graph does not support passing a URL reference here.</span></span><br /><span data-ttu-id="5e7d8-203">Exemplo: `data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="5e7d8-203">Example: `data="name:part-name"`</span></span></p>
<span data-ttu-id="5e7d8-204">**type**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-204">**type**</span></span></p>
<span data-ttu-id="5e7d8-205">O tipo de mídia de arquivo, usado para determinar o ícone de arquivo a ser usado na página e qual aplicativo é iniciado quando o usuário ativa o arquivo no dispositivo a partir do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-205">The file media type, used to determine the file icon to use on the page, and which application starts when the user activates the file on the device from OneNote.</span></span><br /><span data-ttu-id="5e7d8-206">Exemplo: `type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="5e7d8-206">Example: `type="application/pdf"`</span></span></p>


<a name="file-media-types"></a>

### <a name="file-media-types"></a><span data-ttu-id="5e7d8-207">Tipos de mídia de arquivo</span><span class="sxs-lookup"><span data-stu-id="5e7d8-207">File media types</span></span>  
<span data-ttu-id="5e7d8-208">O Microsoft Graph usa o ícone de tipos de arquivo predefinido para arquivos anexos ou um ícone genérico quando a API não reconhece o tipo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-208">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="5e7d8-209">A tabela a seguir mostra alguns tipos de arquivos comuns reconhecidos pela API.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-209">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="5e7d8-210">application/pdf</span><span class="sxs-lookup"><span data-stu-id="5e7d8-210">application/pdf</span></span>  
- <span data-ttu-id="5e7d8-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="5e7d8-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="5e7d8-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="5e7d8-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="5e7d8-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="5e7d8-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="5e7d8-214">image/png</span><span class="sxs-lookup"><span data-stu-id="5e7d8-214">image/png</span></span>
- <span data-ttu-id="5e7d8-215">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="5e7d8-215">image/jpeg. Required.</span></span>
- <span data-ttu-id="5e7d8-216">image/gif</span><span class="sxs-lookup"><span data-stu-id="5e7d8-216">image/gif</span></span>
- <span data-ttu-id="5e7d8-217">audio/wav</span><span class="sxs-lookup"><span data-stu-id="5e7d8-217">audio/wav</span></span>
- <span data-ttu-id="5e7d8-218">video/mp4</span><span class="sxs-lookup"><span data-stu-id="5e7d8-218">video/mp4</span></span>
- <span data-ttu-id="5e7d8-219">application/msword</span><span class="sxs-lookup"><span data-stu-id="5e7d8-219">application/msword</span></span>
- <span data-ttu-id="5e7d8-220">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="5e7d8-220">application/mspowerpoint</span></span>
- <span data-ttu-id="5e7d8-221">application/excel</span><span class="sxs-lookup"><span data-stu-id="5e7d8-221">application/excel</span></span>

<span data-ttu-id="5e7d8-222">Ver [limitações](#size-limitations-for-post-pages-requests) que se aplicam ao criar páginas que contém mídia.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-222">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>
### <a name="add-a-file-attachment"></a><span data-ttu-id="5e7d8-223">Adicionar um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="5e7d8-223">Add a file attachment</span></span>

<span data-ttu-id="5e7d8-224">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de arquivo binário.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-224">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="5e7d8-225">Basta enviar dados binários, não use Base64 ou codifique.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-225">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```
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
### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="5e7d8-226">Adicionar imagens de conteúdos de arquivo PDF</span><span class="sxs-lookup"><span data-stu-id="5e7d8-226">Add images of PDF file contents</span></span>

<span data-ttu-id="5e7d8-227">No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<img data-render-src="name:part-name" ... />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de arquivo binário.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-227">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="5e7d8-228">Basta enviar dados binários, não use Base64 ou codifique.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-228">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```
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
## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="5e7d8-229">Limitações de tamanho para solicitações de páginas de POSTAGEM</span><span class="sxs-lookup"><span data-stu-id="5e7d8-229">Size limitations for POST pages requests</span></span>

<span data-ttu-id="5e7d8-230">Ao enviar imagem e arquivo de dados, esteja ciente destas limitações: <!--TODO: check these--></span><span class="sxs-lookup"><span data-stu-id="5e7d8-230">When sending image and file data, be aware of these limitations: <!--TODO: check these--></span></span>

- <span data-ttu-id="5e7d8-231">O limite de tamanho da POSTAGEM total é de aproximadamente 70 MB, incluindo imagens, arquivos e outros dados.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-231">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="5e7d8-232">O limite real é afetado pela codificação downstream, portanto, não há um limite de número de bytes fixo.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-232">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="5e7d8-233">As solicitações que excederem o limite podem produzir resultados não confiáveis.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-233">Requests that exceed the limit may produce unreliable results.</span></span>

- <span data-ttu-id="5e7d8-234">O limite de cada parte de dados é de 25 MB, incluindo os cabeçalhos das partes.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-234">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="5e7d8-235">Partes de dados que excedem o limite são rejeitadas pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-235">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="5e7d8-236">O número máximo de imagens por página é 150.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-236">The maximum number of images per page is 150.</span></span> <span data-ttu-id="5e7d8-237">Ao usar o atributo `src="http://..."`, a API ignora rótulos **img** que ultrapassam o limite.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-237">When using the `src="http://..."` attribute, the API ignores **img** tags beyond the limit.</span></span>

- <span data-ttu-id="5e7d8-238">O número máximo de partes de dados é 6 por POSTAGEM, incluindo a parte obrigatória **Apresentação**.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-238">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="5e7d8-239">Cada pedido pode conter até cinco elementos **img** que usam **data-render-src** um elemento **object** que usa **data-render-src**. Outras referências de imagem e arquivo são ignoradas.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-239">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="5e7d8-240">O número máximo de imagens em uma POSTAGEM única é 30, não importa qual o método usado para enviá-las para a API.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-240">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="5e7d8-241">Imagens adicionais são ignoradas.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-241">Additional images are ignored.</span></span> <span data-ttu-id="5e7d8-242">Se quiser capturar uma página da Web que contém muitas imagens, considere [capturar toda a página como um instantâneo](#add-a-webpage-snapshot).</span><span class="sxs-lookup"><span data-stu-id="5e7d8-242">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="5e7d8-243">Quando usar HTML ou *data-render-src*</span><span class="sxs-lookup"><span data-stu-id="5e7d8-243">When to use HTML versus *data-render-src*</span></span> 
<span data-ttu-id="5e7d8-244">Para decidir entre colocar HTML diretamente na página do OneNote em vez de usar o atributo **data-render-src**, considere o seguinte:</span><span class="sxs-lookup"><span data-stu-id="5e7d8-244">When trying to decide between putting HTML directly onto the OneNote page instead of using the **data-render-src** attribute, consider the following:</span></span>

- <span data-ttu-id="5e7d8-245">Provavelmente, a melhor maneira de enviar HTML complexo para o mecanismo de renderização é por meio de **data-render-src**, em vez de tentar modificar o HTML para caber naquilo que o Microsoft Graph aceita.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-245">Complex HTML is probably best sent to the rendering engine via **data-render-src**, rather than attempting to modify the HTML to fit into what Microsoft Graph can accept.</span></span> <span data-ttu-id="5e7d8-246">Isso também ocorre quando o HTML inclui rótulos sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-246">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="5e7d8-247">Provavelmente, a melhor maneira de fazer a renderização de página com precisão para preservar o layout e a aparência da página é com o mecanismo de renderização por meio do **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-247">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="5e7d8-248">Geralmente, a melhor maneira de acrescentar texto diretamente editável é inserindo HTML diretamente na página.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-248">Directly-editable text is often best done with inserting the HTML directly onto the page.</span></span> <span data-ttu-id="5e7d8-249">As imagens renderizadas são examinadas por um sistema de reconhecimento óptico de caracteres (OCR), mas não é a mesma coisa.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-249">The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="5e7d8-250">Normalmente, a melhor maneira de fazer um instantâneo no tempo para fins de histórico ou arquivamento é com o método data-render-src.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-250">Snapshot-in-time for historical or archival purposes is usually best done with the data-render-src method.</span></span>

- <span data-ttu-id="5e7d8-251">O **data-render-src ** realmente se destaca pela funcionalidade de marcação do design da página da Web para revisões.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-251">Marking-up a web page design for revisions is one place the **data-render-src** truly shines.</span></span> <span data-ttu-id="5e7d8-252">Com as funcionalidades de escrita à tinta do OneNote, é possível desenhar na imagem para indicar alterações ou destacar áreas importantes.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-252">Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas.</span></span> <span data-ttu-id="5e7d8-253">Com a página da Web como uma imagem fica muito mais fácil.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-253">Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="5e7d8-254">As imagens muito grandes ou as imagens nos formatos que o OneNote não aceita diretamente podem, às vezes, ser transformadas em miniaturas e convertidas com o atributo **data-render-src** mais facilmente do que fazer em seu próprio código.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-254">Very large images, or images in formats that OneNote doesn't directly accept can sometimes be thumbnailed and converted with the **data-render-src** attribure more easily than by doing it in your own code.</span></span> <span data-ttu-id="5e7d8-255">Mesmo que a imagem também esteja disponível online, inserir os dados em sua POSTAGEM pode às vezes disponibilizar antes a página selecionada para o usuário do OneNote, reduzindo o número total de idas e vindas necessárias para criar a página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-255">Even if the image is also available onlinet, embedding the data in your POST can sometimes make the captured page available to OneNote user sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="5e7d8-256">Às vezes, a melhor maneira para determinar qual método funciona melhor para os usuários é experimentar as duas formas conforme você desenvolve seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-256">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="5e7d8-257">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e7d8-257">Permissions</span></span>

<span data-ttu-id="5e7d8-258">Para criar ou atualizar páginas do OneNote, solicite permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-258">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="5e7d8-259">Escolha o nível mais baixo que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="5e7d8-259">Choose the lowest level that your app needs to do its work.</span></span>

<span data-ttu-id="5e7d8-260">**Permissões para _páginas POST_**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-260">**Permissions for _POST pages_**</span></span>

- <span data-ttu-id="5e7d8-261">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="5e7d8-261">Notes.Create</span></span>
- <span data-ttu-id="5e7d8-262">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e7d8-262">Notes.ReadWrite</span></span>
- <span data-ttu-id="5e7d8-263">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e7d8-263">Notes.ReadWrite.All</span></span> 

<span data-ttu-id="5e7d8-264">**Permissões para _páginas PATCH_**</span><span class="sxs-lookup"><span data-stu-id="5e7d8-264">**Permissions for _PATCH pages_**</span></span>

- <span data-ttu-id="5e7d8-265">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e7d8-265">Notes.ReadWrite</span></span>
- <span data-ttu-id="5e7d8-266">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e7d8-266">Notes.ReadWrite.All</span></span>

<span data-ttu-id="5e7d8-267">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="5e7d8-267">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="5e7d8-268">Recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="5e7d8-268">Additional resources</span></span>

- [<span data-ttu-id="5e7d8-269">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="5e7d8-269">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="5e7d8-270">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="5e7d8-270">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="5e7d8-271">Perguntas sobre desenvolvimento do OneNote no Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="5e7d8-271">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="5e7d8-272">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="5e7d8-272">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
