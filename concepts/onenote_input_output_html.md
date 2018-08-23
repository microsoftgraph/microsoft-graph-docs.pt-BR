# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="c31a6-101">HTML de entrada e saída nas páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="c31a6-101">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="c31a6-102">O HTML que define o conteúdo e a estrutura da página quando você [cria](onenote-create-page.md) ou [atualiza](onenote_update_page.md) uma página do OneNote é chamado de *HTML de entrada*.</span><span class="sxs-lookup"><span data-stu-id="c31a6-102">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote_update_page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="c31a6-103">O HTML que é retornado quando você [obtém o conteúdo da página](onenote-get-content.md) é chamado de *HTML de saída*.</span><span class="sxs-lookup"><span data-stu-id="c31a6-103">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*.</span></span> <span data-ttu-id="c31a6-104">O HTML de saída não será igual ao HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="c31a6-104">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="c31a6-105">As APIs do OneNote no Microsoft Graph preservam o conteúdo semântico e a estrutura básica do HTML de entrada, mas os convertem em um conjunto de [elementos HTML e propriedades CSS com suporte](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="c31a6-105">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="c31a6-106">As APIs também adicionam atributos personalizados que dão suporte a recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c31a6-106">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="c31a6-107">Este artigo descreve os principais elementos e atributos do HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-107">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="c31a6-108">Pode ser útil entender o HTML de entrada quando você estiver criando ou atualizando o conteúdo da página e o HTML de saída quando estiver analisando o conteúdo da página retornado.</span><span class="sxs-lookup"><span data-stu-id="c31a6-108">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="c31a6-109">elemento body</span><span class="sxs-lookup"><span data-stu-id="c31a6-109">Body element</span></span>

<span data-ttu-id="c31a6-110">O conteúdo HTML no corpo da página representa o conteúdo e a estrutura da página incluindo os recursos de imagem e arquivo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-110">The HTML content in the page body represents the page content and structure, including image and file resources.</span></span> <span data-ttu-id="c31a6-111">O elemento **body** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-111">The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="c31a6-112">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-112">Input attributes</span></span>

|<span data-ttu-id="c31a6-113">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-113">Input attribute</span></span>|<span data-ttu-id="c31a6-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-114">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-115">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="c31a6-115">data-absolute-enabled</span></span> | <span data-ttu-id="c31a6-116">Indica se o corpo da entrada dá suporte a elementos [posicionados absolutos](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-116">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="c31a6-117">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-117">style</span></span> | <p><span data-ttu-id="c31a6-118">As propriedades [style](#styles) do CSS do corpo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-118">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="c31a6-119">No HTML de saída, as configurações de entrada podem ser retornadas embutidas em elementos filho apropriados.</span><span class="sxs-lookup"><span data-stu-id="c31a6-119">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="c31a6-120">Atualmente, a cor da tela de fundo não tem suporte para o elemento **body**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-120">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="c31a6-121">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-121">Output attributes</span></span>

|<span data-ttu-id="c31a6-122">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-122">Output attribute</span></span>|<span data-ttu-id="c31a6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-123">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-124">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="c31a6-124">data-absolute-enabled</span></span> | <span data-ttu-id="c31a6-125">Indica se o corpo dá suporte a elementos [posicionados absolutos](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-125">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> <span data-ttu-id="c31a6-126">Sempre **true** no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-126">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="c31a6-127">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-127">style</span></span> | <span data-ttu-id="c31a6-128">As propriedades **font-family** e **font-size** do corpo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-128">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="c31a6-129">elementos Div</span><span class="sxs-lookup"><span data-stu-id="c31a6-129">Div elements</span></span>

<span data-ttu-id="c31a6-130">Os elementos **div** contêm texto, imagens e outros tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-130">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="c31a6-131">Um elemento **div** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-131">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="c31a6-132">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-132">Input attributes</span></span>

|<span data-ttu-id="c31a6-133">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-133">Input attribute</span></span>|<span data-ttu-id="c31a6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-134">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-135">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-135">data-id</span></span> | <span data-ttu-id="c31a6-136">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-136">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-137">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-137">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-138">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="c31a6-138">data-render-fallback</span></span> | <span data-ttu-id="c31a6-139">A ação de fallback se [extraction](onenote-extract-data.md) falhar: **render** (padrão) ou **none**</span><span class="sxs-lookup"><span data-stu-id="c31a6-139">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**.</span></span> |
| <span data-ttu-id="c31a6-140">data-render-method</span><span class="sxs-lookup"><span data-stu-id="c31a6-140">data-render-method</span></span> | <span data-ttu-id="c31a6-141">O método [extraction](onenote-extract-data.md) a ser executado, por exemplo:</span><span class="sxs-lookup"><span data-stu-id="c31a6-141">The [extraction](onenote-extract-data.md) method to perform, for example:  or .</span></span><br/><span data-ttu-id="c31a6-142">`extract.businesscard` ou `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="c31a6-142">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="c31a6-143">data-render-src</span><span class="sxs-lookup"><span data-stu-id="c31a6-143">data-render-src</span></span> | <span data-ttu-id="c31a6-144">A fonte de conteúdo para [extraction](onenote-extract-data.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-144">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="c31a6-145">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-145">style</span></span> | <span data-ttu-id="c31a6-146">As propriedades de posição, tamanho, fonte e cor para o div:</span><span class="sxs-lookup"><span data-stu-id="c31a6-146">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="c31a6-147">**position** (apenas **absolute**), **left**, **top** e **width** (a altura é configurada automaticamente para divs)</span><span class="sxs-lookup"><span data-stu-id="c31a6-147">**position** (**absolute** only), **left**, **top**, and **width** (height is auto-configured for divs)</span></span><br/><br/><span data-ttu-id="c31a6-148">Usado para criar um div [posicionado absoluto](onenote-abs-pos.md), somente se o div for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="c31a6-148">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="c31a6-149">Exemplo: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="c31a6-149">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="c31a6-150">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-150">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="c31a6-151">No HTML de saída, esses valores são retornados embutidos em elementos filho apropriados.</span><span class="sxs-lookup"><span data-stu-id="c31a6-151">In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="c31a6-152">As APIs do OneNote no Microsoft Graph encapsulam todo o conteúdo do corpo em pelo menos um div.</span><span class="sxs-lookup"><span data-stu-id="c31a6-152">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="c31a6-153">A API cria um div padrão (atribuído com `data-id="_default"`) para incluir o conteúdo do corpo se:</span><span class="sxs-lookup"><span data-stu-id="c31a6-153">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="c31a6-154">O atributo **data-absolute-enabled** do elemento body de entrada for omitido ou definido como **false**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-154">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**.</span></span> <span data-ttu-id="c31a6-155">Nesse caso, todo o conteúdo do corpo é colocado no div padrão.</span><span class="sxs-lookup"><span data-stu-id="c31a6-155">In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="c31a6-156">O atributo **data-absolute-enabled** do elemento body de entrada for **true**, mas o HTML de entrada contiver filhos diretos que não são [elementos](onenote-abs-pos.md)&nbsp;**div**, **img** ou **object** posicionados de forma absoluta.</span><span class="sxs-lookup"><span data-stu-id="c31a6-156">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="c31a6-157">Nesse caso, os filhos diretos que não forem [elementos](onenote-abs-pos.md)&nbsp;**div**, **img** ou **object** posicionados de forma absoluta serão colocados no div padrão.</span><span class="sxs-lookup"><span data-stu-id="c31a6-157">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="c31a6-158">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-158">Output attributes</span></span>

|<span data-ttu-id="c31a6-159">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-159">Output attribute</span></span>|<span data-ttu-id="c31a6-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-160">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-161">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-161">data-id</span></span> | <span data-ttu-id="c31a6-162">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-162">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-163">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-163">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-164">id</span><span class="sxs-lookup"><span data-stu-id="c31a6-164">id</span></span> | <span data-ttu-id="c31a6-165">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-165">A unique, generated ID for the element.</span></span> <span data-ttu-id="c31a6-166">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="c31a6-166">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="c31a6-167">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-167">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-168">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-168">style</span></span> | <span data-ttu-id="c31a6-169">As propriedades de tamanho e posição do div.</span><span class="sxs-lookup"><span data-stu-id="c31a6-169">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="c31a6-170">Divs não contribuintes</span><span class="sxs-lookup"><span data-stu-id="c31a6-170">Non-contributing divs</span></span>

<span data-ttu-id="c31a6-171">Quando um elemento **div** no HTML de entrada não contribui com a estrutura da página nem carrega informações usadas pelo OneNote, a API move o conteúdo do div para o div pai ou padrão.</span><span class="sxs-lookup"><span data-stu-id="c31a6-171">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="c31a6-172">Isso é ilustrado nos exemplos a seguir.</span><span class="sxs-lookup"><span data-stu-id="c31a6-172">This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="c31a6-173">HTML de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-173">Input HTML</span></span>

<span data-ttu-id="c31a6-174">Contém um div aninhado, não contribuinte.</span><span class="sxs-lookup"><span data-stu-id="c31a6-174">Contains a non-contributing, nested div.</span></span>

```html
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
        <div>
            <p>Some text</p>
            <div>
                <p>More text inside a div that doesn't define page structure</p>
            </div>
        </div>
    </body>
</html>
```

#### <a name="output-html"></a><span data-ttu-id="c31a6-175">HTML de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-175">Output HTML</span></span>

> <span data-ttu-id="c31a6-176">**Observação:** o conteúdo do div foi movido para o div pai e as marcas `<div>` aninhadas foram removidas.</span><span class="sxs-lookup"><span data-stu-id="c31a6-176">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="c31a6-177">O div seria preservado se definisse qualquer informação semântica, como **data-id** (exemplo: `<div data-id="keep-me">`).</span><span class="sxs-lookup"><span data-stu-id="c31a6-177">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11px">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <p>Some text</p>
            <p>More text inside a nested div</p>
        </div>
    </body>
</html>
```


## <a name="img-elements"></a><span data-ttu-id="c31a6-178">elementos img</span><span class="sxs-lookup"><span data-stu-id="c31a6-178">Img elements</span></span>

<span data-ttu-id="c31a6-179">Imagens em páginas do OneNote são representadas pelos elementos **img**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-179">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="c31a6-180">Um elemento **img** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-180">An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="c31a6-181">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-181">Input attributes</span></span>

|<span data-ttu-id="c31a6-182">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-182">Input attribute</span></span>|<span data-ttu-id="c31a6-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-183">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-184">alt</span><span class="sxs-lookup"><span data-stu-id="c31a6-184">alt</span></span> | <span data-ttu-id="c31a6-185">O texto Alt fornecido para a imagem.</span><span class="sxs-lookup"><span data-stu-id="c31a6-185">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="c31a6-186">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-186">data-id</span></span> | <span data-ttu-id="c31a6-187">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-187">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-188">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-188">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-189">data-render-src</span><span class="sxs-lookup"><span data-stu-id="c31a6-189">data-render-src</span></span> |<span data-ttu-id="c31a6-190">Ou **data-render-src** ou **src** é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c31a6-190">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="c31a6-191">A página da Web a ser renderizada como uma imagem mapeada por bit na página do OneNote:</span><span class="sxs-lookup"><span data-stu-id="c31a6-191">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="c31a6-192">- `data-render-src="http://..."` para uma URL pública.</span><span class="sxs-lookup"><span data-stu-id="c31a6-192">- `data-render-src="http://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="c31a6-193">- `data-render-src="name:BlockName"` para parte de uma imagem no bloco "Apresentação" de uma [solicitação de partes múltiplas](../api-reference/v1.0/api/section_post_pages.md#example).</span><span class="sxs-lookup"><span data-stu-id="c31a6-193">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span><br/><br/><span data-ttu-id="c31a6-194">Esse método é útil quando a página da Web é mais complexa que a página que o OneNote pode renderizar fielmente ou quando a página exige credenciais de logon.</span><span class="sxs-lookup"><span data-stu-id="c31a6-194">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="c31a6-195">data-tag</span><span class="sxs-lookup"><span data-stu-id="c31a6-195">data-tag</span></span> | <span data-ttu-id="c31a6-196">Uma [marca de anotação](onenote-note-tags.md) no elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-196">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="c31a6-197">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-197">style</span></span> |<span data-ttu-id="c31a6-198">As propriedades de posição e tamanho para a imagem: **position** (somente **absolute**), **left**, **top**, **width** e **height**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-198">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="c31a6-199">O tamanho pode ser definido em qualquer imagem.</span><span class="sxs-lookup"><span data-stu-id="c31a6-199">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="c31a6-200">As propriedades de posição serão usadas para criar uma imagem [posicionada absoluta](onenote-abs-pos.md), somente se a imagem for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="c31a6-200">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="c31a6-201">Exemplo: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="c31a6-201">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="c31a6-202">No HTML de saída, o tamanho da imagem é retornado separadamente nos atributos **width** e **height**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-202">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="c31a6-203">src</span><span class="sxs-lookup"><span data-stu-id="c31a6-203">src</span></span> |<span data-ttu-id="c31a6-204">Ou **src** ou **data-render-src** é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c31a6-204">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="c31a6-205">A imagem a ser renderizada na página do OneNote:</span><span class="sxs-lookup"><span data-stu-id="c31a6-205">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="c31a6-206">- `src="http://..."` para uma URL para uma imagem publicamente disponível na Internet.</span><span class="sxs-lookup"><span data-stu-id="c31a6-206">- `src="http://..."` for a URL to a publicly available image on the internet.</span></span><br/><br/> <span data-ttu-id="c31a6-207">- `src="name:BlockName"` para uma parte nomeada em uma solicitação da partes múltiplas que representa a imagem.</span><span class="sxs-lookup"><span data-stu-id="c31a6-207">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="c31a6-208">width, height</span><span class="sxs-lookup"><span data-stu-id="c31a6-208">width, height</span></span> | <span data-ttu-id="c31a6-209">A largura ou altura da imagem, em pixels, mas sem o px.</span><span class="sxs-lookup"><span data-stu-id="c31a6-209">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="c31a6-210">Exemplo: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="c31a6-210">Example: `width="400"`</span></span> |
 
> <span data-ttu-id="c31a6-211">**Observação:** as APIs do OneNote detectam automaticamente o tipo de imagem de entrada e o retorna como **data-fullres-src-type** no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-211">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="c31a6-212">A API também retorna o tipo de imagem da imagem otimizada em **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-212">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="c31a6-213">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-213">Output attributes</span></span>

|<span data-ttu-id="c31a6-214">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-214">Output attribute</span></span>|<span data-ttu-id="c31a6-215">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-215">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-216">alt</span><span class="sxs-lookup"><span data-stu-id="c31a6-216">alt</span></span> | <span data-ttu-id="c31a6-217">O texto Alt fornecido para a imagem.</span><span class="sxs-lookup"><span data-stu-id="c31a6-217">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="c31a6-218">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-218">data-id</span></span> | <span data-ttu-id="c31a6-219">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-219">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-220">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-220">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-221">data-index</span><span class="sxs-lookup"><span data-stu-id="c31a6-221">data-index</span></span> | <span data-ttu-id="c31a6-222">A posição da imagem.</span><span class="sxs-lookup"><span data-stu-id="c31a6-222">The position of the image.</span></span> <span data-ttu-id="c31a6-223">Para suporte à [divisão de imagem](#split-images).</span><span class="sxs-lookup"><span data-stu-id="c31a6-223">For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="c31a6-224">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="c31a6-224">data-fullres-src</span></span> | <span data-ttu-id="c31a6-225">O ponto de extremidade para a versão do recurso de imagem que foi originalmente inserido na página.</span><span class="sxs-lookup"><span data-stu-id="c31a6-225">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="c31a6-226">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="c31a6-226">data-fullres-src-type</span></span> | <span data-ttu-id="c31a6-227">O tipo de mídia do recurso **data-fullres-src**, por exemplo: `image/png` ou `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="c31a6-227">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="c31a6-228">data-options</span><span class="sxs-lookup"><span data-stu-id="c31a6-228">data-options</span></span> | <span data-ttu-id="c31a6-229">O tipo de fonte: **printout** para arquivos PDF ou **splitimage** para todos os outros.</span><span class="sxs-lookup"><span data-stu-id="c31a6-229">The source type: **printout** for PDF files or **splitimage** for all others.</span></span> <span data-ttu-id="c31a6-230">Aplica-se somente à [divisão de imagens](#split-images) criada com o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-230">Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="c31a6-231">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="c31a6-231">data-render-original-src</span></span> | <span data-ttu-id="c31a6-232">A URL de origem original da imagem, se a imagem da origem for da Internet pública e tiver sido criada com o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-232">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="c31a6-233">data-src-type</span><span class="sxs-lookup"><span data-stu-id="c31a6-233">data-src-type</span></span> | <span data-ttu-id="c31a6-234">O tipo de mídia do recurso **src**, por exemplo: `image/png` ou `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="c31a6-234">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="c31a6-235">data-tag</span><span class="sxs-lookup"><span data-stu-id="c31a6-235">data-tag</span></span> | <span data-ttu-id="c31a6-236">Uma [marca de anotação](onenote-note-tags.md) no elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-236">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="c31a6-237">id</span><span class="sxs-lookup"><span data-stu-id="c31a6-237">id</span></span> | <span data-ttu-id="c31a6-238">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-238">A unique, generated ID for the element.</span></span> <span data-ttu-id="c31a6-239">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="c31a6-239">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="c31a6-240">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-240">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-241">src</span><span class="sxs-lookup"><span data-stu-id="c31a6-241">src</span></span> | <span data-ttu-id="c31a6-242">O ponto de extremidade para a versão do recurso de imagem que foi otimizada para navegadores da Web, bem como para fatores forma de dispositivos móveis e tablet.</span><span class="sxs-lookup"><span data-stu-id="c31a6-242">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="c31a6-243">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-243">style</span></span> | <span data-ttu-id="c31a6-244">As propriedades de posição da imagem.</span><span class="sxs-lookup"><span data-stu-id="c31a6-244">The position properties of the image.</span></span> |
| <span data-ttu-id="c31a6-245">width, height</span><span class="sxs-lookup"><span data-stu-id="c31a6-245">width, height</span></span> | <span data-ttu-id="c31a6-246">A largura ou altura da imagem, em pixels.</span><span class="sxs-lookup"><span data-stu-id="c31a6-246">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="c31a6-247">Exemplos de HTML de saída para imagens</span><span class="sxs-lookup"><span data-stu-id="c31a6-247">Output HTML examples for images</span></span>

<span data-ttu-id="c31a6-248">Os elementos **img** de saída contêm pontos de extremidade para recursos de arquivo de imagem e o tipo de imagem, como mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-248">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="c31a6-249">Você pode fazer [solicitações GET separadas a pontos de extremidade de recurso de imagem](../api-reference/v1.0/api/resource_get.md) para recuperar os respectivos conteúdos binários.</span><span class="sxs-lookup"><span data-stu-id="c31a6-249">You can make separate [GET requests to image resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="c31a6-250">Por padrão, as imagens não serão renderizadas diretamente em um navegador, pois elas são privadas e é necessária autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="c31a6-250">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> <span data-ttu-id="c31a6-251">Para obter URLs públicas para os recursos de imagem em uma página, inclua **preAuthenticated=true** na cadeia de caracteres de consulta ao recuperar o conteúdo da página (exemplo: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="c31a6-251">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="c31a6-252">As URLs públicas que são retornadas são válidas por uma hora.</span><span class="sxs-lookup"><span data-stu-id="c31a6-252">The public URLs that are returned are valid for one hour.</span></span> 

#### <a name="image-with-public-url-when-preauthenticatedtrue-is-included-in-the-request"></a><span data-ttu-id="c31a6-253">Imagem com URL pública quando _preAuthenticated=true_ é incluído na solicitação</span><span class="sxs-lookup"><span data-stu-id="c31a6-253">Image with public URL when _preAuthenticated=true_ is included in the request</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}"
/>
```

<span data-ttu-id="c31a6-254">Os exemplos a seguir mostram as informações que um elemento **img** pode conter no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-254">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="c31a6-255">Imagem com recursos de resolução alta e prontos para Web</span><span class="sxs-lookup"><span data-stu-id="c31a6-255">Image with web-ready and high resolution resources</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    [data-render-original-src="{original-source-url-or-named-part}"]
    [data-id="{image-id}"]
    [alt="supplied alt text"]
    [width="345"] [height="180"]
    [style="..."] />
```

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="c31a6-256">Imagem criada usando o atributo *data-render-src*</span><span class="sxs-lookup"><span data-stu-id="c31a6-256">Image created by using the *data-render-src* attribute</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    data-render-original-src="{original-source-url-or-named-part}"
    [data-id="{image-id}"]
    [data-index="{index-of-split-image}"]
    [data-options="{printout-or-splitimage}"]
    [alt="supplied alt text"]
    [width="1024"] [height="1900"]
    [style="..."] />
```

### <a name="split-images"></a><span data-ttu-id="c31a6-257">Dividir imagens</span><span class="sxs-lookup"><span data-stu-id="c31a6-257">Split images</span></span>

<span data-ttu-id="c31a6-258">As imagens que são criadas usando o atributo **data-render-src** (de uma URL de página da Web ou de uma parte nomeada) podem ser divididas em várias imagens de componente por motivos de desempenho e renderização.</span><span class="sxs-lookup"><span data-stu-id="c31a6-258">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons.</span></span> <span data-ttu-id="c31a6-259">Todas as imagens de componente recebem o mesmo valor de **data-id**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-259">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="c31a6-260">Cada imagem de componente tem um atributo de índice por dados com base zero que define o layout vertical original.</span><span class="sxs-lookup"><span data-stu-id="c31a6-260">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="c31a6-261">Dividir imagem com três imagens de componente</span><span class="sxs-lookup"><span data-stu-id="c31a6-261">Split image with three component images</span></span>

```html
<div data-id="multi-component-image" style="position:absolute;left:48px;top:120px;width:624px">
    <img
        src="{image-resource0-url}/$value"
        data-src-type="image/{type}"
        data-fullres-src="{image-resource0-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="0" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource1-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource1-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="1" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource2-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource2-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="2" 
        data-render-original-src=""{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
</div>
```

<span data-ttu-id="c31a6-262">Como os usuários podem mover as imagens na página, os índices retornados podem estar fora de ordem.</span><span class="sxs-lookup"><span data-stu-id="c31a6-262">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="c31a6-263">A ordenação deve estar na ordem y de cima para baixo e, na ordem x da esquerda para a direita, se houver conflitos na ordem y.</span><span class="sxs-lookup"><span data-stu-id="c31a6-263">Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="c31a6-264">Elementos iframe</span><span class="sxs-lookup"><span data-stu-id="c31a6-264">iframe elements</span></span>

<span data-ttu-id="c31a6-265">As páginas do OneNote podem conter vídeos inseridos representados pelos elementos **iframe**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-265">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="c31a6-266">**Observação:** você também pode [anexar um arquivo de vídeo usando um elemento **object**](onenote_images_files.md#adding-files).</span><span class="sxs-lookup"><span data-stu-id="c31a6-266">**Note:** You can also [attach a video file using an **object** element](onenote_images_files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="c31a6-267">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-267">Input attributes</span></span>

|<span data-ttu-id="c31a6-268">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-268">Input attribute</span></span>|<span data-ttu-id="c31a6-269">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-269">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-270">data-original-src</span><span class="sxs-lookup"><span data-stu-id="c31a6-270">data-original-src</span></span> | <span data-ttu-id="c31a6-271">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c31a6-271">Required.</span></span> <span data-ttu-id="c31a6-272">A URL da fonte do vídeo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-272">The URL of the video source.</span></span> <span data-ttu-id="c31a6-273">Veja a [lista de fontes de vídeo com suporte](onenote_images_files.md#adding-videos).</span><span class="sxs-lookup"><span data-stu-id="c31a6-273">See the [list of supported video sources](onenote_images_files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="c31a6-274">Exemplo: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="c31a6-274">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="c31a6-275">width, height</span><span class="sxs-lookup"><span data-stu-id="c31a6-275">width, height</span></span> | <span data-ttu-id="c31a6-276">A largura ou altura do iframe, em pixels.</span><span class="sxs-lookup"><span data-stu-id="c31a6-276">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="c31a6-277">Exemplo: `width=300`</span><span class="sxs-lookup"><span data-stu-id="c31a6-277">Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="c31a6-278">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-278">Output attributes</span></span>

|<span data-ttu-id="c31a6-279">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-279">Output attribute</span></span>|<span data-ttu-id="c31a6-280">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-280">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-281">data-original-src</span><span class="sxs-lookup"><span data-stu-id="c31a6-281">data-original-src</span></span> | <span data-ttu-id="c31a6-282">A URL da fonte do vídeo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-282">The URL of the video source.</span></span> |
| <span data-ttu-id="c31a6-283">src</span><span class="sxs-lookup"><span data-stu-id="c31a6-283">src</span></span> | <span data-ttu-id="c31a6-284">O link para o vídeo que é inserido na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c31a6-284">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="c31a6-285">width, height</span><span class="sxs-lookup"><span data-stu-id="c31a6-285">width, height</span></span> | <span data-ttu-id="c31a6-286">A largura ou altura do iframe, em pixels.</span><span class="sxs-lookup"><span data-stu-id="c31a6-286">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="c31a6-287">Exemplo: `width=300`</span><span class="sxs-lookup"><span data-stu-id="c31a6-287">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="c31a6-288">Exemplo de HTML de saída para vídeos</span><span class="sxs-lookup"><span data-stu-id="c31a6-288">Output HTML example for videos</span></span>

<span data-ttu-id="c31a6-289">Os elementos **iframe** de saída contêm pontos de extremidade que se vinculam à página e ao vídeo da fonte, como mostrado.</span><span class="sxs-lookup"><span data-stu-id="c31a6-289">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="c31a6-290">elementos object</span><span class="sxs-lookup"><span data-stu-id="c31a6-290">Object elements</span></span>

<span data-ttu-id="c31a6-291">As páginas do OneNote contêm anexos de arquivo representados pelos elementos **object**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-291">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="c31a6-292">Um elemento **object** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-292">An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="c31a6-293">**Observação:** As APIs do OneNote também podem renderizar conteúdo de arquivo como imagens em uma página quando o arquivo é enviado como uma imagem e usa o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-293">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="c31a6-294">Exemplo: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="c31a6-294">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="c31a6-295">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-295">Input attributes</span></span>

|<span data-ttu-id="c31a6-296">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-296">Input attribute</span></span>|<span data-ttu-id="c31a6-297">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-297">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-298">data</span><span class="sxs-lookup"><span data-stu-id="c31a6-298">data</span></span> | <span data-ttu-id="c31a6-299">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c31a6-299">Required.</span></span> <span data-ttu-id="c31a6-300">O nome da parte que representa o arquivo na [solicitação de partes múltiplas](../api-reference/v1.0/api/section_post_pages.md#example).</span><span class="sxs-lookup"><span data-stu-id="c31a6-300">The name of the part that represents the file in the [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span> |
| <span data-ttu-id="c31a6-301">data-attachment</span><span class="sxs-lookup"><span data-stu-id="c31a6-301">data-attachment</span></span> | <span data-ttu-id="c31a6-302">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c31a6-302">Required.</span></span> <span data-ttu-id="c31a6-303">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-303">The file name.</span></span> |
| <span data-ttu-id="c31a6-304">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-304">data-id</span></span> | <span data-ttu-id="c31a6-305">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-305">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-306">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-306">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-307">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-307">style</span></span> | <span data-ttu-id="c31a6-308">As propriedades de posição e tamanho para o objeto: **position** (somente **absolute**), **left**, **top** e **width**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-308">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="c31a6-309">Usado para criar um objeto [posicionado absoluto](onenote-abs-pos.md), somente se o objeto for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="c31a6-309">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="c31a6-310">Exemplo: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="c31a6-310">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="c31a6-311">type</span><span class="sxs-lookup"><span data-stu-id="c31a6-311">type</span></span> | <span data-ttu-id="c31a6-312">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c31a6-312">Required.</span></span><br/><br/><span data-ttu-id="c31a6-313">O tipo de arquivo de mídia padrão.</span><span class="sxs-lookup"><span data-stu-id="c31a6-313">The standard media file type.</span></span> <span data-ttu-id="c31a6-314">Os tipos de arquivo conhecidos exibem o ícone associado ao tipo de arquivo na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c31a6-314">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="c31a6-315">Os tipos de arquivo desconhecidos exibem um ícone de arquivo genérico.</span><span class="sxs-lookup"><span data-stu-id="c31a6-315">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="c31a6-316">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-316">Output attributes</span></span>

|<span data-ttu-id="c31a6-317">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-317">Output attribute</span></span>|<span data-ttu-id="c31a6-318">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-318">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-319">data</span><span class="sxs-lookup"><span data-stu-id="c31a6-319">data</span></span> | <span data-ttu-id="c31a6-320">O ponto de extremidade para o recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-320">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="c31a6-321">data-attachment</span><span class="sxs-lookup"><span data-stu-id="c31a6-321">data-attachment</span></span> | <span data-ttu-id="c31a6-322">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-322">The file name.</span></span> |
| <span data-ttu-id="c31a6-323">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-323">data-id</span></span> | <span data-ttu-id="c31a6-324">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-324">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-325">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-325">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-326">id</span><span class="sxs-lookup"><span data-stu-id="c31a6-326">id</span></span> | <span data-ttu-id="c31a6-327">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-327">A unique, generated ID for the element.</span></span> <span data-ttu-id="c31a6-328">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="c31a6-328">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="c31a6-329">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-329">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-330">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-330">style</span></span> | <span data-ttu-id="c31a6-331">As propriedades de posição do objeto.</span><span class="sxs-lookup"><span data-stu-id="c31a6-331">The position properties of the object.</span></span> |
| <span data-ttu-id="c31a6-332">type</span><span class="sxs-lookup"><span data-stu-id="c31a6-332">type</span></span> | <span data-ttu-id="c31a6-333">O tipo de arquivo de mídia padrão.</span><span class="sxs-lookup"><span data-stu-id="c31a6-333">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="c31a6-334">Exemplo de HTML de saída para objetos</span><span class="sxs-lookup"><span data-stu-id="c31a6-334">Output HTML example for objects</span></span>

<span data-ttu-id="c31a6-335">Os elementos **object** de saída contêm pontos de extremidade que se vinculam aos recursos de arquivo na página, como mostrado.</span><span class="sxs-lookup"><span data-stu-id="c31a6-335">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="c31a6-336">Você pode fazer [solicitações GET separadas a pontos de extremidade de recurso de arquivo](../api-reference/v1.0/api/resource_get.md) para recuperar os respectivos conteúdos binários.</span><span class="sxs-lookup"><span data-stu-id="c31a6-336">You can make separate [GET requests to file resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="c31a6-337">Parágrafos e cabeçalhos</span><span class="sxs-lookup"><span data-stu-id="c31a6-337">Paragraphs and headings</span></span>

<span data-ttu-id="c31a6-338">Os parágrafos, cabeçalhos e outros contêineres de texto podem incluir os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-338">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="c31a6-339">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-339">Input attributes</span></span>

|<span data-ttu-id="c31a6-340">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-340">Input attribute</span></span>|<span data-ttu-id="c31a6-341">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-341">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-342">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-342">data-id</span></span> | <span data-ttu-id="c31a6-343">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-343">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-344">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-344">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-345">data-tag</span><span class="sxs-lookup"><span data-stu-id="c31a6-345">data-tag</span></span> | <span data-ttu-id="c31a6-346">Uma [marca de anotação](onenote-note-tags.md) em um elemento **p** ou **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-346">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="c31a6-347">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-347">style</span></span> | <span data-ttu-id="c31a6-348">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-348">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="c31a6-349">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-349">Output attributes</span></span>

|<span data-ttu-id="c31a6-350">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-350">Output attribute</span></span>|<span data-ttu-id="c31a6-351">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-351">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-352">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-352">data-id</span></span> | <span data-ttu-id="c31a6-353">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-353">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-354">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-354">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-355">data-tag</span><span class="sxs-lookup"><span data-stu-id="c31a6-355">data-tag</span></span> | <span data-ttu-id="c31a6-356">Uma [marca de anotação](onenote-note-tags.md) em um elemento **p** ou **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-356">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="c31a6-357">id</span><span class="sxs-lookup"><span data-stu-id="c31a6-357">id</span></span> | <span data-ttu-id="c31a6-358">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-358">A unique, generated ID for the element.</span></span> <span data-ttu-id="c31a6-359">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="c31a6-359">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="c31a6-360">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-360">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-361">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-361">style</span></span> | <span data-ttu-id="c31a6-362">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-362">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="c31a6-363">No HTML de saída, esses valores podem ser retornados embutidos em elementos filho apropriados ou em elementos **span**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-363">In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="c31a6-364">Os exemplos a seguir mostram HTML de entrada que usa maneiras diferentes de definir estilos em contêineres de texto e o HTML de saída que é retornado.</span><span class="sxs-lookup"><span data-stu-id="c31a6-364">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="c31a6-365">HTML de entrada com estilos definidos usando estilos de caractere embutidos, na marca de início, e dentro de um elemento span.</span><span class="sxs-lookup"><span data-stu-id="c31a6-365">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="c31a6-366">Saída HTML com o estilo de caractere `<i>` e as configurações de fonte na marca de início `<p>` retornadas como estilos CSS embutidos em elementos span.</span><span class="sxs-lookup"><span data-stu-id="c31a6-366">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="c31a6-367">Listas</span><span class="sxs-lookup"><span data-stu-id="c31a6-367">Lists</span></span>

<span data-ttu-id="c31a6-368">As listas são representadas como elementos **ol** ou **ul** que contêm itens de lista representados como elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-368">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="c31a6-369">Listas e itens de lista podem conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-369">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="c31a6-370">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-370">Input attributes</span></span>

|<span data-ttu-id="c31a6-371">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-371">Input attribute</span></span>|<span data-ttu-id="c31a6-372">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-372">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-373">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-373">data-id</span></span> | <span data-ttu-id="c31a6-374">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-374">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-375">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-375">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-376">data-tag</span><span class="sxs-lookup"><span data-stu-id="c31a6-376">data-tag</span></span> | <span data-ttu-id="c31a6-377">Uma [marca de anotação](onenote-note-tags.md) em um elemento **ul**, **ol** ou **li**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-377">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="c31a6-378">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-378">style</span></span> | <span data-ttu-id="c31a6-379">O **list-style-type** e as propriedades [style](#styles) do CSS para a lista ou o item de lista.</span><span class="sxs-lookup"><span data-stu-id="c31a6-379">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="c31a6-380">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-380">Output attributes</span></span>

|<span data-ttu-id="c31a6-381">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-381">Output attribute</span></span>|<span data-ttu-id="c31a6-382">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-382">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-383">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-383">data-id</span></span> | <span data-ttu-id="c31a6-384">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-384">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-385">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-385">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-386">data-tag</span><span class="sxs-lookup"><span data-stu-id="c31a6-386">data-tag</span></span> |  <span data-ttu-id="c31a6-387">Uma [marca de anotação](onenote-note-tags.md) em um período em um elemento **li**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-387">A [note tag](onenote-note-tags.md) on a span in a **li** element.</span></span> |
| <span data-ttu-id="c31a6-388">id</span><span class="sxs-lookup"><span data-stu-id="c31a6-388">id</span></span> | <span data-ttu-id="c31a6-389">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-389">A unique, generated ID for the element.</span></span> <span data-ttu-id="c31a6-390">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="c31a6-390">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="c31a6-391">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-391">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-392">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-392">style</span></span> | <span data-ttu-id="c31a6-393">O **list-style-type** e as propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-393">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="c31a6-394">No HTML de saída, as configurações no nível de lista são retornadas em itens de lista.</span><span class="sxs-lookup"><span data-stu-id="c31a6-394">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="c31a6-395">As propriedades padrão não são retornadas.</span><span class="sxs-lookup"><span data-stu-id="c31a6-395">Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="c31a6-396">Estilos de lista</span><span class="sxs-lookup"><span data-stu-id="c31a6-396">List styles</span></span>

<span data-ttu-id="c31a6-397">As APIs do OneNote no Microsoft Graph dão suporte aos seguintes estilos de lista:</span><span class="sxs-lookup"><span data-stu-id="c31a6-397">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="c31a6-398">Lista ordenada</span><span class="sxs-lookup"><span data-stu-id="c31a6-398">Ordered list</span></span>|<span data-ttu-id="c31a6-399">Lista não ordenada</span><span class="sxs-lookup"><span data-stu-id="c31a6-399">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-400">nenhum</span><span class="sxs-lookup"><span data-stu-id="c31a6-400">none</span></span> | <span data-ttu-id="c31a6-401">nenhum</span><span class="sxs-lookup"><span data-stu-id="c31a6-401">none</span></span> |
| <span data-ttu-id="c31a6-402">decimal (padrão)</span><span class="sxs-lookup"><span data-stu-id="c31a6-402">decimal (default)</span></span> | <span data-ttu-id="c31a6-403">disc (padrão)</span><span class="sxs-lookup"><span data-stu-id="c31a6-403">disc (default)</span></span> |
| <span data-ttu-id="c31a6-404">alfa inferior</span><span class="sxs-lookup"><span data-stu-id="c31a6-404">lower-alpha</span></span> | <span data-ttu-id="c31a6-405">círculo</span><span class="sxs-lookup"><span data-stu-id="c31a6-405">circle</span></span> |
| <span data-ttu-id="c31a6-406">romano inferior</span><span class="sxs-lookup"><span data-stu-id="c31a6-406">lower-roman</span></span> | <span data-ttu-id="c31a6-407">quadrado</span><span class="sxs-lookup"><span data-stu-id="c31a6-407">square</span></span> |
| <span data-ttu-id="c31a6-408">alfa superior</span><span class="sxs-lookup"><span data-stu-id="c31a6-408">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="c31a6-409">romano superior</span><span class="sxs-lookup"><span data-stu-id="c31a6-409">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="c31a6-410">Você pode aplicar estilos globais para uma lista no elemento **ol** ou **ul** no HTML de entrada, mas estilos são retornados nos elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-410">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="c31a6-411">Estilo de lista homogêneo</span><span class="sxs-lookup"><span data-stu-id="c31a6-411">Homogenous list style</span></span>

<span data-ttu-id="c31a6-412">Este exemplo mostra o HTML de entrada que define o tipo de estilo de lista no elemento **ol** e estilos CSS em itens de lista individuais.</span><span class="sxs-lookup"><span data-stu-id="c31a6-412">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="c31a6-413">Este é o HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-413">This is the output HTML.</span></span> <span data-ttu-id="c31a6-414">Observe que os estilos são retornados embutidos nos elementos **li** ou **span** individuais.</span><span class="sxs-lookup"><span data-stu-id="c31a6-414">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="c31a6-415">Estilos de lista variáveis</span><span class="sxs-lookup"><span data-stu-id="c31a6-415">Variable list styles</span></span>

<span data-ttu-id="c31a6-416">Este exemplo mostra o HTML de entrada que define diferentes tipos de estilo de lista nos elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-416">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="c31a6-417">Este é o HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-417">This is the output HTML.</span></span> <span data-ttu-id="c31a6-418">Observe que os estilos são retornados embutidos nos elementos **li** ou **span** individuais.</span><span class="sxs-lookup"><span data-stu-id="c31a6-418">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="c31a6-419">Tabelas</span><span class="sxs-lookup"><span data-stu-id="c31a6-419">Tables</span></span>

<span data-ttu-id="c31a6-420">As tabelas são representadas como elementos **table** que podem conter elementos **tr** e **td**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-420">Tables are represented as **table** elements that can contain **tr** and **td** elements.</span></span> <span data-ttu-id="c31a6-421">Há suporte para tabelas aninhadas.</span><span class="sxs-lookup"><span data-stu-id="c31a6-421">Nested tables are supported.</span></span>

<span data-ttu-id="c31a6-422">As tabelas podem conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="c31a6-422">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="c31a6-423">As APIs do OneNote não dão suporte aos atributos **rowspan** ou **colspan**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-423">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="c31a6-424">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-424">Input attributes</span></span>

|<span data-ttu-id="c31a6-425">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="c31a6-425">Input attribute</span></span>|<span data-ttu-id="c31a6-426">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-426">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-427">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-427">data-id</span></span> | <span data-ttu-id="c31a6-428">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-428">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-429">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-429">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-430">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-430">style</span></span> | <span data-ttu-id="c31a6-431">As propriedades [style](#styles) do CSS do elemento e também:</span><span class="sxs-lookup"><span data-stu-id="c31a6-431">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="c31a6-432">- **border** (borda).</span><span class="sxs-lookup"><span data-stu-id="c31a6-432">- **border**.</span></span> <span data-ttu-id="c31a6-433">Pode ser 0px ou 1px.</span><span class="sxs-lookup"><span data-stu-id="c31a6-433">Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="c31a6-434">- **width** (largura).</span><span class="sxs-lookup"><span data-stu-id="c31a6-434">- **width**.</span></span> <span data-ttu-id="c31a6-435">Com suporte de **table** e **td** como pixels ou porcentagem de largura da página.</span><span class="sxs-lookup"><span data-stu-id="c31a6-435">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="c31a6-436">Exemplo: `width="100px"` ou `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="c31a6-436">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="c31a6-437">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-437">Output attributes</span></span>

|<span data-ttu-id="c31a6-438">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-438">Output attribute</span></span>|<span data-ttu-id="c31a6-439">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a6-439">Description</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-440">data-id</span><span class="sxs-lookup"><span data-stu-id="c31a6-440">data-id</span></span> | <span data-ttu-id="c31a6-441">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-441">A reference for the element.</span></span><br/><br/><span data-ttu-id="c31a6-442">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-442">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-443">id</span><span class="sxs-lookup"><span data-stu-id="c31a6-443">id</span></span> | <span data-ttu-id="c31a6-444">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-444">A unique, generated ID for the element.</span></span> <span data-ttu-id="c31a6-445">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="c31a6-445">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="c31a6-446">Usado para [atualizar conteúdo da página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-446">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="c31a6-447">style</span><span class="sxs-lookup"><span data-stu-id="c31a6-447">style</span></span> | <span data-ttu-id="c31a6-448">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="c31a6-448">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="c31a6-449">Os exemplos a seguir mostram HTML de entrada que usa maneiras diferentes de definir estilos em tabelas e o HTML de saída que é retornado.</span><span class="sxs-lookup"><span data-stu-id="c31a6-449">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="c31a6-450">HTML de entrada com configurações opcionais em níveis diferentes</span><span class="sxs-lookup"><span data-stu-id="c31a6-450">Input HTML with optional settings at different levels.</span></span>

```html
<table style="border:0px;width:500px;background-color:green">
    <tr> 
        <td>Cell 1</td> 
        <td>Cell 2</td> 
        <td>Cell 3</td> 
    </tr> 
    <tr style="background-color:blue"> 
        <td style="text-align:right;background-color:red">Left</td> 
        <td style="text-align:center">Middle</td> 
        <td>Right</td> 
    </tr> 
</table>
```
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="c31a6-451">HTML de saída com estilos CSS retornados embutidos nos elementos td</span><span class="sxs-lookup"><span data-stu-id="c31a6-451">Output HTML with CSS styles returned inline on the td elements.</span></span>

```html
<table style="border:0px">
    <tr>
        <td style="background-color:green;width:166;border:0px">Cell 1</td>
        <td style="background-color:green;width:166;border:0px">Cell 2</td>
        <td style="background-color:green;width:166;border:0px">Cell 3</td>
    </tr>
    <tr>
        <td style="background-color:red;width:166;border:0px;text-align:right">Left</td>
        <td style="background-color:blue;width:166;border:0px;text-align:center">Middle</td>
        <td style="background-color:blue;width:166;border:0px">Right</td>
    </tr>
</table>
``` 


## <a name="styles"></a><span data-ttu-id="c31a6-452">Estilos</span><span class="sxs-lookup"><span data-stu-id="c31a6-452">Styles</span></span>

<span data-ttu-id="c31a6-453">As APIs do OneNote no Microsoft Graph dão suporte as propriedades **style** do CSS embutidas a seguir para elementos no corpo da página, como **body**, **div**, **p**, **li** e **span**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-453">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="c31a6-454">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c31a6-454">Property</span></span>|<span data-ttu-id="c31a6-455">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c31a6-455">Example</span></span>|
|:------|:------|
| <span data-ttu-id="c31a6-456">background-color</span><span class="sxs-lookup"><span data-stu-id="c31a6-456">background-color</span></span> | <span data-ttu-id="c31a6-457">`style="background-color:#66cc66"` (o padrão é branco)</span><span class="sxs-lookup"><span data-stu-id="c31a6-457">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="c31a6-458">Há suporte para cores nomeadas e formato hexadecimal.</span><span class="sxs-lookup"><span data-stu-id="c31a6-458">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="c31a6-459">color</span><span class="sxs-lookup"><span data-stu-id="c31a6-459">color</span></span> | <span data-ttu-id="c31a6-460">`style="color:#ffffff"` (o padrão é preto)</span><span class="sxs-lookup"><span data-stu-id="c31a6-460">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="c31a6-461">font-family</span><span class="sxs-lookup"><span data-stu-id="c31a6-461">font-family</span></span> | <span data-ttu-id="c31a6-462">`style="font-family:Courier"` (o padrão é Calibri)</span><span class="sxs-lookup"><span data-stu-id="c31a6-462">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="c31a6-463">font-size</span><span class="sxs-lookup"><span data-stu-id="c31a6-463">font-size</span></span> | <span data-ttu-id="c31a6-464">`style="font-size:10pt"` (o padrão é 11pt)</span><span class="sxs-lookup"><span data-stu-id="c31a6-464">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="c31a6-465">As APIs aceitam o tamanho da fonte em *pt* ou *px*, mas converte *px* em *pt*.</span><span class="sxs-lookup"><span data-stu-id="c31a6-465">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="c31a6-466">Valores decimais são arredondados para o n,0pt ou n,5pt mais próximo.</span><span class="sxs-lookup"><span data-stu-id="c31a6-466">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="c31a6-467">font-style</span><span class="sxs-lookup"><span data-stu-id="c31a6-467">font-style</span></span> | <span data-ttu-id="c31a6-468">`style="font-style:italic"` (somente normal ou itálico)</span><span class="sxs-lookup"><span data-stu-id="c31a6-468">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="c31a6-469">font-weight</span><span class="sxs-lookup"><span data-stu-id="c31a6-469">font-weight</span></span> | <span data-ttu-id="c31a6-470">`style="font-weight:bold"` (somente normal ou negrito)</span><span class="sxs-lookup"><span data-stu-id="c31a6-470">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="c31a6-471">strike-through</span><span class="sxs-lookup"><span data-stu-id="c31a6-471">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="c31a6-472">text-align</span><span class="sxs-lookup"><span data-stu-id="c31a6-472">text-align</span></span> | <span data-ttu-id="c31a6-473">`style="text-align:center"` (somente para elementos de bloco)</span><span class="sxs-lookup"><span data-stu-id="c31a6-473">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="c31a6-474">text-decoration</span><span class="sxs-lookup"><span data-stu-id="c31a6-474">text-decoration</span></span> | <span data-ttu-id="c31a6-475">`style="text-decoration:underline"` (somente nenhum ou sublinhado)</span><span class="sxs-lookup"><span data-stu-id="c31a6-475">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="c31a6-476">Os seguintes estilos de caractere embutidos também têm suporte:</span><span class="sxs-lookup"><span data-stu-id="c31a6-476">The following inline character styles and are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="c31a6-477">&lt;b&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-477">&lt;b&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="c31a6-478">&lt;i&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-478">&lt;i&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="c31a6-479">&lt;u&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-479">&lt;u&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="c31a6-480">&lt;em&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-480">&lt;em&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="c31a6-481">&lt;strong&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-481">&lt;strong&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="c31a6-482">&lt;strike&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-482">&lt;strike&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="c31a6-483">&lt;sup&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-483">&lt;sup&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="c31a6-484">&lt;sub&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-484">&lt;sub&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="c31a6-485">&lt;del&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-485">&lt;del&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="c31a6-486">&lt;cite&gt;</span><span class="sxs-lookup"><span data-stu-id="c31a6-486">&lt;cite&gt;</span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="c31a6-487">Exemplo de HTML de entrada e saída</span><span class="sxs-lookup"><span data-stu-id="c31a6-487">Input and output HTML example</span></span>

<span data-ttu-id="c31a6-488">A imagem a seguir mostra uma página simples que foi criada com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c31a6-488">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Imagem de uma página do OneNote com notas de conteúdo do estudo da Wikipédia](images/onenote-sample-image.png)

<span data-ttu-id="c31a6-490">Este é o HTML de entrada enviado no corpo da mensagem para criar a página.</span><span class="sxs-lookup"><span data-stu-id="c31a6-490">This is the input HTML sent in the message body to create the page.</span></span>

```html
<html lang="en-US">
    <head>
        <title>Sample Study Notes</title>
        <meta name="created" content="2015-01-01T01:01"/>
    </head>
    <body>
        <h1>Aurora Borealis</h1>
        <p>Dancing lights in the sky. Also called <i>Northern Lights</i>. Caused by solar radiation.</p>
        <br />
        <p><b>Intersting facts</b></p>
        <table>
            <tr>
                <td>Neil Armstrong</td>
                <td>Commander</td>
            </tr>
            <tr>
                <td>Buzz Aldrin</td>
                <td>LM Pilot</td>
            </tr>
            <tr>
                <td>Michael Collins</td>
                <td>Command Module Pilot</td>
            </tr>
        </table>
        <img alt="Apollo 11 commemorative stamp." src="http://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<br/>

<span data-ttu-id="c31a6-491">Este é o HTML de saída que o Microsoft Graph retorna quando você [obtém o conteúdo da página](onenote-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="c31a6-491">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="c31a6-492">**Observação:** quando você [cria uma página](onenote-create-page.md) ou [obtém metadados de página](../api-reference/v1.0/api/page_get.md), a API retorna a URL de ponto de extremidade do *conteúdo* da página na propriedade **contentUrl**.</span><span class="sxs-lookup"><span data-stu-id="c31a6-492">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](../api-reference/v1.0/api/page_get.md), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Sample Study Notes</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">American History 101: Moon Landing</h1>
            <p>First moon landing - July 20, 1969 with Apollo 11 (Eagle)</p>
            <br />
            <p><span style="font-weight:bold">Apollo 11 Astronauts</span></p>
            <table style="border:0px">
                <tr>
                    <td style="border:0px">Neil Armstrong</td>
                    <td style="border:0px">Commander</td>
                </tr>
                <tr>
                    <td style="border:0px">Buzz Aldrin</td>
                    <td style="border:0px">LM Pilot</td>
                </tr>
                <tr>
                    <td style="border:0px">Michael Collins</td>
                    <td style="border:0px">Command Module Pilot</td>
                </tr>
            </table>
            <br />
            <img alt="Apollo 11 commemorative stamp." width="400" height="248" src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value"
                 data-src-type="image/jpeg" data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value" data-fullres-src-type="image/jpeg" />
            <p>References:</p>
            <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="c31a6-493">Confira também</span><span class="sxs-lookup"><span data-stu-id="c31a6-493">See also</span></span>

- [<span data-ttu-id="c31a6-494">Obter a estrutura e o conteúdo do OneNote</span><span class="sxs-lookup"><span data-stu-id="c31a6-494">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="c31a6-495">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="c31a6-495">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="c31a6-496">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="c31a6-496">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="c31a6-497">Adicionar imagens, vídeos e arquivos</span><span class="sxs-lookup"><span data-stu-id="c31a6-497">Add images, videos, and files</span></span>](onenote_images_files.md)
