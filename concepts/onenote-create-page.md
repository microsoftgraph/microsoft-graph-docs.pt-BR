# <a name="create-onenote-pages"></a><span data-ttu-id="c41c8-101">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="c41c8-101">Create OneNote pages</span></span>

<span data-ttu-id="c41c8-102">**Aplica-se a**: Blocos de anotações de consumidor no OneDrive | Blocos de anotações empresariais no Office 365</span><span class="sxs-lookup"><span data-stu-id="c41c8-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="c41c8-103">Para criar uma página do OneNote, você envia uma solicitação POST para um ponto de extremidade de *pages*.</span><span class="sxs-lookup"><span data-stu-id="c41c8-103">To create a OneNote page, you send a POST request to a *pages* endpoint.</span></span> <span data-ttu-id="c41c8-104">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="c41c8-104">For example:</span></span>

`POST ../notes/sections/{id}/pages`

<br/>

<span data-ttu-id="c41c8-105">Envie o HTML que define a página no corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c41c8-105">Send the HTML that defines the page in the message body.</span></span> <span data-ttu-id="c41c8-106">Se a solicitação for bem-sucedida, o Microsoft Graph retornará um código de status de HTTP 201.</span><span class="sxs-lookup"><span data-stu-id="c41c8-106">If the request is successful, Microsoft Graph returns a 201 HTTP status code.</span></span>


> <span data-ttu-id="c41c8-107">**Observação:** para saber mais sobre as solicitações POST que você pode enviar para criar seções, grupos de seções e blocos de anotações, consulte a nossa [referência interativa do REST](http://dev.onenote.com/docs).</span><span class="sxs-lookup"><span data-stu-id="c41c8-107">**Note:** To learn about the POST requests you can send to create sections, section groups, and notebooks, see our [interactive REST reference](http://dev.onenote.com/docs).</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="c41c8-108">Construir a URI de solicitação</span><span class="sxs-lookup"><span data-stu-id="c41c8-108">Construct the request URI</span></span>

<span data-ttu-id="c41c8-109">Para construir a URI de solicitação POST, comece com a URL raiz do serviço:</span><span class="sxs-lookup"><span data-stu-id="c41c8-109">To construct the POST request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="c41c8-110">Depois acrescente o ponto de extremidade de *pages*:</span><span class="sxs-lookup"><span data-stu-id="c41c8-110">Then append the *pages* endpoint:</span></span>

- <span data-ttu-id="c41c8-111">**Criar uma página em qualquer seção (especificada pelo nome da seção)**</span><span class="sxs-lookup"><span data-stu-id="c41c8-111">**Create a page in any section (specified by section name)**</span></span><br/><br/>`.../pages?sectionName=DefaultSection`

- <span data-ttu-id="c41c8-112">**Criar uma página em qualquer seção (especificada pela ID)**</span><span class="sxs-lookup"><span data-stu-id="c41c8-112">**Create a page in any section (specified by ID)**</span></span><br/><br/>`.../sections/{section-id}/pages` 

<span data-ttu-id="c41c8-113">Se você estiver criando páginas no bloco de anotações pessoal do usuário, o Microsoft Graph também fornecerá pontos de extremidade que você pode usar para criar páginas no bloco de anotações padrão:</span><span class="sxs-lookup"><span data-stu-id="c41c8-113">If you're creating pages in the user's personal notebook, Microsoft Graph also provides endpoints you can use to create pages in the default notebook:</span></span>

- <span data-ttu-id="c41c8-114">**Criar uma página na seção padrão do bloco de anotações padrão**</span><span class="sxs-lookup"><span data-stu-id="c41c8-114">**Create a page in the default section of the default notebook**</span></span><br/><br/>`../pages` 



<span data-ttu-id="c41c8-115">Sua URI de solicitação completa parecerá com um dos seguintes exemplos:</span><span class="sxs-lookup"><span data-stu-id="c41c8-115">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

<span data-ttu-id="c41c8-116">Saiba mais sobre a [URL raiz de serviço](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="c41c8-116">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a><span data-ttu-id="c41c8-117">Usar o parâmetro de URL *sectionName*</span><span class="sxs-lookup"><span data-stu-id="c41c8-117">Using the *sectionName* URL parameter</span></span>

<span data-ttu-id="c41c8-118">As seguintes regras aplicam-se ao usar o parâmetro *sectionName* para a criação de uma página em uma seção nomeada no bloco de anotações padrão:</span><span class="sxs-lookup"><span data-stu-id="c41c8-118">The following rules apply when using the *sectionName* parameter to create a page in a named section in the default notebook:</span></span>

- <span data-ttu-id="c41c8-119">Apenas seções de nível superior podem ser referenciadas (não as seções nos grupos de seções).</span><span class="sxs-lookup"><span data-stu-id="c41c8-119">Only top-level sections can be referenced (not sections within section groups).</span></span>

- <span data-ttu-id="c41c8-120">Se não houver uma seção com o nome especificado no bloco de anotações padrão, a API a criará.</span><span class="sxs-lookup"><span data-stu-id="c41c8-120">If a section with the specified name doesn't exist in the default notebook, the API creates it.</span></span> <span data-ttu-id="c41c8-121">Os seguintes caracteres não são permitidos nos nomes de seção: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="c41c8-121">These characters are not allowed for section names: ?`? * \ / : < > | & # " % ~`</span></span>

- <span data-ttu-id="c41c8-122">Os nomes das seções não diferenciam letras maiúsculas de minúsculas para correspondência, mas a diferença entre maiúsculas e minúsculas é preservada ao criar seções.</span><span class="sxs-lookup"><span data-stu-id="c41c8-122">Section names are case-insensitive for matching, but case is preserved when sections are created.</span></span> <span data-ttu-id="c41c8-123">Portanto, "Minha Nova Seção" será exibida assim, mas também seria feita a correspondência de "minha nova seção" nas postagens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="c41c8-123">So "My New Section" will display like that, but "my new section" would also match on subsequent posts.</span></span>

- <span data-ttu-id="c41c8-124">Os nomes das seções devem ser codificados por URL.</span><span class="sxs-lookup"><span data-stu-id="c41c8-124">Section names must be URL-encoded.</span></span> <span data-ttu-id="c41c8-125">Por exemplo, os espaços devem ser codificados como *20%*.</span><span class="sxs-lookup"><span data-stu-id="c41c8-125">For example, spaces must be encoded as *%20*.</span></span>

- <span data-ttu-id="c41c8-126">O parâmetro *sectionName* só é válido com a rota `../notes/pages` (não com `../notes/sections/{id}/pages`).</span><span class="sxs-lookup"><span data-stu-id="c41c8-126">The *sectionName* parameter is valid only with the `../notes/pages` route (not `../notes/sections/{id}/pages`).</span></span>

<span data-ttu-id="c41c8-127">Como serão criadas seções caso não existam, é seguro usar essa chamada com todas as páginas que o seu aplicativo criar.</span><span class="sxs-lookup"><span data-stu-id="c41c8-127">Because sections are created if they don't exist, it's safe to use this call with every page your app creates.</span></span> <span data-ttu-id="c41c8-128">Os usuários podem renomear as seções, mas a API criará uma nova seção com o nome da seção que você fornecer.</span><span class="sxs-lookup"><span data-stu-id="c41c8-128">Users might rename sections, but the API will create a new section with the section name that you supply.</span></span> 

> <span data-ttu-id="c41c8-129">**Observação:** os links retornados pela API para as páginas de uma seção renomeada ainda abrirão essas páginas antigas.</span><span class="sxs-lookup"><span data-stu-id="c41c8-129">**Note:** The links returned by the API for pages in a renamed section will still reach those older pages.</span></span> 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="c41c8-130">Criar o corpo da mensagem</span><span class="sxs-lookup"><span data-stu-id="c41c8-130">Construct the message body</span></span>

<span data-ttu-id="c41c8-131">O HTML que define o conteúdo da página se chama *HTML de entrada*.</span><span class="sxs-lookup"><span data-stu-id="c41c8-131">The HTML that defines page content is called *input HTML*.</span></span> <span data-ttu-id="c41c8-132">O HTML de entrada é compatível com um [subconjunto de HTML e CSS padrão](#supported-html-and-css-for-onenote-pages), com a adição de atributos personalizados.</span><span class="sxs-lookup"><span data-stu-id="c41c8-132">Input HTML supports a [subset of standard HTML and CSS](#supported-html-and-css-for-onenote-pages), with the addition of custom attributes.</span></span> <span data-ttu-id="c41c8-133">(Os atributos personalizados, como **data-id** e **data-render-src**, são descritos em [HTML de entrada e de saída](onenote_input_output_html.md).)</span><span class="sxs-lookup"><span data-stu-id="c41c8-133">(Custom attributes, like **data-id** and **data-render-src**, are described in [Input and output HTML](onenote_input_output_html.md).)</span></span> 

<span data-ttu-id="c41c8-134">Envie o HTML de entrada no corpo da mensagem da solicitação POST.</span><span class="sxs-lookup"><span data-stu-id="c41c8-134">Send the input HTML in the message body of the POST request.</span></span> <span data-ttu-id="c41c8-135">Você pode enviar o HTML de entrada diretamente no corpo da mensagem usando o tipo de conteúdo `application/xhtml+xml` ou `text/html`, ou pode enviá-lo na parte "Apresentação" de uma solicitação de diversas partes.</span><span class="sxs-lookup"><span data-stu-id="c41c8-135">You can send the input HTML directly in the message body using the  `application/xhtml+xml` or `text/html` content type, or you can send it in the "Presentation" part of a multipart request.</span></span> 

<span data-ttu-id="c41c8-136">O exemplo a seguir envia o HTML de entrada diretamente no corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c41c8-136">The following example sends the input HTML directly in the message body.</span></span>

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: application/xhtml+xml

<!DOCTYPE html>
<html>
  <head>
    <title>A page with a block of HTML</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>This page contains some <i>formatted</i> <b>text</b> and an image.</p>
    <img src="http://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<br/>

<span data-ttu-id="c41c8-137">Se você estiver enviando dados binários, use uma [solicitação de diversas partes](#example-request).</span><span class="sxs-lookup"><span data-stu-id="c41c8-137">If you're sending binary data, you must use a [multipart request](#example-request).</span></span> 

> <span data-ttu-id="c41c8-138">**Observação:** para simplificar a programação e a consistência em seu aplicativo, use as solicitações de diversas partes para criar todas as páginas.</span><span class="sxs-lookup"><span data-stu-id="c41c8-138">To simplify programming and consistency in your app, you can use multipart requests to create all pages.</span></span> <span data-ttu-id="c41c8-139">É uma boa ideia usar uma biblioteca para criar mensagens de diversas partes.</span><span class="sxs-lookup"><span data-stu-id="c41c8-139">It's a good idea to use a library to construct multipart messages.</span></span> <span data-ttu-id="c41c8-140">Isso reduz o risco da criação de cargas mal formadas.</span><span class="sxs-lookup"><span data-stu-id="c41c8-140">This reduces the risk of creating malformed payloads.</span></span>


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a><span data-ttu-id="c41c8-141">Requisitos e limitações para HTML de entrada em solicitações de páginas POST</span><span class="sxs-lookup"><span data-stu-id="c41c8-141">Requirements and limitations for input HTML in POST pages requests</span></span>

<span data-ttu-id="c41c8-142">Ao enviar HTML de entrada, lembre-se desses requisitos e limitações gerais:</span><span class="sxs-lookup"><span data-stu-id="c41c8-142">When sending input HTML, be aware of these general requirements and limitations:</span></span>  

- <span data-ttu-id="c41c8-143">O HTML de entrada deve ser codificado em UTF-8 e Extensible HTML bem elaborado.</span><span class="sxs-lookup"><span data-stu-id="c41c8-143">Input HTML should be UTF-8 encoded and well-formed XHTML.</span></span> <span data-ttu-id="c41c8-144">Todas as marcas de início do contêiner exigem marcas de fechamento correspondentes.</span><span class="sxs-lookup"><span data-stu-id="c41c8-144">All container start tags require matching closing tags.</span></span> <span data-ttu-id="c41c8-145">Todos os valores do atributo devem estar entre aspas simples ou duplas.</span><span class="sxs-lookup"><span data-stu-id="c41c8-145">All attribute values must be surrounded by double- or single-quote marks.</span></span>  <!--docs say MUST be encoded-->

- <span data-ttu-id="c41c8-146">O código JavaScript, os arquivos inclusos e CSS são removidos.</span><span class="sxs-lookup"><span data-stu-id="c41c8-146">JavaScript code, included files, and CSS are removed.</span></span> 

- <span data-ttu-id="c41c8-147">Os formulários HTML são removidos totalmente.</span><span class="sxs-lookup"><span data-stu-id="c41c8-147">HTML forms are removed in their entirety.</span></span>  

- <span data-ttu-id="c41c8-148">O Microsoft Graph é compatível com um [subconjunto de elementos HTML](#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="c41c8-148">Microsoft Graph supports a [subset of HTML elements](#supported-html-and-css-for-onenote-pages).</span></span> 

- <span data-ttu-id="c41c8-149">O Microsoft Graph é compatível com um subconjunto de atributos HTML comuns e um conjunto de atributos personalizados, como o atributo **data-id** usado para atualizar as páginas.</span><span class="sxs-lookup"><span data-stu-id="c41c8-149">Microsoft Graph supports a subset of common HTML attributes and a set of custom attributes, such as the **data-id** attribute used for updating pages.</span></span> <span data-ttu-id="c41c8-150">Confira os atributos compatíveis em [HTML de entrada e de saída](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="c41c8-150">For supported attributes, see [Input and output HTML](onenote_input_output_html.md).</span></span>


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a><span data-ttu-id="c41c8-151">HTML e CSS compatíveis com páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="c41c8-151">Supported HTML and CSS for OneNote pages</span></span>

<span data-ttu-id="c41c8-152">Nem todos os elementos, atributos e propriedades são compatíveis (em HTML4, Extensible HTML, CSS, HTML5 etc.).</span><span class="sxs-lookup"><span data-stu-id="c41c8-152">Not all elements, attributes, and properties are supported (in HTML4, XHTML, CSS, HTML5, etc.).</span></span> <span data-ttu-id="c41c8-153">Em vez disso, o Microsoft Graph aceita um conjunto limitado de HTML mais adequado à forma como as pessoas usam o OneNote.</span><span class="sxs-lookup"><span data-stu-id="c41c8-153">Instead, Microsoft Graph accepts a limited set of HTML that better fits how people use OneNote.</span></span> <span data-ttu-id="c41c8-154">Saiba mais em [Suporte de marca HTML para páginas](http://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span><span class="sxs-lookup"><span data-stu-id="c41c8-154">For more information, see [HTML tag support for pages](http://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span></span> <span data-ttu-id="c41c8-155">Se uma marca não estiver listada aqui, provavelmente será ignorada.</span><span class="sxs-lookup"><span data-stu-id="c41c8-155">If a tag's not listed there, it'll probably be ignored.</span></span>

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

<span data-ttu-id="c41c8-156">A lista a seguir mostra os tipos de elementos básicos compatíveis com o Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="c41c8-156">The following list shows the basic element types that Microsoft Graph supports:</span></span>

- <span data-ttu-id="c41c8-157">`<head>` e `<body>`</span><span class="sxs-lookup"><span data-stu-id="c41c8-157">`<head>` and `<body>`</span></span></p>
- <span data-ttu-id="c41c8-158">`<title>` e `<meta>` que definem a data de criação e o título de página</span><span class="sxs-lookup"><span data-stu-id="c41c8-158">`<title>` and `<meta>` that set the page title and creation date</span></span></p>
- <span data-ttu-id="c41c8-159">`<h1>` a `<h6>` para títulos de seção</span><span class="sxs-lookup"><span data-stu-id="c41c8-159">`<h1>` through `<h6>` for section headings</span></span></p>
- <span data-ttu-id="c41c8-160">`<p>` para parágrafos</span><span class="sxs-lookup"><span data-stu-id="c41c8-160">`<p>` for paragraphs</span></span></p>
- <span data-ttu-id="c41c8-161">`<ul>`, `<ol>` e `<li>` para listas e itens de lista</span><span class="sxs-lookup"><span data-stu-id="c41c8-161">`<ul>`, `<ol>`, and `<li>` for lists and list items</span></span></p>
- <span data-ttu-id="c41c8-162">`<table>`, `<tr>` e `<td>`, incluindo tabelas aninhadas</span><span class="sxs-lookup"><span data-stu-id="c41c8-162">`<table>`, `<tr>` and `<td>`, including nested tables</span></span></p>
- <span data-ttu-id="c41c8-163">`<pre>` para texto pré-formatado (preserva as quebras de linha e espaços em branco)</span><span class="sxs-lookup"><span data-stu-id="c41c8-163">`<pre>` for preformatted text (preserves white space and line breaks)</span></span></p>
- <span data-ttu-id="c41c8-164">`<b>` e `<i>` para estilos de caractere em negrito e itálico</span><span class="sxs-lookup"><span data-stu-id="c41c8-164">`<b>` and `<i>` for bold and italic character styles</span></span></p>

<span data-ttu-id="c41c8-165">O Microsoft Graph preserva o conteúdo semântico e a estrutura básica do HTML de entrada ao criar páginas, mas converte o HTML de entrada para usar o conjunto compatível de HTML e CSS.</span><span class="sxs-lookup"><span data-stu-id="c41c8-165">Microsoft Graph preserves the semantic content and basic structure of the input HTML when it creates pages, but it converts the input HTML to use the supported set of HTML and CSS.</span></span> <span data-ttu-id="c41c8-166">Os recursos que não existem no OneNote não têm nada para ser convertido, portanto, podem não ser reconhecidos no HTML de origem.</span><span class="sxs-lookup"><span data-stu-id="c41c8-166">Features that don't exist in OneNote have nothing to be translated to, so they might not be recognized in the source HTML.</span></span> 


<a name="example"></a>

## <a name="example-request"></a><span data-ttu-id="c41c8-167">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="c41c8-167">Example request</span></span>

<span data-ttu-id="c41c8-168">Esse exemplo de solicitação de diversas partes cria uma página que contém imagens e um arquivo inserido.</span><span class="sxs-lookup"><span data-stu-id="c41c8-168">This example multipart request creates a page that contains images and an embedded file.</span></span> <span data-ttu-id="c41c8-169">A parte **Apresentação** necessária contém o HTML de entrada que define a página.</span><span class="sxs-lookup"><span data-stu-id="c41c8-169">The required **Presentation** part contains the input HTML that defines the page.</span></span> <span data-ttu-id="c41c8-170">A parte **imageBlock1** contém os dados de imagem binária, e **fileBlock1** contém os dados do arquivo binário.</span><span class="sxs-lookup"><span data-stu-id="c41c8-170">The **imageBlock1** part contains the binary image data and **fileBlock1** contains the binary file data.</span></span> <span data-ttu-id="c41c8-171">As partes de dados também podem conter HTML e, nesse caso, o Microsoft Graph [processa o HTML como uma imagem](onenote_images_files.md#add-an-image-using-binary-data) na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c41c8-171">Data parts can also contain HTML, in which case Microsoft Graph [renders the HTML as an image](onenote_images_files.md#add-an-image-using-binary-data) on the OneNote page.</span></span> 

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with rendered images and an attached file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an <i>online source</i>:</p>
    <img src="http://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as <b>binary data</b>:</p>
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

<span data-ttu-id="c41c8-172">Para obter mais exemplos que mostram como criar páginas que contêm imagens e outros arquivos, consulte [Adicionar imagens e arquivos](onenote_images_files.md), nossos [tutoriais](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-tutorial) e nossos [exemplos](https://github.com/onenotedev).</span><span class="sxs-lookup"><span data-stu-id="c41c8-172">For more examples that show how to create pages that contain images and other files, see [Add images and files](onenote_images_files.md), our [tutorials](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-tutorial), and our [samples](https://github.com/onenotedev).</span></span> <span data-ttu-id="c41c8-173">Além disso, saiba como [criar elementos posicionados absolutos](onenote-abs-pos.md), [usar marcas de anotação](onenote-note-tags.md) e [extrair dados](onenote-extract-data.md) para capturas de cartão de visita e as listagens online de receitas e de produtos.</span><span class="sxs-lookup"><span data-stu-id="c41c8-173">Also, learn how to [create absolute positioned elements](onenote-abs-pos.md), [use note tags](onenote-note-tags.md), and [extract data](onenote-extract-data.md) for business card captures and online recipe and product listings.</span></span>

<span data-ttu-id="c41c8-174">O Microsoft Graph é rigoroso com certos formatos, como novas linhas CRLF em um corpo da mensagem de diversas partes.</span><span class="sxs-lookup"><span data-stu-id="c41c8-174">Microsoft Graph is strict about some formats, such as CRLF newlines in a multipart message body.</span></span> <span data-ttu-id="c41c8-175">Para reduzir o risco de criar cargas mal formadas, você deve usar uma biblioteca para criar mensagens de diversas partes.</span><span class="sxs-lookup"><span data-stu-id="c41c8-175">To reduce the risk of creating malformed payloads, you should use a library to construct multipart messages.</span></span> 

<span data-ttu-id="c41c8-176">Se você receber o status 400 para uma carga mal formada, verifique a formatação de novas linhas e espaços em branco e verifique se há problemas de codificação.</span><span class="sxs-lookup"><span data-stu-id="c41c8-176">If you do receive a 400 status for a malformed payload, check the formatting of newlines and whitespaces, and check for encoding issues.</span></span> <span data-ttu-id="c41c8-177">Por exemplo, tente usar `charset=utf-8` (exemplo: `Content-Type: text/html; charset=utf-8`).</span><span class="sxs-lookup"><span data-stu-id="c41c8-177">For example, try using `charset=utf-8` (example: `Content-Type: text/html; charset=utf-8`).</span></span>

<span data-ttu-id="c41c8-178">Consulte [Requisitos e limitações do HTML de entrada](#requirements-and-limitations-for-input-html-in-post-pages-requests) e [Limites de tamanho para solicitações POST](onenote_images_files.md#size-limitations-for-post-pages-requests).</span><span class="sxs-lookup"><span data-stu-id="c41c8-178">See [requirements and limitations for input HTML](#requirements-and-limitations-for-input-html-in-post-pages-requests) and [size limits for POST requests](onenote_images_files.md#size-limitations-for-post-pages-requests).</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a><span data-ttu-id="c41c8-179">Informações de solicitação e resposta para solicitações de *páginas POST* </span><span class="sxs-lookup"><span data-stu-id="c41c8-179">Request and response information for *POST pages* requests</span></span>

| <span data-ttu-id="c41c8-180">Dados da solicitação</span><span class="sxs-lookup"><span data-stu-id="c41c8-180">Request data</span></span> | <span data-ttu-id="c41c8-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="c41c8-181">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c41c8-182">Protocolo</span><span class="sxs-lookup"><span data-stu-id="c41c8-182">Protocol</span></span> | <span data-ttu-id="c41c8-183">Todas as solicitações usam o protocolo HTTPS de SSL/TLS.</span><span class="sxs-lookup"><span data-stu-id="c41c8-183">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="c41c8-184">Cabeçalho de autorização</span><span class="sxs-lookup"><span data-stu-id="c41c8-184">Authorization header</span></span> | <p><span data-ttu-id="c41c8-185">`Bearer {token}`, onde `{token}` é um token de acesso do OAuth 2.0 válido para o aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="c41c8-185">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="c41c8-186">Se ele estiver ausente ou for inválido, a solicitação falhará com um código de status 401.</span><span class="sxs-lookup"><span data-stu-id="c41c8-186">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="c41c8-187">Confira [Autenticação e permissões](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c41c8-187">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="c41c8-188">Cabeçalho content-type</span><span class="sxs-lookup"><span data-stu-id="c41c8-188">Content-Type header</span></span> | <p><span data-ttu-id="c41c8-189">`text/html` ou `application/xhtml+xml` para o conteúdo HTML, seja enviado diretamente no corpo da mensagem, seja na parte "Apresentação" obrigatória de solicitações de diversas partes.</span><span class="sxs-lookup"><span data-stu-id="c41c8-189">`text/html` or `application/xhtml+xml` for the HTML content, whether it's sent directly in the message body or in the required "Presentation" part of multipart requests.</span></span></p><p><span data-ttu-id="c41c8-190">As solicitações de diversas partes são necessárias quando se enviam dados binários e usam o tipo de conteúdo `multipart/form-data; boundary=part-boundary`, onde `{part-boundary}` é uma cadeia de caracteres que sinaliza o início e o término de cada parte de dados.</span><span class="sxs-lookup"><span data-stu-id="c41c8-190">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  
| <span data-ttu-id="c41c8-191">Cabeçalho Accept</span><span class="sxs-lookup"><span data-stu-id="c41c8-191">Accept header</span></span> | `application/json` | 

<br/>

| <span data-ttu-id="c41c8-192">Dados de resposta</span><span class="sxs-lookup"><span data-stu-id="c41c8-192">Response data</span></span> | <span data-ttu-id="c41c8-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="c41c8-193">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c41c8-194">Código de êxito</span><span class="sxs-lookup"><span data-stu-id="c41c8-194">Success code</span></span> | <span data-ttu-id="c41c8-195">Um código de status HTTP 201.</span><span class="sxs-lookup"><span data-stu-id="c41c8-195">A 201 HTTP status code.</span></span> |  
| <span data-ttu-id="c41c8-196">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="c41c8-196">Response body</span></span> | <span data-ttu-id="c41c8-197">Uma representação OData da nova página no formato JSON.</span><span class="sxs-lookup"><span data-stu-id="c41c8-197">A OData representation of the new page in JSON format.</span></span> |  
| <span data-ttu-id="c41c8-198">Erros</span><span class="sxs-lookup"><span data-stu-id="c41c8-198">Errors</span></span> | <span data-ttu-id="c41c8-199">Se a solicitação falhar, a API retornará erros no objeto **@api.diagnostics** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c41c8-199">If the request fails, the API returns errors in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="c41c8-200">Cabeçalho location</span><span class="sxs-lookup"><span data-stu-id="c41c8-200">Location header</span></span> | <span data-ttu-id="c41c8-201">A URL do recurso para a nova página.</span><span class="sxs-lookup"><span data-stu-id="c41c8-201">The resource URL for the new page.</span></span> |  
| <span data-ttu-id="c41c8-202">Cabeçalho X-CorrelationId</span><span class="sxs-lookup"><span data-stu-id="c41c8-202">X-CorrelationId header</span></span> | <span data-ttu-id="c41c8-203">Um GUID que identifica de forma exclusiva a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c41c8-203">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="c41c8-204">Você pode usar esse valor juntamente com o valor do cabeçalho Data ao trabalhar com o suporte da Microsoft para solucionar problemas.</span><span class="sxs-lookup"><span data-stu-id="c41c8-204">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="c41c8-205">Criar a URL raiz do serviço do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c41c8-205">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="c41c8-206">A URL raiz do serviço do Microsoft Graph usa o formato a seguir para todas as chamadas para o Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="c41c8-206">The Microsoft Graph service root URL uses the following format for all calls to Microsoft Graph.</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="c41c8-207">O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="c41c8-207">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="c41c8-208">Use `v1.0` para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="c41c8-208">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="c41c8-209">Use `beta` para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="c41c8-209">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="c41c8-210">Os recursos e a funcionalidade na versão beta podem mudar, por isso, você não deve usá-la no código de produção.</span><span class="sxs-lookup"><span data-stu-id="c41c8-210">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="c41c8-211">Use `me` para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="c41c8-211">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="c41c8-212">Use `users/{id}` para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="c41c8-212">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="c41c8-213">Use o [Microsoft Graph](https://graph.microsoft.com/v1.0/users) para obter as IDs de usuário.</span><span class="sxs-lookup"><span data-stu-id="c41c8-213">Use the [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="c41c8-214">Permissões</span><span class="sxs-lookup"><span data-stu-id="c41c8-214">Permissions</span></span>

<span data-ttu-id="c41c8-215">Para criar páginas do OneNote, solicite as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="c41c8-215">To create OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="c41c8-216">Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="c41c8-216">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="c41c8-217">Escolha entre:</span><span class="sxs-lookup"><span data-stu-id="c41c8-217">Choose from:</span></span>

- <span data-ttu-id="c41c8-218">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="c41c8-218">Notes.Create</span></span>
- <span data-ttu-id="c41c8-219">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c41c8-219">Notes.ReadWrite</span></span>
- <span data-ttu-id="c41c8-220">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c41c8-220">Notes.ReadWrite.All</span></span>

<span data-ttu-id="c41c8-221">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Referência de permissões do Microsoft Graph](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c41c8-221">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>




<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="c41c8-222">Confira também</span><span class="sxs-lookup"><span data-stu-id="c41c8-222">See also</span></span>

- [<span data-ttu-id="c41c8-223">Adicionar imagens e arquivos</span><span class="sxs-lookup"><span data-stu-id="c41c8-223">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="c41c8-224">Criar elementos posicionados absolutos</span><span class="sxs-lookup"><span data-stu-id="c41c8-224">Create absolute positioned elements</span></span>](onenote-abs-pos.md)  
- [<span data-ttu-id="c41c8-225">Extrair dados</span><span class="sxs-lookup"><span data-stu-id="c41c8-225">Extract data</span></span>](onenote-extract-data.md)
- [<span data-ttu-id="c41c8-226">Usar marcas de anotação</span><span class="sxs-lookup"><span data-stu-id="c41c8-226">Use note tags</span></span>](onenote-note-tags.md)
- [<span data-ttu-id="c41c8-227">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="c41c8-227">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="c41c8-228">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="c41c8-228">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="c41c8-229">Perguntas sobre desenvolvimento do OneNote no Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="c41c8-229">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="c41c8-230">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="c41c8-230">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  


