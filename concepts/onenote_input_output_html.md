# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="8351b-101">HTML de entrada e saída nas páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="8351b-101">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="8351b-102">O HTML que define o conteúdo e a estrutura da página quando você [cria](../api-reference/v1.0/api/section_post_pages.md) ou [atualiza](../api-reference/v1.0/api/page_update.md) uma página do OneNote é chamado de *HTML de entrada*.</span><span class="sxs-lookup"><span data-stu-id="8351b-102">The HTML that defines the page content and structure when you [create](../api-reference/v1.0/api/section_post_pages.md) or [update](../api-reference/v1.0/api/page_update.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="8351b-103">O HTML que é retornado quando você [obtém o conteúdo da página](../api-reference/v1.0/api/page_get.md) é chamado de *HTML de saída*.</span><span class="sxs-lookup"><span data-stu-id="8351b-103">The HTML that's returned when you [get page content](../api-reference/v1.0/api/page_get.md) is called *output HTML*.</span></span> <span data-ttu-id="8351b-104">O HTML de saída não será igual ao HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="8351b-104">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="8351b-105">As APIs do OneNote no Microsoft Graph preservam o conteúdo semântico e a estrutura básica do HTML de entrada, mas os convertem em um conjunto de [elementos HTML e propriedades CSS com suporte](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-create-page#supported-html).</span><span class="sxs-lookup"><span data-stu-id="8351b-105">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-create-page#supported-html).</span></span> <span data-ttu-id="8351b-106">As APIs também adicionam atributos personalizados que dão suporte a recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="8351b-106">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="8351b-107">Este artigo descreve os principais elementos e atributos do HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-107">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="8351b-108">Pode ser útil entender o HTML de entrada quando você estiver criando ou atualizando o conteúdo da página e o HTML de saída quando estiver analisando o conteúdo da página retornado.</span><span class="sxs-lookup"><span data-stu-id="8351b-108">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="8351b-109">Elemento body</span><span class="sxs-lookup"><span data-stu-id="8351b-109">Body element</span></span>
<span data-ttu-id="8351b-110">O conteúdo HTML no corpo da página representa o conteúdo e a estrutura da página, inclusive os recursos de imagem e arquivo.</span><span class="sxs-lookup"><span data-stu-id="8351b-110">The HTML content in the page body represents the page content and structure, including image and file resources.</span></span> <span data-ttu-id="8351b-111">O elemento **body** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-111">The **body** element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="8351b-112">**Atributos de entrada**</span><span class="sxs-lookup"><span data-stu-id="8351b-112">**Input attributes**</span></span>

|<span data-ttu-id="8351b-113">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="8351b-113">Input attribute</span></span>|<span data-ttu-id="8351b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-114">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-115">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="8351b-115">data-absolute-enabled</span></span> | <span data-ttu-id="8351b-116">Indica se o corpo da entrada dá suporte a elementos [posicionados absolutos](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="8351b-116">Indicates whether the input body supports [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) elements.</span></span> |
| <span data-ttu-id="8351b-117">style</span><span class="sxs-lookup"><span data-stu-id="8351b-117">style</span></span> | <p><span data-ttu-id="8351b-118">As propriedades [style](#styles) do CSS do corpo.</span><span class="sxs-lookup"><span data-stu-id="8351b-118">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="8351b-119">No HTML de saída, as configurações de entrada podem ser retornadas embutidas em elementos filho apropriados.</span><span class="sxs-lookup"><span data-stu-id="8351b-119">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="8351b-120">Atualmente, a cor da tela de fundo não tem suporte para o elemento **body**.</span><span class="sxs-lookup"><span data-stu-id="8351b-120">Background color is not currently supported for the **body** element.</span></span></p> |
 

<span data-ttu-id="8351b-121">**Atributos de saída**</span><span class="sxs-lookup"><span data-stu-id="8351b-121">**Output attributes**</span></span>

|<span data-ttu-id="8351b-122">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="8351b-122">Output attribute</span></span>|<span data-ttu-id="8351b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-123">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-124">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="8351b-124">data-absolute-enabled</span></span> | <span data-ttu-id="8351b-125">Indica se o corpo dá suporte a elementos [posicionados absolutos](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="8351b-125">Indicates whether the body supports [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) elements.</span></span> <span data-ttu-id="8351b-126">Sempre **true** no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-126">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="8351b-127">style</span><span class="sxs-lookup"><span data-stu-id="8351b-127">style</span></span> | <span data-ttu-id="8351b-128">As propriedades **font-family** e **font-size** do corpo.</span><span class="sxs-lookup"><span data-stu-id="8351b-128">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="8351b-129">Elementos Div</span><span class="sxs-lookup"><span data-stu-id="8351b-129">Div elements</span></span>
<span data-ttu-id="8351b-130">Os elementos **Div** contêm texto, imagens e outros tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8351b-130">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="8351b-131">Um elemento **div** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-131">A **div** element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="8351b-132">**Atributos de entrada**</span><span class="sxs-lookup"><span data-stu-id="8351b-132">**Input attributes**</span></span>

|<span data-ttu-id="8351b-133">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="8351b-133">Input attribute</span></span>|<span data-ttu-id="8351b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-134">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-135">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-135">data-id</span></span> | <span data-ttu-id="8351b-136">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-136">A reference for the element.</span></span> <span data-ttu-id="8351b-137">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-137">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-138">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="8351b-138">data-render-fallback</span></span> | <span data-ttu-id="8351b-139">A ação de fallback se [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) falhar: **render** (padrão) ou **none**.</span><span class="sxs-lookup"><span data-stu-id="8351b-139">The fallback action if the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) fails: **render** (default) or **none**.</span></span> |
| <span data-ttu-id="8351b-140">data-render-method</span><span class="sxs-lookup"><span data-stu-id="8351b-140">data-render-method</span></span> | <span data-ttu-id="8351b-141">O método [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) a ser executado, por exemplo: `extract.businesscard` ou `extract.recipe`.</span><span class="sxs-lookup"><span data-stu-id="8351b-141">The [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) method to perform, for example: `extract.businesscard` or `extract.recipe`.</span></span> |
| <span data-ttu-id="8351b-142">data-render-src</span><span class="sxs-lookup"><span data-stu-id="8351b-142">data-render-src</span></span> | <span data-ttu-id="8351b-143">A fonte de conteúdo para [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span><span class="sxs-lookup"><span data-stu-id="8351b-143">The content source for the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span></span> |
| <span data-ttu-id="8351b-144">style</span><span class="sxs-lookup"><span data-stu-id="8351b-144">style</span></span> | <p><span data-ttu-id="8351b-145">As propriedades de posição, tamanho, fonte e cor para o div:</span><span class="sxs-lookup"><span data-stu-id="8351b-145">The position, size, font, and color properties for the div:</span></span></p><p> <span data-ttu-id="8351b-146">- **position** (apenas **absolute**), **left**, **top** e **width**.</span><span class="sxs-lookup"><span data-stu-id="8351b-146">- **position** (**absolute** only), **left**, **top**, and **width**.</span></span> <span data-ttu-id="8351b-147">(A altura é configurada automaticamente para divs.)</span><span class="sxs-lookup"><span data-stu-id="8351b-147">(Height is auto-configured for divs.)</span></span><br /><span data-ttu-id="8351b-148">Usado para criar um div [posicionado absoluto](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos), somente se o div for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="8351b-148">Used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="8351b-149">Exemplo: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="8351b-149">Example`<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></p><p> <span data-ttu-id="8351b-150">- As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-150">- The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="8351b-151">No HTML de saída, esses valores são retornados embutidos em elementos filho apropriados.</span><span class="sxs-lookup"><span data-stu-id="8351b-151">In the output HTML, these values are returned inline on appropriate child elements.</span></span></p> |
 

<span data-ttu-id="8351b-152">As APIs do OneNote no Microsoft Graph encapsulam todo o conteúdo do corpo em pelo menos um div.</span><span class="sxs-lookup"><span data-stu-id="8351b-152">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="8351b-153">A API cria um div padrão (atribuído com `data-id="_default"`) para incluir o conteúdo do corpo se:</span><span class="sxs-lookup"><span data-stu-id="8351b-153">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="8351b-154">O atributo **data-absolute-enabled** do elemento body de entrada for omitido ou definido como **false**.</span><span class="sxs-lookup"><span data-stu-id="8351b-154">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**.</span></span> <span data-ttu-id="8351b-155">Nesse caso, todo o conteúdo do corpo é colocado no div padrão.</span><span class="sxs-lookup"><span data-stu-id="8351b-155">In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="8351b-156">O atributo **data-absolute-enabled** do elemento body de entrada for **true**, mas o HTML de entrada contiver filhos diretos que não são [elementos](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img** ou **object** posicionados de forma absoluta.</span><span class="sxs-lookup"><span data-stu-id="8351b-156">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="8351b-157">Nesse caso, os filhos diretos que não forem [elementos](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img** ou **object** posicionados de forma absoluta serão colocados no div padrão.</span><span class="sxs-lookup"><span data-stu-id="8351b-157">In this case, direct children that aren't [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


<span data-ttu-id="8351b-158">**Atributos de saída**</span><span class="sxs-lookup"><span data-stu-id="8351b-158">**Output attributes**</span></span>

|<span data-ttu-id="8351b-159">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="8351b-159">Output attribute</span></span>|<span data-ttu-id="8351b-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-160">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-161">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-161">data-id</span></span> | <span data-ttu-id="8351b-162">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-162">A reference for the element.</span></span> <span data-ttu-id="8351b-163">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-163">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-164">id</span><span class="sxs-lookup"><span data-stu-id="8351b-164">id</span></span> | <span data-ttu-id="8351b-165">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-165">A unique ID for the group.</span></span> <span data-ttu-id="8351b-166">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="8351b-166">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="8351b-167">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-167">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-168">style</span><span class="sxs-lookup"><span data-stu-id="8351b-168">style</span></span> | <span data-ttu-id="8351b-169">As propriedades de tamanho e posição do div.</span><span class="sxs-lookup"><span data-stu-id="8351b-169">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="8351b-170">Divs não contribuintes</span><span class="sxs-lookup"><span data-stu-id="8351b-170">Non-contributing divs</span></span>
<span data-ttu-id="8351b-171">Quando um elemento **div** no HTML de entrada não contribui com a estrutura da página nem carrega informações usadas pelo OneNote, a API move o conteúdo do div para o div pai ou padrão.</span><span class="sxs-lookup"><span data-stu-id="8351b-171">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="8351b-172">Isso é ilustrado nos exemplos a seguir.</span><span class="sxs-lookup"><span data-stu-id="8351b-172">This is illustrated in the following examples.</span></span>

<span data-ttu-id="8351b-173">**HTML de entrada** que contém um div aninhado não contribuinte.</span><span class="sxs-lookup"><span data-stu-id="8351b-173">**Input HTML** that contains a non-contributing, nested div.</span></span>

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

<span data-ttu-id="8351b-174">**HTML de saída**</span><span class="sxs-lookup"><span data-stu-id="8351b-174">**Output HTML**</span></span>

><span data-ttu-id="8351b-175">**Observação:** o conteúdo do div foi movido para o div pai e as marcas `<div>` aninhadas foram removidas.</span><span class="sxs-lookup"><span data-stu-id="8351b-175">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="8351b-176">O div seria preservado se definisse qualquer informação semântica, como **data-id** (exemplo: `<div data-id="keep-me">`).</span><span class="sxs-lookup"><span data-stu-id="8351b-176">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

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


## <a name="img-elements"></a><span data-ttu-id="8351b-177">Elementos Img</span><span class="sxs-lookup"><span data-stu-id="8351b-177">Img elements</span></span>
<span data-ttu-id="8351b-178">Imagens em páginas do OneNote são representadas pelos elementos **img**.</span><span class="sxs-lookup"><span data-stu-id="8351b-178">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="8351b-179">Um elemento **img** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-179">An **img** element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="8351b-180">**Atributos de entrada**</span><span class="sxs-lookup"><span data-stu-id="8351b-180">**Input attributes**</span></span>

|<span data-ttu-id="8351b-181">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="8351b-181">Input attribute</span></span>|<span data-ttu-id="8351b-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-182">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-183">alt</span><span class="sxs-lookup"><span data-stu-id="8351b-183">ALT</span></span> | <span data-ttu-id="8351b-184">O texto Alt fornecido para a imagem.</span><span class="sxs-lookup"><span data-stu-id="8351b-184">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="8351b-185">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-185">data-id</span></span> | <span data-ttu-id="8351b-186">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-186">A reference for the element.</span></span> <span data-ttu-id="8351b-187">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-187">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-188">data-render-src</span><span class="sxs-lookup"><span data-stu-id="8351b-188">data-render-src</span></span> |<span data-ttu-id="8351b-189">Ou **data-render-src** ou **src** é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8351b-189">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="8351b-190">A página da Web a ser renderizada como uma imagem mapeada por bit na página do OneNote:</span><span class="sxs-lookup"><span data-stu-id="8351b-190">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br /> <span data-ttu-id="8351b-191">- `data-render-src="http://..."` para uma URL pública.</span><span class="sxs-lookup"><span data-stu-id="8351b-191">- `data-render-src="http://..."` for a public URL.</span></span><br /> <span data-ttu-id="8351b-192">- `data-render-src="name:BlockName"` para parte de uma imagem no bloco "Apresentação" de uma [solicitação de partes múltiplas](../api-reference/v1.0/api/section_post_pages.md#example).</span><span class="sxs-lookup"><span data-stu-id="8351b-192">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span><br/><br/><span data-ttu-id="8351b-193">Esse método é útil quando a página da Web é mais complexa que a página que o OneNote pode renderizar fielmente ou quando a página exige credenciais de logon.</span><span class="sxs-lookup"><span data-stu-id="8351b-193">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="8351b-194">data-tag</span><span class="sxs-lookup"><span data-stu-id="8351b-194">data-tag</span></span> | <span data-ttu-id="8351b-195">Uma [marca de anotação](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) no elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-195">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="8351b-196">style</span><span class="sxs-lookup"><span data-stu-id="8351b-196">style</span></span> |<span data-ttu-id="8351b-197">As propriedades de posição e tamanho para a imagem: **position** (somente **absolute**), **left**, **top**, **width** e **height**.</span><span class="sxs-lookup"><span data-stu-id="8351b-197">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="8351b-198">O tamanho pode ser definido em qualquer imagem.</span><span class="sxs-lookup"><span data-stu-id="8351b-198">Size can be set on any image.</span></span> <span data-ttu-id="8351b-199">As propriedades de posição serão usadas para criar uma imagem [posicionada absoluta](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos), somente se a imagem for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="8351b-199">Position properties are used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="8351b-200">Exemplo: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="8351b-200">Example`<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="8351b-201">No HTML de saída, o tamanho da imagem é retornado separadamente nos atributos **width** e **height**.</span><span class="sxs-lookup"><span data-stu-id="8351b-201">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="8351b-202">src</span><span class="sxs-lookup"><span data-stu-id="8351b-202">Src</span></span> |<span data-ttu-id="8351b-203">Ou **src** ou **data-render-src** é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8351b-203">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="8351b-204">A imagem a ser renderizada na página do OneNote:</span><span class="sxs-lookup"><span data-stu-id="8351b-204">The image to render on the OneNote page:</span></span><br /> <span data-ttu-id="8351b-205">- `src="http://..."` para uma URL para uma imagem publicamente disponível na Internet.</span><span class="sxs-lookup"><span data-stu-id="8351b-205">- `src="http://..."` for a URL to a publicly available image on the internet.</span></span><br /> <span data-ttu-id="8351b-206">- `src="name:BlockName"` para uma parte nomeada em uma solicitação da partes múltiplas que representa a imagem.</span><span class="sxs-lookup"><span data-stu-id="8351b-206">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="8351b-207">width, height</span><span class="sxs-lookup"><span data-stu-id="8351b-207">width, height</span></span> | <span data-ttu-id="8351b-208">A largura ou altura da imagem, em pixels, mas sem o px.</span><span class="sxs-lookup"><span data-stu-id="8351b-208">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="8351b-209">Exemplo: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="8351b-209">Example`width="400"`</span></span> |
 
><span data-ttu-id="8351b-210">**Observação:** as APIs do OneNote detectam automaticamente o tipo de imagem de entrada e o retorna como o **data-fullres-src-type** no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-210">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="8351b-211">A API também retorna o tipo de imagem da imagem otimizada em **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="8351b-211">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

<span data-ttu-id="8351b-212">**Atributos de saída**</span><span class="sxs-lookup"><span data-stu-id="8351b-212">**Output attributes**</span></span>

|<span data-ttu-id="8351b-213">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="8351b-213">Output attribute</span></span>|<span data-ttu-id="8351b-214">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-214">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-215">alt</span><span class="sxs-lookup"><span data-stu-id="8351b-215">ALT</span></span> | <span data-ttu-id="8351b-216">O texto Alt fornecido para a imagem.</span><span class="sxs-lookup"><span data-stu-id="8351b-216">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="8351b-217">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-217">data-id</span></span> | <span data-ttu-id="8351b-218">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-218">A reference for the element.</span></span> <span data-ttu-id="8351b-219">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-219">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-220">data-index</span><span class="sxs-lookup"><span data-stu-id="8351b-220">data-index</span></span> | <span data-ttu-id="8351b-221">A posição da imagem.</span><span class="sxs-lookup"><span data-stu-id="8351b-221">The position of the value.</span></span> <span data-ttu-id="8351b-222">Para suporte à [divisão de imagem](#split-images).</span><span class="sxs-lookup"><span data-stu-id="8351b-222">For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="8351b-223">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="8351b-223">data-fullres-src</span></span> | <span data-ttu-id="8351b-224">O ponto de extremidade para a versão do recurso de imagem que foi originalmente inserido na página.</span><span class="sxs-lookup"><span data-stu-id="8351b-224">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="8351b-225">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="8351b-225">data-fullres-src-type</span></span> | <span data-ttu-id="8351b-226">O tipo de mídia do recurso **data-fullres-src**, por exemplo: `image/png` ou `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="8351b-226">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="8351b-227">data-options</span><span class="sxs-lookup"><span data-stu-id="8351b-227">data-options</span></span> | <span data-ttu-id="8351b-228">O tipo de fonte: **printout** para arquivos PDF ou **splitimage** para todos os outros.</span><span class="sxs-lookup"><span data-stu-id="8351b-228">The source type: **printout** for PDF files or **splitimage** for all others.</span></span> <span data-ttu-id="8351b-229">Aplica-se somente à [divisão de imagens](#split-images) criada com o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="8351b-229">Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="8351b-230">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="8351b-230">data-render-original-src</span></span> | <span data-ttu-id="8351b-231">A URL de origem original da imagem, se a imagem da origem for da Internet pública e tiver sido criada com o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="8351b-231">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="8351b-232">data-src-type</span><span class="sxs-lookup"><span data-stu-id="8351b-232">data-src-type</span></span> | <span data-ttu-id="8351b-233">O tipo de mídia do recurso **src**, por exemplo: `image/png` ou `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="8351b-233">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="8351b-234">data-tag</span><span class="sxs-lookup"><span data-stu-id="8351b-234">data-tag</span></span> | <span data-ttu-id="8351b-235">Uma [marca de anotação](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) no elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-235">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="8351b-236">id</span><span class="sxs-lookup"><span data-stu-id="8351b-236">id</span></span> | <span data-ttu-id="8351b-237">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-237">A unique ID for the group.</span></span> <span data-ttu-id="8351b-238">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="8351b-238">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="8351b-239">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-239">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-240">src</span><span class="sxs-lookup"><span data-stu-id="8351b-240">Src</span></span> | <span data-ttu-id="8351b-241">O ponto de extremidade para a versão do recurso de imagem que foi otimizada para navegadores da Web, bem como para fatores forma de dispositivos móveis e tablet.</span><span class="sxs-lookup"><span data-stu-id="8351b-241">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="8351b-242">style</span><span class="sxs-lookup"><span data-stu-id="8351b-242">style</span></span> | <span data-ttu-id="8351b-243">As propriedades de posição da imagem.</span><span class="sxs-lookup"><span data-stu-id="8351b-243">The position properties of the image.</span></span> |
| <span data-ttu-id="8351b-244">width, height</span><span class="sxs-lookup"><span data-stu-id="8351b-244">width, height</span></span> | <span data-ttu-id="8351b-245">A largura ou altura da imagem, em pixels.</span><span class="sxs-lookup"><span data-stu-id="8351b-245">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="8351b-246">Exemplos de HTML de saída para imagens</span><span class="sxs-lookup"><span data-stu-id="8351b-246">Output HTML examples for images</span></span>
<span data-ttu-id="8351b-247">Os elementos **img** de saída contêm pontos de extremidade para recursos de arquivo de imagem e o tipo de imagem, como mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="8351b-247">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="8351b-248">Você pode fazer [solicitações GET separadas a pontos de extremidade de recurso de imagem](../api-reference/v1.0/api/resource_get.md) para recuperar os respectivos conteúdos binários.</span><span class="sxs-lookup"><span data-stu-id="8351b-248">You can make separate [GET requests to image resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```http
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="8351b-249">Por padrão, as imagens não serão renderizadas diretamente em um navegador, pois elas são privadas e é necessária autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="8351b-249">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span> <span data-ttu-id="8351b-250">Para obter URLs públicas para os recursos de imagem em uma página, inclua **preAuthenticated=true** na cadeia de caracteres de consulta ao recuperar o conteúdo da página (exemplo: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="8351b-250">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="8351b-251">As URLs públicas que são retornadas são válidas por uma hora.</span><span class="sxs-lookup"><span data-stu-id="8351b-251">The public URLs that are returned are valid for one hour.</span></span> 

<span data-ttu-id="8351b-252">**Imagem com URL pública quando _preAuthenticated=true_ é incluído na solicitação**</span><span class="sxs-lookup"><span data-stu-id="8351b-252">**Image with public URL when _preAuthenticated=true_ is included in the request**</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}" />
```

<span data-ttu-id="8351b-253">Os exemplos a seguir mostram as informações que um elemento **img** pode conter no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-253">The following examples show the information an **img** element might contain in the output HTML.</span></span>

<span data-ttu-id="8351b-254">**Imagem com recursos de resolução alta e prontos para Web**</span><span class="sxs-lookup"><span data-stu-id="8351b-254">**Image with web-ready and high resolution resources**</span></span>

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

<span data-ttu-id="8351b-255">**Imagem criada usando o atributo *data-render-src* **</span><span class="sxs-lookup"><span data-stu-id="8351b-255">**Image created by using the *data-render-src* attribute**</span></span>

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

### <a name="split-images"></a><span data-ttu-id="8351b-256">Dividir imagens</span><span class="sxs-lookup"><span data-stu-id="8351b-256">Split images</span></span>

<span data-ttu-id="8351b-257">As imagens que são criadas usando o atributo **data-render-src** (de uma URL de página da Web ou de uma parte nomeada) podem ser divididas em várias imagens de componente por motivos de desempenho e renderização.</span><span class="sxs-lookup"><span data-stu-id="8351b-257">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons.</span></span> <span data-ttu-id="8351b-258">Todas as imagens de componente recebem o mesmo valor de **data-id**.</span><span class="sxs-lookup"><span data-stu-id="8351b-258">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="8351b-259">Cada imagem de componente tem um atributo de índice por dados com base zero que define o layout vertical original.</span><span class="sxs-lookup"><span data-stu-id="8351b-259">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

<span data-ttu-id="8351b-260">**Dividir imagem com três imagens de componente**</span><span class="sxs-lookup"><span data-stu-id="8351b-260">**Split image with three component images**</span></span>

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

<span data-ttu-id="8351b-261">Como os usuários podem mover as imagens na página, os índices retornados podem estar fora de ordem.</span><span class="sxs-lookup"><span data-stu-id="8351b-261">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="8351b-262">A ordenação deve estar na ordem y de cima para baixo e, na ordem x da esquerda para a direita, se houver conflitos na ordem y.</span><span class="sxs-lookup"><span data-stu-id="8351b-262">Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="8351b-263">Elementos iframe</span><span class="sxs-lookup"><span data-stu-id="8351b-263">iframe elements</span></span>
<span data-ttu-id="8351b-264">As páginas do OneNote podem conter vídeos inseridos representados pelos elementos **iframe**.</span><span class="sxs-lookup"><span data-stu-id="8351b-264">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

><span data-ttu-id="8351b-265">**Observação:** você também pode [anexar um arquivo de vídeo usando um elemento **object**](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files).</span><span class="sxs-lookup"><span data-stu-id="8351b-265">**Note:** You can also [attach a video file using an **object** element](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files).</span></span>

<span data-ttu-id="8351b-266">**Atributos de entrada**</span><span class="sxs-lookup"><span data-stu-id="8351b-266">**Input attributes**</span></span>

|<span data-ttu-id="8351b-267">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="8351b-267">Input attribute</span></span>|<span data-ttu-id="8351b-268">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-268">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-269">data-original-src</span><span class="sxs-lookup"><span data-stu-id="8351b-269">data-original-src</span></span> | <span data-ttu-id="8351b-270">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8351b-270">Required.</span></span> <span data-ttu-id="8351b-271">A URL da fonte do vídeo.</span><span class="sxs-lookup"><span data-stu-id="8351b-271">The URL of the video source.</span></span> <span data-ttu-id="8351b-272">Veja a [lista de fontes de vídeo com suporte](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span><span class="sxs-lookup"><span data-stu-id="8351b-272">See the [list of supported video sources](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span></span> <span data-ttu-id="8351b-273">Exemplo: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="8351b-273">Example`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="8351b-274">width, height</span><span class="sxs-lookup"><span data-stu-id="8351b-274">width, height</span></span> | <span data-ttu-id="8351b-275">A largura ou altura do iframe, em pixels.</span><span class="sxs-lookup"><span data-stu-id="8351b-275">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="8351b-276">Exemplo: `width=300`</span><span class="sxs-lookup"><span data-stu-id="8351b-276">Example`width=300`</span></span> |

<span data-ttu-id="8351b-277">**Atributos de saída**</span><span class="sxs-lookup"><span data-stu-id="8351b-277">**Output attributes**</span></span>

|<span data-ttu-id="8351b-278">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="8351b-278">Output attribute</span></span>|<span data-ttu-id="8351b-279">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-279">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-280">data-original-src</span><span class="sxs-lookup"><span data-stu-id="8351b-280">data-original-src</span></span> | <span data-ttu-id="8351b-281">A URL da fonte do vídeo.</span><span class="sxs-lookup"><span data-stu-id="8351b-281">The URL of the video source.</span></span> |
| <span data-ttu-id="8351b-282">src</span><span class="sxs-lookup"><span data-stu-id="8351b-282">Src</span></span> | <span data-ttu-id="8351b-283">O link para o vídeo que é inserido na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="8351b-283">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="8351b-284">width, height</span><span class="sxs-lookup"><span data-stu-id="8351b-284">width, height</span></span> | <span data-ttu-id="8351b-285">A largura ou altura do iframe, em pixels.</span><span class="sxs-lookup"><span data-stu-id="8351b-285">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="8351b-286">Exemplo: `width=300`</span><span class="sxs-lookup"><span data-stu-id="8351b-286">Example`width=300`</span></span> |
 
<span data-ttu-id="8351b-287">Exemplo de **HTML de saída** para vídeos</span><span class="sxs-lookup"><span data-stu-id="8351b-287">**Output HTML** example for videos</span></span>

<span data-ttu-id="8351b-288">Os elementos **iframe** de saída contêm pontos de extremidade que se vinculam à página e ao vídeo da fonte, como mostrado.</span><span class="sxs-lookup"><span data-stu-id="8351b-288">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="8351b-289">Elementos object</span><span class="sxs-lookup"><span data-stu-id="8351b-289">Object elements</span></span>
<span data-ttu-id="8351b-290">As páginas do OneNote contêm anexos de arquivo representados pelos elementos **object**.</span><span class="sxs-lookup"><span data-stu-id="8351b-290">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="8351b-291">Um elemento **object** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-291">An **object** element can contain the following attributes in the input and output HTML.</span></span>

><span data-ttu-id="8351b-292">**Observação:** As APIs do OneNote também podem renderizar conteúdo de arquivo como imagens em uma página quando o arquivo é enviado como uma imagem e usa o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="8351b-292">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span> <span data-ttu-id="8351b-293">Exemplo: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="8351b-293">Example`<img data-render-src="name:part-name" ... />`</span></span>
 

<span data-ttu-id="8351b-294">**Atributos de entrada**</span><span class="sxs-lookup"><span data-stu-id="8351b-294">**Input attributes**</span></span>

|<span data-ttu-id="8351b-295">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="8351b-295">Input attribute</span></span>|<span data-ttu-id="8351b-296">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-296">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-297">data</span><span class="sxs-lookup"><span data-stu-id="8351b-297">data</span></span> | <span data-ttu-id="8351b-298">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8351b-298">Required.</span></span> <span data-ttu-id="8351b-299">O nome da parte que representa o arquivo na [solicitação de partes múltiplas](../api-reference/v1.0/api/section_post_pages.md#example).</span><span class="sxs-lookup"><span data-stu-id="8351b-299">The name of the part that represents the file in the [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span> |
| <span data-ttu-id="8351b-300">data-attachment</span><span class="sxs-lookup"><span data-stu-id="8351b-300">data-attachment</span></span> | <span data-ttu-id="8351b-301">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8351b-301">Required.</span></span> <span data-ttu-id="8351b-302">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8351b-302">The file name.</span></span> |
| <span data-ttu-id="8351b-303">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-303">data-id</span></span> | <span data-ttu-id="8351b-304">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-304">A reference for the element.</span></span> <span data-ttu-id="8351b-305">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-305">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-306">style</span><span class="sxs-lookup"><span data-stu-id="8351b-306">style</span></span> | <p><span data-ttu-id="8351b-307">As propriedades de posição e tamanho para o objeto: **position** (somente **absolute**), **left**, **top** e **width**.</span><span class="sxs-lookup"><span data-stu-id="8351b-307">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span></p><p><span data-ttu-id="8351b-308">Usado para criar um objeto [posicionado absoluto](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos), somente se o objeto for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="8351b-308">Used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="8351b-309">Exemplo: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="8351b-309">Example`<object style="position:absolute;top:350px;left:300px" ... />`</span></span></p> |
| <span data-ttu-id="8351b-310">type</span><span class="sxs-lookup"><span data-stu-id="8351b-310">type</span></span> | <span data-ttu-id="8351b-311">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8351b-311">Required.</span></span> <span data-ttu-id="8351b-312">O tipo de arquivo de mídia padrão.</span><span class="sxs-lookup"><span data-stu-id="8351b-312">The standard media file type.</span></span> <span data-ttu-id="8351b-313">Os tipos de arquivo conhecidos exibem o ícone associado ao tipo de arquivo na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="8351b-313">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="8351b-314">Os tipos de arquivo desconhecidos exibem um ícone de arquivo genérico.</span><span class="sxs-lookup"><span data-stu-id="8351b-314">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

<span data-ttu-id="8351b-315">**Atributos de saída**</span><span class="sxs-lookup"><span data-stu-id="8351b-315">**Output attributes**</span></span>

|<span data-ttu-id="8351b-316">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="8351b-316">Output attribute</span></span>|<span data-ttu-id="8351b-317">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-317">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-318">data</span><span class="sxs-lookup"><span data-stu-id="8351b-318">data</span></span> | <span data-ttu-id="8351b-319">O ponto de extremidade para o recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="8351b-319">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="8351b-320">data-attachment</span><span class="sxs-lookup"><span data-stu-id="8351b-320">data-attachment</span></span> | <span data-ttu-id="8351b-321">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8351b-321">The file name.</span></span> |
| <span data-ttu-id="8351b-322">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-322">data-id</span></span> | <span data-ttu-id="8351b-323">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-323">A reference for the element.</span></span> <span data-ttu-id="8351b-324">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-324">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-325">id</span><span class="sxs-lookup"><span data-stu-id="8351b-325">id</span></span> | <span data-ttu-id="8351b-326">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-326">A unique ID for the group.</span></span> <span data-ttu-id="8351b-327">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="8351b-327">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="8351b-328">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-328">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-329">style</span><span class="sxs-lookup"><span data-stu-id="8351b-329">style</span></span> | <span data-ttu-id="8351b-330">As propriedades de posição do objeto.</span><span class="sxs-lookup"><span data-stu-id="8351b-330">The position properties of the object.</span></span> |
| <span data-ttu-id="8351b-331">type</span><span class="sxs-lookup"><span data-stu-id="8351b-331">type</span></span> | <span data-ttu-id="8351b-332">O tipo de arquivo de mídia padrão.</span><span class="sxs-lookup"><span data-stu-id="8351b-332">The standard media file type.</span></span> |
 

<span data-ttu-id="8351b-333">Exemplo de **HTML de saída** para objetos</span><span class="sxs-lookup"><span data-stu-id="8351b-333">**Output HTML** example for objects</span></span>

<span data-ttu-id="8351b-334">Os elementos **object** de saída contêm pontos de extremidade que se vinculam aos recursos de arquivo na página, como mostrado.</span><span class="sxs-lookup"><span data-stu-id="8351b-334">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="8351b-335">Você pode fazer [solicitações GET separadas a pontos de extremidade de recurso de arquivo](../api-reference/v1.0/api/resource_get.md) para recuperar os respectivos conteúdos binários.</span><span class="sxs-lookup"><span data-stu-id="8351b-335">You can make separate [GET requests to file resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="8351b-336">Parágrafos e cabeçalhos</span><span class="sxs-lookup"><span data-stu-id="8351b-336">Paragraphs and headings</span></span>

<span data-ttu-id="8351b-337">Os parágrafos, cabeçalhos e outros contêineres de texto podem incluir os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-337">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="8351b-338">**Atributos de entrada**</span><span class="sxs-lookup"><span data-stu-id="8351b-338">**Input attributes**</span></span>

|<span data-ttu-id="8351b-339">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="8351b-339">Input attribute</span></span>|<span data-ttu-id="8351b-340">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-340">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-341">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-341">data-id</span></span> | <span data-ttu-id="8351b-342">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-342">A reference for the element.</span></span> <span data-ttu-id="8351b-343">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-343">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-344">data-tag</span><span class="sxs-lookup"><span data-stu-id="8351b-344">data-tag</span></span> | <span data-ttu-id="8351b-345">Uma [marca de anotação](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) em um elemento **p** ou **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="8351b-345">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="8351b-346">style</span><span class="sxs-lookup"><span data-stu-id="8351b-346">style</span></span> | <span data-ttu-id="8351b-347">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-347">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="8351b-348">**Atributos de saída**</span><span class="sxs-lookup"><span data-stu-id="8351b-348">**Output attributes**</span></span>

|<span data-ttu-id="8351b-349">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="8351b-349">Output attribute</span></span>|<span data-ttu-id="8351b-350">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-350">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-351">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-351">data-id</span></span> | <span data-ttu-id="8351b-352">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-352">A reference for the element.</span></span> <span data-ttu-id="8351b-353">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-353">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-354">data-tag</span><span class="sxs-lookup"><span data-stu-id="8351b-354">data-tag</span></span> | <span data-ttu-id="8351b-355">Uma [marca de anotação](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) em um elemento **p** ou **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="8351b-355">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="8351b-356">id</span><span class="sxs-lookup"><span data-stu-id="8351b-356">id</span></span> | <span data-ttu-id="8351b-357">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-357">A unique ID for the group.</span></span> <span data-ttu-id="8351b-358">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="8351b-358">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="8351b-359">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-359">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-360">style</span><span class="sxs-lookup"><span data-stu-id="8351b-360">style</span></span> | <span data-ttu-id="8351b-361">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-361">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="8351b-362">No HTML de saída, esses valores podem ser retornados embutidos em elementos filho apropriados ou em elementos **span**.</span><span class="sxs-lookup"><span data-stu-id="8351b-362">In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="8351b-363">Os exemplos a seguir mostram HTML de entrada que usa maneiras diferentes de definir estilos em contêineres de texto e o HTML de saída que é retornado.</span><span class="sxs-lookup"><span data-stu-id="8351b-363">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

<span data-ttu-id="8351b-364">**HTML de entrada** com estilos definidos usando estilos de caractere embutidos, na marca de início, e dentro de um elemento **span**.</span><span class="sxs-lookup"><span data-stu-id="8351b-364">**Input HTML** with styles defined using inline character styles, in the start tag, and within a **span** element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

<span data-ttu-id="8351b-365">**Saída HTML** com o estilo de caractere `<i>` e as configurações de fonte na marca de início `<p>` retornadas como estilos CSS embutidos em elementos **span**.</span><span class="sxs-lookup"><span data-stu-id="8351b-365">**Output HTML** with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on **span** elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="8351b-366">Listas</span><span class="sxs-lookup"><span data-stu-id="8351b-366">Lists</span></span>
<span data-ttu-id="8351b-367">As listas são representadas como elementos **ol** ou **ul** que contêm itens de lista representados como elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="8351b-367">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="8351b-368">Listas e itens de lista podem conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-368">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="8351b-369">**Atributos de entrada**</span><span class="sxs-lookup"><span data-stu-id="8351b-369">**Input attributes**</span></span>

|<span data-ttu-id="8351b-370">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="8351b-370">Input attribute</span></span>|<span data-ttu-id="8351b-371">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-371">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-372">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-372">data-id</span></span> | <span data-ttu-id="8351b-373">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-373">A reference for the element.</span></span> <span data-ttu-id="8351b-374">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-374">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-375">data-tag</span><span class="sxs-lookup"><span data-stu-id="8351b-375">data-tag</span></span> | <span data-ttu-id="8351b-376">Uma [marca de anotação](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) em um elemento **ul**, **ol** ou **li**.</span><span class="sxs-lookup"><span data-stu-id="8351b-376">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="8351b-377">style</span><span class="sxs-lookup"><span data-stu-id="8351b-377">style</span></span> | <span data-ttu-id="8351b-378">O **list-style-type** e as propriedades [style](#styles) do CSS para a lista ou o item de lista.</span><span class="sxs-lookup"><span data-stu-id="8351b-378">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

<span data-ttu-id="8351b-379">**Atributos de saída**</span><span class="sxs-lookup"><span data-stu-id="8351b-379">**Output attributes**</span></span>

|<span data-ttu-id="8351b-380">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="8351b-380">Output attribute</span></span>|<span data-ttu-id="8351b-381">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-381">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-382">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-382">data-id</span></span> | <span data-ttu-id="8351b-383">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-383">A reference for the element.</span></span> <span data-ttu-id="8351b-384">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-384">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-385">data-tag</span><span class="sxs-lookup"><span data-stu-id="8351b-385">data-tag</span></span> |  <span data-ttu-id="8351b-386">Uma [marca de anotação](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) em um período em um elemento **li**.</span><span class="sxs-lookup"><span data-stu-id="8351b-386">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a span in a **li** element.</span></span> |
| <span data-ttu-id="8351b-387">id</span><span class="sxs-lookup"><span data-stu-id="8351b-387">id</span></span> | <span data-ttu-id="8351b-388">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-388">A unique ID for the group.</span></span> <span data-ttu-id="8351b-389">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="8351b-389">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="8351b-390">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-390">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-391">style</span><span class="sxs-lookup"><span data-stu-id="8351b-391">style</span></span> | <span data-ttu-id="8351b-392">O **list-style-type** e as propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-392">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="8351b-393">No HTML de saída, as configurações no nível de lista são retornadas em itens de lista.</span><span class="sxs-lookup"><span data-stu-id="8351b-393">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="8351b-394">As propriedades padrão não são retornadas.</span><span class="sxs-lookup"><span data-stu-id="8351b-394">The following properties are not returned:</span></span> |
 

<span data-ttu-id="8351b-395">As APIs do OneNote no Microsoft Graph dão suporte aos seguintes estilos de lista:</span><span class="sxs-lookup"><span data-stu-id="8351b-395">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="8351b-396">Lista ordenada</span><span class="sxs-lookup"><span data-stu-id="8351b-396">Ordered list</span></span>|<span data-ttu-id="8351b-397">Lista não ordenada</span><span class="sxs-lookup"><span data-stu-id="8351b-397">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-398">none</span><span class="sxs-lookup"><span data-stu-id="8351b-398">none</span></span> | <span data-ttu-id="8351b-399">none</span><span class="sxs-lookup"><span data-stu-id="8351b-399">none</span></span> |
| <span data-ttu-id="8351b-400">decimal (default)</span><span class="sxs-lookup"><span data-stu-id="8351b-400">decimal (default)</span></span> | <span data-ttu-id="8351b-401">disc (default)</span><span class="sxs-lookup"><span data-stu-id="8351b-401">disc (default)</span></span> |
| <span data-ttu-id="8351b-402">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="8351b-402">lower-alpha</span></span> | <span data-ttu-id="8351b-403">circle</span><span class="sxs-lookup"><span data-stu-id="8351b-403">Circle.</span></span> |
| <span data-ttu-id="8351b-404">lower-roman</span><span class="sxs-lookup"><span data-stu-id="8351b-404">lower-roman</span></span> | <span data-ttu-id="8351b-405">square</span><span class="sxs-lookup"><span data-stu-id="8351b-405">Square.</span></span> |
| <span data-ttu-id="8351b-406">upper-alpha</span><span class="sxs-lookup"><span data-stu-id="8351b-406">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="8351b-407">upper-roman</span><span class="sxs-lookup"><span data-stu-id="8351b-407">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="8351b-408">Você pode aplicar estilos globais para uma lista no elemento **ol** ou **ul** no HTML de entrada, mas estilos são retornados nos elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="8351b-408">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

<span data-ttu-id="8351b-409">**Estilo de lista homogêneo**</span><span class="sxs-lookup"><span data-stu-id="8351b-409">**Homogenous list style**</span></span>

<span data-ttu-id="8351b-410">Este exemplo mostra o HTML de entrada que define o tipo de estilo de lista no elemento **ol** e estilos CSS em itens de lista individuais.</span><span class="sxs-lookup"><span data-stu-id="8351b-410">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="8351b-411">Este é o HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-411">This is the output HTML.</span></span> <span data-ttu-id="8351b-412">Observe que os estilos são retornados embutidos nos elementos **li** ou **span** individuais.</span><span class="sxs-lookup"><span data-stu-id="8351b-412">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

<span data-ttu-id="8351b-413">**Estilos de lista variáveis**</span><span class="sxs-lookup"><span data-stu-id="8351b-413">**Variable list styles**</span></span>

<span data-ttu-id="8351b-414">Este exemplo mostra o HTML de entrada que define diferentes tipos de estilo de lista nos elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="8351b-414">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="8351b-415">Este é o HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-415">This is the output HTML.</span></span> <span data-ttu-id="8351b-416">Observe que os estilos são retornados embutidos nos elementos **li** ou **span** individuais.</span><span class="sxs-lookup"><span data-stu-id="8351b-416">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="8351b-417">Tabelas</span><span class="sxs-lookup"><span data-stu-id="8351b-417">Tables</span></span>
<span data-ttu-id="8351b-418">As tabelas são representadas como elementos **table** que podem conter elementos **tr** e **td**.</span><span class="sxs-lookup"><span data-stu-id="8351b-418">Tables are represented as **table** elements that can contain **tr** and **td** elements.</span></span> <span data-ttu-id="8351b-419">Há suporte para tabelas aninhadas.</span><span class="sxs-lookup"><span data-stu-id="8351b-419">Nested tables are supported.</span></span>

<span data-ttu-id="8351b-420">As tabelas podem conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="8351b-420">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="8351b-421">As APIs do OneNote não dão suporte aos atributos **rowspan** ou **colspan**.</span><span class="sxs-lookup"><span data-stu-id="8351b-421">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

<span data-ttu-id="8351b-422">**Atributos de entrada**</span><span class="sxs-lookup"><span data-stu-id="8351b-422">**Input attributes**</span></span>

|<span data-ttu-id="8351b-423">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="8351b-423">Input attribute</span></span>|<span data-ttu-id="8351b-424">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-424">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-425">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-425">data-id</span></span> | <span data-ttu-id="8351b-426">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-426">A reference for the element.</span></span> <span data-ttu-id="8351b-427">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-427">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-428">style</span><span class="sxs-lookup"><span data-stu-id="8351b-428">style</span></span> | <span data-ttu-id="8351b-429">As propriedades [style](#styles) do CSS do elemento e também:</span><span class="sxs-lookup"><span data-stu-id="8351b-429">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="8351b-430">- **border**.</span><span class="sxs-lookup"><span data-stu-id="8351b-430">Border</span></span> <span data-ttu-id="8351b-431">Pode ser 0px ou 1px.</span><span class="sxs-lookup"><span data-stu-id="8351b-431">Can be either 0px or 1px.</span></span><br /> <span data-ttu-id="8351b-432">- **width**.</span><span class="sxs-lookup"><span data-stu-id="8351b-432">width</span></span> <span data-ttu-id="8351b-433">Com suporte de **table** e **td** como pixels ou porcentagem de largura da página.</span><span class="sxs-lookup"><span data-stu-id="8351b-433">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br /><span data-ttu-id="8351b-434">Exemplo: `width="100px"` ou `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="8351b-434">Example: `width="100px"` or `width="60%"`</span></span> |
 

<span data-ttu-id="8351b-435">**Atributos de saída**</span><span class="sxs-lookup"><span data-stu-id="8351b-435">**Output attributes**</span></span>

|<span data-ttu-id="8351b-436">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="8351b-436">Output attribute</span></span>|<span data-ttu-id="8351b-437">Descrição</span><span class="sxs-lookup"><span data-stu-id="8351b-437">Description</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-438">data-id</span><span class="sxs-lookup"><span data-stu-id="8351b-438">data-id</span></span> | <span data-ttu-id="8351b-439">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-439">A reference for the element.</span></span> <span data-ttu-id="8351b-440">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-440">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-441">id</span><span class="sxs-lookup"><span data-stu-id="8351b-441">id</span></span> | <span data-ttu-id="8351b-442">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-442">A unique ID for the group.</span></span> <span data-ttu-id="8351b-443">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](../api-reference/v1.0/api/page_get.md) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="8351b-443">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="8351b-444">Usado para [atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-444">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="8351b-445">style</span><span class="sxs-lookup"><span data-stu-id="8351b-445">style</span></span> | <span data-ttu-id="8351b-446">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="8351b-446">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="8351b-447">Os exemplos a seguir mostram HTML de entrada que usa maneiras diferentes de definir estilos em tabelas e o HTML de saída que é retornado.</span><span class="sxs-lookup"><span data-stu-id="8351b-447">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

<span data-ttu-id="8351b-448">**HTML de entrada** com configurações opcionais em níveis diferentes.</span><span class="sxs-lookup"><span data-stu-id="8351b-448">**Input HTML** with optional settings at different levels.</span></span>

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
 
<span data-ttu-id="8351b-449">**HTML de saída** com estilos CSS retornados embutidos nos elementos **td**.</span><span class="sxs-lookup"><span data-stu-id="8351b-449">**Output HTML** with CSS styles returned inline on the **td** elements.</span></span>

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


## <a name="styles"></a><span data-ttu-id="8351b-450">Estilos</span><span class="sxs-lookup"><span data-stu-id="8351b-450">Styles</span></span>
<span data-ttu-id="8351b-451">As APIs do OneNote no Microsoft Graph dão suporte as propriedades **style** do CSS embutidas a seguir para elementos no corpo da página, como **body**, **div**, **p**, **li** e **span**.</span><span class="sxs-lookup"><span data-stu-id="8351b-451">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="8351b-452">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8351b-452">Property</span></span>|<span data-ttu-id="8351b-453">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8351b-453">Example</span></span>|
|:------|:------|
| <span data-ttu-id="8351b-454">background-color</span><span class="sxs-lookup"><span data-stu-id="8351b-454">background-color</span></span> | <span data-ttu-id="8351b-455">`style="background-color:#66cc66"` (o padrão é branco)</span><span class="sxs-lookup"><span data-stu-id="8351b-455">`style="background-color:#66cc66"` (defaults to white)</span></span><br /><span data-ttu-id="8351b-456">Há suporte para cores nomeadas e formato hexadecimal.</span><span class="sxs-lookup"><span data-stu-id="8351b-456">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="8351b-457">color</span><span class="sxs-lookup"><span data-stu-id="8351b-457">color</span></span> | <span data-ttu-id="8351b-458">`style="color:#ffffff"` (o padrão é preto)</span><span class="sxs-lookup"><span data-stu-id="8351b-458">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="8351b-459">font-family</span><span class="sxs-lookup"><span data-stu-id="8351b-459">font-family</span></span> | <span data-ttu-id="8351b-460">`style="font-family:Courier"` (o padrão é Calibri)</span><span class="sxs-lookup"><span data-stu-id="8351b-460">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="8351b-461">font-size</span><span class="sxs-lookup"><span data-stu-id="8351b-461">FontSize</span></span> | <span data-ttu-id="8351b-462">`style="font-size:10pt"` (o padrão é 11pt)</span><span class="sxs-lookup"><span data-stu-id="8351b-462">`style="font-size:10pt"` (defaults to 11pt)</span></span><br /><span data-ttu-id="8351b-463">As APIs aceitam o tamanho da fonte em *pt* ou *px*, mas converte *px* em *pt*.</span><span class="sxs-lookup"><span data-stu-id="8351b-463">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="8351b-464">Valores decimais são arredondados para o n,0pt ou n,5pt mais próximo.</span><span class="sxs-lookup"><span data-stu-id="8351b-464">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="8351b-465">font-style</span><span class="sxs-lookup"><span data-stu-id="8351b-465">font-style</span></span> | <span data-ttu-id="8351b-466">`style="font-style:italic"` (somente normal ou itálico)</span><span class="sxs-lookup"><span data-stu-id="8351b-466">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="8351b-467">font-weight</span><span class="sxs-lookup"><span data-stu-id="8351b-467">FontWeight</span></span> | <span data-ttu-id="8351b-468">`style="font-weight:bold"` (somente normal ou negrito)</span><span class="sxs-lookup"><span data-stu-id="8351b-468">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="8351b-469">strike-through</span><span class="sxs-lookup"><span data-stu-id="8351b-469">Strikethrough</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="8351b-470">text-align</span><span class="sxs-lookup"><span data-stu-id="8351b-470">text-align</span></span> | <span data-ttu-id="8351b-471">`style="text-align:center"` (somente para elementos de bloco)</span><span class="sxs-lookup"><span data-stu-id="8351b-471">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="8351b-472">text-decoration</span><span class="sxs-lookup"><span data-stu-id="8351b-472">text-decoration</span></span> | <span data-ttu-id="8351b-473">`style="text-decoration:underline"` (somente nenhum ou sublinhado)</span><span class="sxs-lookup"><span data-stu-id="8351b-473">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="8351b-474">Os seguintes estilos de caractere embutidos e também têm suporte:</span><span class="sxs-lookup"><span data-stu-id="8351b-474">The following inline character styles and are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="8351b-475">&lt;b&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-475">b.</span></span></td>
<td id="simplecell"><span data-ttu-id="8351b-476">&lt;i&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-476">I</span></span></td>
<td id="simplecell"><span data-ttu-id="8351b-477">&lt;u&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-477">U</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="8351b-478">&lt;em&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-478">
EM 
</span></span></td>
<td id="simplecell"><span data-ttu-id="8351b-479">&lt;strong&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-479">Strong.</span></span></td>
<td id="simplecell"><span data-ttu-id="8351b-480">&lt;strike&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-480">&lt;strike&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="8351b-481">&lt;sup&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-481">Scr sup.</span></span></td>
<td id="simplecell"><span data-ttu-id="8351b-482">&lt;sub&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-482">&lt;Sub&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="8351b-483">&lt;del&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-483">&lt;del&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="8351b-484">&lt;cite&gt;</span><span class="sxs-lookup"><span data-stu-id="8351b-484">&lt;cite&gt;</span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="8351b-485">Exemplo de HTML de entrada e saída</span><span class="sxs-lookup"><span data-stu-id="8351b-485">Input and output HTML example</span></span>
<span data-ttu-id="8351b-486">A imagem a seguir mostra uma página simples que foi criada com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8351b-486">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Imagem de uma página do OneNote com notas de conteúdo do estudo da Wikipédia](images/onenote-sample-image.png)

<span data-ttu-id="8351b-488">Este é o HTML de entrada enviado no corpo da mensagem para criar a página.</span><span class="sxs-lookup"><span data-stu-id="8351b-488">This is the input HTML sent in the message body to create the page.</span></span>

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

<span data-ttu-id="8351b-489">Este é o HTML de saída que o Microsoft Graph retorna quando você [obtém o conteúdo da página](../api-reference/v1.0/api/page_get.md).</span><span class="sxs-lookup"><span data-stu-id="8351b-489">This is the output HTML that Microsoft Graph returns when you [get page content](../api-reference/v1.0/api/page_get.md).</span></span>

><span data-ttu-id="8351b-490">**Observação:** quando você [cria uma página](../api-reference/v1.0/api/section_post_pages.md) ou [obtém metadados de página](../api-reference/v1.0/api/page_get.md), a API retorna a URL de ponto de extremidade do *conteúdo* da página na propriedade **contentUrl**.</span><span class="sxs-lookup"><span data-stu-id="8351b-490">**Note:** When you [create a page](../api-reference/v1.0/api/section_post_pages.md) or [get page metadata](../api-reference/v1.0/api/page_get.md), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8351b-491">Confira também</span><span class="sxs-lookup"><span data-stu-id="8351b-491">See also</span></span>

- [<span data-ttu-id="8351b-492">Obter a estrutura e o conteúdo do OneNote</span><span class="sxs-lookup"><span data-stu-id="8351b-492">Get OneNote content and structure</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="8351b-493">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="8351b-493">Create OneNote pages</span></span>](../api-reference/v1.0/api/section_post_pages.md)
- [<span data-ttu-id="8351b-494">Atualizar conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="8351b-494">Update page content</span></span>](../api-reference/v1.0/api/page_update.md)
- [<span data-ttu-id="8351b-495">Adicionar imagens e arquivos</span><span class="sxs-lookup"><span data-stu-id="8351b-495">Add images and files</span></span>](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)
