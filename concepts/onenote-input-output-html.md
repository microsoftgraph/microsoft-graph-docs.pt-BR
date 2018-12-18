---
title: HTML de entrada e saída nas páginas do OneNote
description: 'O HTML que define o conteúdo e a estrutura da página quando você cria ou atualiza uma página do OneNote é chamado de *HTML de entrada*. '
author: Jewan-microsoft
ms.openlocfilehash: e169cf17804794d5120b2e968328b06d29a0a5a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351251"
---
# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="59c54-103">HTML de entrada e saída nas páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="59c54-103">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="59c54-104">O HTML que define o conteúdo e a estrutura da página quando você [cria](onenote-create-page.md) ou [atualiza](onenote-update-page.md) uma página do OneNote é chamado de *HTML de entrada*.</span><span class="sxs-lookup"><span data-stu-id="59c54-104">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote-update-page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="59c54-105">O HTML que é retornado quando você [obtém o conteúdo da página](onenote-get-content.md) é chamado de *HTML de saída*.</span><span class="sxs-lookup"><span data-stu-id="59c54-105">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*.</span></span> <span data-ttu-id="59c54-106">O HTML de saída não será igual ao HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="59c54-106">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="59c54-107">As APIs do OneNote no Microsoft Graph preservam o conteúdo semântico e a estrutura básica do HTML de entrada, mas os convertem em um conjunto de [elementos HTML e propriedades CSS com suporte](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="59c54-107">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="59c54-108">As APIs também adicionam atributos personalizados que dão suporte a recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="59c54-108">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="59c54-109">Este artigo descreve os principais elementos e atributos do HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-109">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="59c54-110">Pode ser útil entender o HTML de entrada quando você estiver criando ou atualizando o conteúdo da página e o HTML de saída quando estiver analisando o conteúdo da página retornado.</span><span class="sxs-lookup"><span data-stu-id="59c54-110">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="59c54-111">Elemento body</span><span class="sxs-lookup"><span data-stu-id="59c54-111">body element</span></span>

<span data-ttu-id="59c54-112">O conteúdo HTML no corpo da página representa o conteúdo e a estrutura da página, inclusive os recursos de imagem e arquivo.</span><span class="sxs-lookup"><span data-stu-id="59c54-112">The HTML content in the page body represents the page content and structure, including image and file resources.</span></span> <span data-ttu-id="59c54-113">O elemento **body** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-113">The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="59c54-114">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-114">Input attributes</span></span>

|<span data-ttu-id="59c54-115">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-115">Input attribute</span></span>|<span data-ttu-id="59c54-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-116">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-117">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="59c54-117">data-absolute-enabled</span></span> | <span data-ttu-id="59c54-118">Indica se o corpo da entrada dá suporte a elementos [posicionados absolutos](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-118">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="59c54-119">style</span><span class="sxs-lookup"><span data-stu-id="59c54-119">style</span></span> | <p><span data-ttu-id="59c54-120">As propriedades [style](#styles) do CSS do corpo.</span><span class="sxs-lookup"><span data-stu-id="59c54-120">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="59c54-121">No HTML de saída, as configurações de entrada podem ser retornadas embutidas em elementos filho apropriados.</span><span class="sxs-lookup"><span data-stu-id="59c54-121">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="59c54-122">Atualmente, a cor da tela de fundo não tem suporte para o elemento **body**.</span><span class="sxs-lookup"><span data-stu-id="59c54-122">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="59c54-123">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-123">Output attributes</span></span>

|<span data-ttu-id="59c54-124">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-124">Output attribute</span></span>|<span data-ttu-id="59c54-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-125">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-126">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="59c54-126">data-absolute-enabled</span></span> | <span data-ttu-id="59c54-127">Indica se o corpo dá suporte a elementos [posicionados absolutos](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-127">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> <span data-ttu-id="59c54-128">Sempre **true** no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-128">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="59c54-129">style</span><span class="sxs-lookup"><span data-stu-id="59c54-129">style</span></span> | <span data-ttu-id="59c54-130">As propriedades **font-family** e **font-size** do corpo.</span><span class="sxs-lookup"><span data-stu-id="59c54-130">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="59c54-131">Elementos Div</span><span class="sxs-lookup"><span data-stu-id="59c54-131">div elements</span></span>

<span data-ttu-id="59c54-132">Os elementos **Div** contêm texto, imagens e outros tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="59c54-132">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="59c54-133">Um elemento **div** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-133">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="59c54-134">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-134">Input attributes</span></span>

|<span data-ttu-id="59c54-135">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-135">Input attribute</span></span>|<span data-ttu-id="59c54-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-136">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-137">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-137">data-id</span></span> | <span data-ttu-id="59c54-138">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-138">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-139">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-139">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-140">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="59c54-140">data-render-fallback</span></span> | <span data-ttu-id="59c54-141">A ação de fallback se [extraction](onenote-extract-data.md) falhar: **render** (padrão) ou **none**</span><span class="sxs-lookup"><span data-stu-id="59c54-141">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**</span></span> |
| <span data-ttu-id="59c54-142">data-render-method</span><span class="sxs-lookup"><span data-stu-id="59c54-142">data-render-method</span></span> | <span data-ttu-id="59c54-143">O método [extraction](onenote-extract-data.md) a ser executado, por exemplo:</span><span class="sxs-lookup"><span data-stu-id="59c54-143">The [extraction](onenote-extract-data.md) method to perform, for example:</span></span><br/><span data-ttu-id="59c54-144">`extract.businesscard` ou `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="59c54-144">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="59c54-145">data-render-src</span><span class="sxs-lookup"><span data-stu-id="59c54-145">data-render-src</span></span> | <span data-ttu-id="59c54-146">A fonte de conteúdo para [extraction](onenote-extract-data.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-146">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="59c54-147">style</span><span class="sxs-lookup"><span data-stu-id="59c54-147">style</span></span> | <span data-ttu-id="59c54-148">As propriedades de posição, tamanho, fonte e cor para o div:</span><span class="sxs-lookup"><span data-stu-id="59c54-148">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="59c54-149">**posição** (**absoluto** somente), **esquerdo**, **superior** e **largura** (a altura é automaticamente configurada para divs)</span><span class="sxs-lookup"><span data-stu-id="59c54-149">**position** (**absolute** only), **left**, **top**, and **width** (height is auto-configured for divs)</span></span><br/><br/><span data-ttu-id="59c54-150">Usado para criar um div [posicionado absoluto](onenote-abs-pos.md), somente se o div for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="59c54-150">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="59c54-151">Exemplo: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="59c54-151">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="59c54-152">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-152">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="59c54-153">No HTML de saída, esses valores são retornados embutidos em elementos filho apropriados.</span><span class="sxs-lookup"><span data-stu-id="59c54-153">In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="59c54-154">As APIs do OneNote no Microsoft Graph encapsulam todo o conteúdo do corpo em pelo menos um div.</span><span class="sxs-lookup"><span data-stu-id="59c54-154">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="59c54-155">A API cria um div padrão (atribuído com `data-id="_default"`) para incluir o conteúdo do corpo se:</span><span class="sxs-lookup"><span data-stu-id="59c54-155">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="59c54-156">O atributo **data-absolute-enabled** do elemento body de entrada for omitido ou definido como **false**.</span><span class="sxs-lookup"><span data-stu-id="59c54-156">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**.</span></span> <span data-ttu-id="59c54-157">Nesse caso, todo o conteúdo do corpo é colocado no div padrão.</span><span class="sxs-lookup"><span data-stu-id="59c54-157">In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="59c54-158">O atributo **data-absolute-enabled** do elemento body de entrada for **true**, mas o HTML de entrada contiver filhos diretos que não são [elementos](onenote-abs-pos.md)&nbsp;**div**, **img** ou **object** posicionados de forma absoluta.</span><span class="sxs-lookup"><span data-stu-id="59c54-158">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="59c54-159">Nesse caso, os filhos diretos que não forem [elementos](onenote-abs-pos.md)&nbsp;**div**, **img** ou **object** posicionados de forma absoluta serão colocados no div padrão.</span><span class="sxs-lookup"><span data-stu-id="59c54-159">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="59c54-160">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-160">Output attributes</span></span>

|<span data-ttu-id="59c54-161">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-161">Output attribute</span></span>|<span data-ttu-id="59c54-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-162">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-163">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-163">data-id</span></span> | <span data-ttu-id="59c54-164">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-164">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-165">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-165">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-166">id</span><span class="sxs-lookup"><span data-stu-id="59c54-166">id</span></span> | <span data-ttu-id="59c54-167">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-167">A unique, generated ID for the element.</span></span> <span data-ttu-id="59c54-168">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="59c54-168">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="59c54-169">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-169">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-170">style</span><span class="sxs-lookup"><span data-stu-id="59c54-170">style</span></span> | <span data-ttu-id="59c54-171">As propriedades de tamanho e posição do div.</span><span class="sxs-lookup"><span data-stu-id="59c54-171">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="59c54-172">Divs não contribuintes</span><span class="sxs-lookup"><span data-stu-id="59c54-172">Non-contributing divs</span></span>

<span data-ttu-id="59c54-173">Quando um elemento **div** no HTML de entrada não contribui com a estrutura da página nem carrega informações usadas pelo OneNote, a API move o conteúdo do div para o div pai ou padrão.</span><span class="sxs-lookup"><span data-stu-id="59c54-173">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="59c54-174">Isso é ilustrado nos exemplos a seguir.</span><span class="sxs-lookup"><span data-stu-id="59c54-174">This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="59c54-175">HTML de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-175">Input HTML</span></span>

<span data-ttu-id="59c54-176">Contém um div aninhado não contribuinte.</span><span class="sxs-lookup"><span data-stu-id="59c54-176">Contains a non-contributing, nested div.</span></span>

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

#### <a name="output-html"></a><span data-ttu-id="59c54-177">HTML de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-177">Output HTML</span></span>

> <span data-ttu-id="59c54-178">**Observação**: o conteúdo do div foi movido para o div pai e as marcas `<div>` aninhadas foram removidas.</span><span class="sxs-lookup"><span data-stu-id="59c54-178">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="59c54-179">O div seria preservado se definisse qualquer informação semântica, como **data-id** (exemplo: `<div data-id="keep-me">`).</span><span class="sxs-lookup"><span data-stu-id="59c54-179">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
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


## <a name="img-elements"></a><span data-ttu-id="59c54-180">Elementos img</span><span class="sxs-lookup"><span data-stu-id="59c54-180">img elements</span></span>

<span data-ttu-id="59c54-181">Imagens em páginas do OneNote são representadas pelos elementos **img**.</span><span class="sxs-lookup"><span data-stu-id="59c54-181">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="59c54-182">Um elemento **img** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-182">An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="59c54-183">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-183">Input attributes</span></span>

|<span data-ttu-id="59c54-184">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-184">Input attribute</span></span>|<span data-ttu-id="59c54-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-185">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-186">alt</span><span class="sxs-lookup"><span data-stu-id="59c54-186">alt</span></span> | <span data-ttu-id="59c54-187">O texto Alt fornecido para a imagem.</span><span class="sxs-lookup"><span data-stu-id="59c54-187">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="59c54-188">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-188">data-id</span></span> | <span data-ttu-id="59c54-189">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-189">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-190">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-190">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-191">data-render-src</span><span class="sxs-lookup"><span data-stu-id="59c54-191">data-render-src</span></span> |<span data-ttu-id="59c54-192">Ou **data-render-src** ou **src** é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59c54-192">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="59c54-193">A página da Web a ser renderizada como uma imagem mapeada por bit na página do OneNote:</span><span class="sxs-lookup"><span data-stu-id="59c54-193">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="59c54-194">- `data-render-src="https://..."` para uma URL pública.</span><span class="sxs-lookup"><span data-stu-id="59c54-194">- `data-render-src="https://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="59c54-195">- `data-render-src="name:BlockName"` para parte de uma imagem no bloco "Apresentação" de uma [solicitação de partes múltiplas](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span><span class="sxs-lookup"><span data-stu-id="59c54-195">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span><br/><br/><span data-ttu-id="59c54-196">Esse método é útil quando a página da Web é mais complexa que a página que o OneNote pode renderizar fielmente ou quando a página exige credenciais de logon.</span><span class="sxs-lookup"><span data-stu-id="59c54-196">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="59c54-197">data-tag</span><span class="sxs-lookup"><span data-stu-id="59c54-197">data-tag</span></span> | <span data-ttu-id="59c54-198">Uma [marca de anotação](onenote-note-tags.md) no elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-198">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="59c54-199">style</span><span class="sxs-lookup"><span data-stu-id="59c54-199">style</span></span> |<span data-ttu-id="59c54-200">As propriedades de posição e tamanho para a imagem: **position** (somente **absolute**), **left**, **top**, **width** e **height**.</span><span class="sxs-lookup"><span data-stu-id="59c54-200">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="59c54-201">O tamanho pode ser definido em qualquer imagem.</span><span class="sxs-lookup"><span data-stu-id="59c54-201">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="59c54-202">As propriedades de posição serão usadas para criar uma imagem [posicionada absoluta](onenote-abs-pos.md), somente se a imagem for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="59c54-202">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="59c54-203">Exemplo: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="59c54-203">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="59c54-204">No HTML de saída, o tamanho da imagem é retornado separadamente nos atributos **width** e **height**.</span><span class="sxs-lookup"><span data-stu-id="59c54-204">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="59c54-205">src</span><span class="sxs-lookup"><span data-stu-id="59c54-205">src</span></span> |<span data-ttu-id="59c54-206">Ou **src** ou **data-render-src** é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59c54-206">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="59c54-207">A imagem a ser renderizada na página do OneNote:</span><span class="sxs-lookup"><span data-stu-id="59c54-207">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="59c54-208">- `src="https://..."` para uma URL para uma imagem publicamente disponível na Internet.</span><span class="sxs-lookup"><span data-stu-id="59c54-208">- `src="https://..."` for a URL to a publicly available image on the Internet.</span></span><br/><br/> <span data-ttu-id="59c54-209">- `src="name:BlockName"` para uma parte nomeada em uma solicitação de partes múltiplas que representa a imagem.</span><span class="sxs-lookup"><span data-stu-id="59c54-209">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="59c54-210">width, height</span><span class="sxs-lookup"><span data-stu-id="59c54-210">width, height</span></span> | <span data-ttu-id="59c54-211">A largura ou altura da imagem, em pixels, mas sem o px.</span><span class="sxs-lookup"><span data-stu-id="59c54-211">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="59c54-212">Exemplo: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="59c54-212">Example: `width="400"`</span></span> |
 
> <span data-ttu-id="59c54-213">**Observação:** as APIs do OneNote detectam automaticamente o tipo de imagem de entrada e o retornam como o **data-fullres-src-type** no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-213">**Note:** The OneNote APIs automatically detect the input image type, and return it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="59c54-214">A API também retorna o tipo de imagem da imagem otimizada em **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="59c54-214">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="59c54-215">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-215">Output attributes</span></span>

|<span data-ttu-id="59c54-216">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-216">Output attribute</span></span>|<span data-ttu-id="59c54-217">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-217">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-218">alt</span><span class="sxs-lookup"><span data-stu-id="59c54-218">alt</span></span> | <span data-ttu-id="59c54-219">O texto Alt fornecido para a imagem.</span><span class="sxs-lookup"><span data-stu-id="59c54-219">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="59c54-220">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-220">data-id</span></span> | <span data-ttu-id="59c54-221">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-221">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-222">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-222">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-223">data-index</span><span class="sxs-lookup"><span data-stu-id="59c54-223">data-index</span></span> | <span data-ttu-id="59c54-224">A posição da imagem.</span><span class="sxs-lookup"><span data-stu-id="59c54-224">The position of the image.</span></span> <span data-ttu-id="59c54-225">Para suporte à [divisão de imagem](#split-images).</span><span class="sxs-lookup"><span data-stu-id="59c54-225">For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="59c54-226">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="59c54-226">data-fullres-src</span></span> | <span data-ttu-id="59c54-227">O ponto de extremidade para a versão do recurso de imagem que foi originalmente inserido na página.</span><span class="sxs-lookup"><span data-stu-id="59c54-227">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="59c54-228">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="59c54-228">data-fullres-src-type</span></span> | <span data-ttu-id="59c54-229">O tipo de mídia do recurso **data-fullres-src**, por exemplo: `image/png` ou `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="59c54-229">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="59c54-230">data-options</span><span class="sxs-lookup"><span data-stu-id="59c54-230">data-options</span></span> | <span data-ttu-id="59c54-231">O tipo de fonte: **printout** para arquivos PDF ou **splitimage** para todos os outros.</span><span class="sxs-lookup"><span data-stu-id="59c54-231">The source type: **printout** for PDF files or **splitimage** for all others.</span></span> <span data-ttu-id="59c54-232">Aplica-se somente à [divisão de imagens](#split-images) criada com o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="59c54-232">Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="59c54-233">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="59c54-233">data-render-original-src</span></span> | <span data-ttu-id="59c54-234">A URL de origem original da imagem, se a imagem da origem for da Internet pública e tiver sido criada com o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="59c54-234">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="59c54-235">data-src-type</span><span class="sxs-lookup"><span data-stu-id="59c54-235">data-src-type</span></span> | <span data-ttu-id="59c54-236">O tipo de mídia do recurso **src**, por exemplo: `image/png` ou `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="59c54-236">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="59c54-237">data-tag</span><span class="sxs-lookup"><span data-stu-id="59c54-237">data-tag</span></span> | <span data-ttu-id="59c54-238">Uma [marca de anotação](onenote-note-tags.md) no elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-238">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="59c54-239">id</span><span class="sxs-lookup"><span data-stu-id="59c54-239">id</span></span> | <span data-ttu-id="59c54-240">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-240">A unique, generated ID for the element.</span></span> <span data-ttu-id="59c54-241">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="59c54-241">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="59c54-242">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-242">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-243">src</span><span class="sxs-lookup"><span data-stu-id="59c54-243">src</span></span> | <span data-ttu-id="59c54-244">O ponto de extremidade para a versão do recurso de imagem que foi otimizada para navegadores da Web, bem como para fatores forma de dispositivos móveis e tablet.</span><span class="sxs-lookup"><span data-stu-id="59c54-244">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="59c54-245">style</span><span class="sxs-lookup"><span data-stu-id="59c54-245">style</span></span> | <span data-ttu-id="59c54-246">As propriedades de posição da imagem.</span><span class="sxs-lookup"><span data-stu-id="59c54-246">The position properties of the image.</span></span> |
| <span data-ttu-id="59c54-247">width, height</span><span class="sxs-lookup"><span data-stu-id="59c54-247">width, height</span></span> | <span data-ttu-id="59c54-248">A largura ou altura da imagem, em pixels.</span><span class="sxs-lookup"><span data-stu-id="59c54-248">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="59c54-249">Exemplos de HTML de saída para imagens</span><span class="sxs-lookup"><span data-stu-id="59c54-249">Output HTML examples for images</span></span>

<span data-ttu-id="59c54-250">Os elementos **img** de saída contêm pontos de extremidade para recursos de arquivo de imagem e o tipo de imagem, como mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="59c54-250">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="59c54-251">Você pode fazer [solicitações GET separadas a pontos de extremidade de recurso de imagem](/graph/api/resource-get?view=graph-rest-1.0) para recuperar os respectivos conteúdos binários.</span><span class="sxs-lookup"><span data-stu-id="59c54-251">You can make separate [GET requests to image resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="59c54-252">Por padrão, as imagens não serão renderizadas diretamente em um navegador, pois elas são privadas e é necessária autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="59c54-252">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> <span data-ttu-id="59c54-253">Para obter URLs públicas para os recursos de imagem em uma página, inclua **preAuthenticated=true** na cadeia de caracteres de consulta ao recuperar o conteúdo da página (exemplo: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="59c54-253">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="59c54-254">As URLs públicas que são retornadas são válidas por uma hora.</span><span class="sxs-lookup"><span data-stu-id="59c54-254">The public URLs that are returned are valid for one hour.</span></span> 

#### <a name="image-with-public-url-when-preauthenticatedtrue-is-included-in-the-request"></a><span data-ttu-id="59c54-255">Imagem com URL pública quando _preAuthenticated=true_ é incluído na solicitação</span><span class="sxs-lookup"><span data-stu-id="59c54-255">Image with public URL when _preAuthenticated=true_ is included in the request</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}"
/>
```

<span data-ttu-id="59c54-256">Os exemplos a seguir mostram as informações que um elemento **img** pode conter no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-256">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="59c54-257">Imagem com recursos de resolução alta e prontos para Web</span><span class="sxs-lookup"><span data-stu-id="59c54-257">Image with web-ready and high resolution resources</span></span>

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

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="59c54-258">Imagem criada usando o atributo *data-render-src*</span><span class="sxs-lookup"><span data-stu-id="59c54-258">Image created by using the *data-render-src* attribute</span></span>

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

### <a name="split-images"></a><span data-ttu-id="59c54-259">Dividir imagens</span><span class="sxs-lookup"><span data-stu-id="59c54-259">Split images</span></span>

<span data-ttu-id="59c54-260">As imagens que são criadas usando o atributo **data-render-src** (de uma URL de página da Web ou de uma parte nomeada) podem ser divididas em várias imagens de componente por motivos de desempenho e renderização.</span><span class="sxs-lookup"><span data-stu-id="59c54-260">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons.</span></span> <span data-ttu-id="59c54-261">Todas as imagens de componente recebem o mesmo valor de **data-id**.</span><span class="sxs-lookup"><span data-stu-id="59c54-261">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="59c54-262">Cada imagem de componente tem um atributo de índice por dados com base zero que define o layout vertical original.</span><span class="sxs-lookup"><span data-stu-id="59c54-262">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="59c54-263">Dividir imagem com três imagens de componente</span><span class="sxs-lookup"><span data-stu-id="59c54-263">Split image with three component images</span></span>

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

<span data-ttu-id="59c54-264">Como os usuários podem mover as imagens na página, os índices retornados podem estar fora de ordem.</span><span class="sxs-lookup"><span data-stu-id="59c54-264">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="59c54-265">A ordenação deve estar na ordem y, de cima para baixo, e na ordem x, da esquerda para a direita, se houver conflitos na ordem y.</span><span class="sxs-lookup"><span data-stu-id="59c54-265">Ordering should be in top to bottom y-order, and then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="59c54-266">Elementos iframe</span><span class="sxs-lookup"><span data-stu-id="59c54-266">iframe elements</span></span>

<span data-ttu-id="59c54-267">As páginas do OneNote podem conter vídeos inseridos representados pelos elementos **iframe**.</span><span class="sxs-lookup"><span data-stu-id="59c54-267">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="59c54-268">**Observação:** você também pode [anexar um arquivo de vídeo usando um elemento **object**](onenote-images-files.md#adding-files).</span><span class="sxs-lookup"><span data-stu-id="59c54-268">**Note:** You can also [attach a video file using an **object** element](onenote-images-files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="59c54-269">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-269">Input attributes</span></span>

|<span data-ttu-id="59c54-270">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-270">Input attribute</span></span>|<span data-ttu-id="59c54-271">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-271">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-272">data-original-src</span><span class="sxs-lookup"><span data-stu-id="59c54-272">data-original-src</span></span> | <span data-ttu-id="59c54-273">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59c54-273">Required.</span></span> <span data-ttu-id="59c54-274">A URL da fonte do vídeo.</span><span class="sxs-lookup"><span data-stu-id="59c54-274">The URL of the video source.</span></span> <span data-ttu-id="59c54-275">Veja a [lista de fontes de vídeo com suporte](onenote-images-files.md#adding-videos).</span><span class="sxs-lookup"><span data-stu-id="59c54-275">See the [list of supported video sources](onenote-images-files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="59c54-276">Exemplo: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="59c54-276">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="59c54-277">width, height</span><span class="sxs-lookup"><span data-stu-id="59c54-277">width, height</span></span> | <span data-ttu-id="59c54-278">A largura ou altura do iframe, em pixels.</span><span class="sxs-lookup"><span data-stu-id="59c54-278">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="59c54-279">Exemplo: `width=300`</span><span class="sxs-lookup"><span data-stu-id="59c54-279">Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="59c54-280">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-280">Output attributes</span></span>

|<span data-ttu-id="59c54-281">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-281">Output attribute</span></span>|<span data-ttu-id="59c54-282">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-282">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-283">data-original-src</span><span class="sxs-lookup"><span data-stu-id="59c54-283">data-original-src</span></span> | <span data-ttu-id="59c54-284">A URL da fonte do vídeo.</span><span class="sxs-lookup"><span data-stu-id="59c54-284">The URL of the video source.</span></span> |
| <span data-ttu-id="59c54-285">src</span><span class="sxs-lookup"><span data-stu-id="59c54-285">src</span></span> | <span data-ttu-id="59c54-286">O link para o vídeo que é inserido na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="59c54-286">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="59c54-287">width, height</span><span class="sxs-lookup"><span data-stu-id="59c54-287">width, height</span></span> | <span data-ttu-id="59c54-288">A largura ou altura do iframe, em pixels.</span><span class="sxs-lookup"><span data-stu-id="59c54-288">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="59c54-289">Exemplo: `width=300`</span><span class="sxs-lookup"><span data-stu-id="59c54-289">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="59c54-290">Exemplo de HTML de saída para vídeos</span><span class="sxs-lookup"><span data-stu-id="59c54-290">Output HTML example for videos</span></span>

<span data-ttu-id="59c54-291">Os elementos **iframe** de saída contêm pontos de extremidade que se vinculam à página e ao vídeo da fonte, como mostrado.</span><span class="sxs-lookup"><span data-stu-id="59c54-291">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="59c54-292">Elementos object</span><span class="sxs-lookup"><span data-stu-id="59c54-292">object elements</span></span>

<span data-ttu-id="59c54-293">As páginas do OneNote contêm anexos de arquivo representados pelos elementos **object**.</span><span class="sxs-lookup"><span data-stu-id="59c54-293">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="59c54-294">Um elemento **object** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-294">An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="59c54-295">**Observação:** As APIs do OneNote também podem renderizar conteúdo de arquivo como imagens em uma página quando o arquivo é enviado como uma imagem e usa o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="59c54-295">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="59c54-296">Exemplo: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="59c54-296">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="59c54-297">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-297">Input attributes</span></span>

|<span data-ttu-id="59c54-298">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-298">Input attribute</span></span>|<span data-ttu-id="59c54-299">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-299">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-300">data</span><span class="sxs-lookup"><span data-stu-id="59c54-300">data</span></span> | <span data-ttu-id="59c54-301">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59c54-301">Required.</span></span> <span data-ttu-id="59c54-302">O nome da parte que representa o arquivo na [solicitação de partes múltiplas](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span><span class="sxs-lookup"><span data-stu-id="59c54-302">The name of the part that represents the file in the [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span> |
| <span data-ttu-id="59c54-303">data-attachment</span><span class="sxs-lookup"><span data-stu-id="59c54-303">data-attachment</span></span> | <span data-ttu-id="59c54-304">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59c54-304">Required.</span></span> <span data-ttu-id="59c54-305">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="59c54-305">The file name.</span></span> |
| <span data-ttu-id="59c54-306">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-306">data-id</span></span> | <span data-ttu-id="59c54-307">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-307">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-308">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-308">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-309">style</span><span class="sxs-lookup"><span data-stu-id="59c54-309">style</span></span> | <span data-ttu-id="59c54-310">As propriedades de posição e tamanho para o objeto: **position** (somente **absolute**), **left**, **top** e **width**.</span><span class="sxs-lookup"><span data-stu-id="59c54-310">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="59c54-311">Usado para criar um objeto [posicionado absoluto](onenote-abs-pos.md), somente se o objeto for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="59c54-311">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="59c54-312">Exemplo: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="59c54-312">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="59c54-313">type</span><span class="sxs-lookup"><span data-stu-id="59c54-313">type</span></span> | <span data-ttu-id="59c54-314">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59c54-314">Required.</span></span><br/><br/><span data-ttu-id="59c54-315">O tipo de arquivo de mídia padrão.</span><span class="sxs-lookup"><span data-stu-id="59c54-315">The standard media file type.</span></span> <span data-ttu-id="59c54-316">Os tipos de arquivo conhecidos exibem o ícone associado ao tipo de arquivo na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="59c54-316">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="59c54-317">Os tipos de arquivo desconhecidos exibem um ícone de arquivo genérico.</span><span class="sxs-lookup"><span data-stu-id="59c54-317">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="59c54-318">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-318">Output attributes</span></span>

|<span data-ttu-id="59c54-319">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-319">Output attribute</span></span>|<span data-ttu-id="59c54-320">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-320">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-321">data</span><span class="sxs-lookup"><span data-stu-id="59c54-321">data</span></span> | <span data-ttu-id="59c54-322">O ponto de extremidade para o recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="59c54-322">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="59c54-323">data-attachment</span><span class="sxs-lookup"><span data-stu-id="59c54-323">data-attachment</span></span> | <span data-ttu-id="59c54-324">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="59c54-324">The file name.</span></span> |
| <span data-ttu-id="59c54-325">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-325">data-id</span></span> | <span data-ttu-id="59c54-326">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-326">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-327">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-327">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-328">id</span><span class="sxs-lookup"><span data-stu-id="59c54-328">id</span></span> | <span data-ttu-id="59c54-329">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-329">A unique, generated ID for the element.</span></span> <span data-ttu-id="59c54-330">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="59c54-330">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="59c54-331">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-331">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-332">style</span><span class="sxs-lookup"><span data-stu-id="59c54-332">style</span></span> | <span data-ttu-id="59c54-333">As propriedades de posição do objeto.</span><span class="sxs-lookup"><span data-stu-id="59c54-333">The position properties of the object.</span></span> |
| <span data-ttu-id="59c54-334">type</span><span class="sxs-lookup"><span data-stu-id="59c54-334">type</span></span> | <span data-ttu-id="59c54-335">O tipo de arquivo de mídia padrão.</span><span class="sxs-lookup"><span data-stu-id="59c54-335">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="59c54-336">Exemplo de HTML de saída para objetos</span><span class="sxs-lookup"><span data-stu-id="59c54-336">Output HTML example for objects</span></span>

<span data-ttu-id="59c54-337">Os elementos **object** de saída contêm pontos de extremidade que se vinculam aos recursos de arquivo na página, como mostrado.</span><span class="sxs-lookup"><span data-stu-id="59c54-337">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="59c54-338">Você pode fazer [solicitações GET separadas a pontos de extremidade de recurso de arquivo](/graph/api/resource-get?view=graph-rest-1.0) para recuperar os respectivos conteúdos binários.</span><span class="sxs-lookup"><span data-stu-id="59c54-338">You can make separate [GET requests to file resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="59c54-339">Parágrafos e cabeçalhos</span><span class="sxs-lookup"><span data-stu-id="59c54-339">Paragraphs and headings</span></span>

<span data-ttu-id="59c54-340">Os parágrafos, cabeçalhos e outros contêineres de texto podem incluir os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-340">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="59c54-341">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-341">Input attributes</span></span>

|<span data-ttu-id="59c54-342">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-342">Input attribute</span></span>|<span data-ttu-id="59c54-343">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-343">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-344">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-344">data-id</span></span> | <span data-ttu-id="59c54-345">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-345">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-346">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-346">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-347">data-tag</span><span class="sxs-lookup"><span data-stu-id="59c54-347">data-tag</span></span> | <span data-ttu-id="59c54-348">Uma [marca de anotação](onenote-note-tags.md) em um elemento **p** ou **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="59c54-348">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="59c54-349">style</span><span class="sxs-lookup"><span data-stu-id="59c54-349">style</span></span> | <span data-ttu-id="59c54-350">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-350">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="59c54-351">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-351">Output attributes</span></span>

|<span data-ttu-id="59c54-352">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-352">Output attribute</span></span>|<span data-ttu-id="59c54-353">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-353">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-354">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-354">data-id</span></span> | <span data-ttu-id="59c54-355">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-355">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-356">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-356">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-357">data-tag</span><span class="sxs-lookup"><span data-stu-id="59c54-357">data-tag</span></span> | <span data-ttu-id="59c54-358">Uma [marca de anotação](onenote-note-tags.md) em um elemento **p** ou **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="59c54-358">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="59c54-359">id</span><span class="sxs-lookup"><span data-stu-id="59c54-359">id</span></span> | <span data-ttu-id="59c54-360">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-360">A unique, generated ID for the element.</span></span> <span data-ttu-id="59c54-361">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="59c54-361">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="59c54-362">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-362">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-363">style</span><span class="sxs-lookup"><span data-stu-id="59c54-363">style</span></span> | <span data-ttu-id="59c54-364">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-364">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="59c54-365">No HTML de saída, esses valores podem ser retornados embutidos em elementos filho apropriados ou em elementos **span**.</span><span class="sxs-lookup"><span data-stu-id="59c54-365">In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="59c54-366">Os exemplos a seguir mostram HTML de entrada que usa maneiras diferentes de definir estilos em contêineres de texto e o HTML de saída que é retornado.</span><span class="sxs-lookup"><span data-stu-id="59c54-366">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="59c54-367">HTML de entrada com estilos definidos usando estilos de caractere embutidos, na marca de início, e dentro de um elemento span.</span><span class="sxs-lookup"><span data-stu-id="59c54-367">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="59c54-368">Saída HTML com o estilo de caractere `<i>` e as configurações de fonte na marca de início `<p>` retornadas como estilos CSS embutidos em elementos span.</span><span class="sxs-lookup"><span data-stu-id="59c54-368">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="59c54-369">Listas</span><span class="sxs-lookup"><span data-stu-id="59c54-369">Lists</span></span>

<span data-ttu-id="59c54-370">As listas são representadas como elementos **ol** ou **ul** que contêm itens de lista representados como elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="59c54-370">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="59c54-371">Listas e itens de lista podem conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-371">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="59c54-372">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-372">Input attributes</span></span>

|<span data-ttu-id="59c54-373">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-373">Input attribute</span></span>|<span data-ttu-id="59c54-374">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-374">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-375">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-375">data-id</span></span> | <span data-ttu-id="59c54-376">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-376">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-377">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-377">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-378">data-tag</span><span class="sxs-lookup"><span data-stu-id="59c54-378">data-tag</span></span> | <span data-ttu-id="59c54-379">Uma [marca de anotação](onenote-note-tags.md) em um elemento **ul**, **ol** ou **li**.</span><span class="sxs-lookup"><span data-stu-id="59c54-379">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="59c54-380">style</span><span class="sxs-lookup"><span data-stu-id="59c54-380">style</span></span> | <span data-ttu-id="59c54-381">O **list-style-type** e as propriedades [style](#styles) do CSS para a lista ou o item de lista.</span><span class="sxs-lookup"><span data-stu-id="59c54-381">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="59c54-382">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-382">Output attributes</span></span>

|<span data-ttu-id="59c54-383">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-383">Output attribute</span></span>|<span data-ttu-id="59c54-384">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-384">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-385">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-385">data-id</span></span> | <span data-ttu-id="59c54-386">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-386">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-387">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-387">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-388">data-tag</span><span class="sxs-lookup"><span data-stu-id="59c54-388">data-tag</span></span> |  <span data-ttu-id="59c54-389">Uma [marca de anotação](onenote-note-tags.md) em um período em um elemento **li**.</span><span class="sxs-lookup"><span data-stu-id="59c54-389">A [note tag](onenote-note-tags.md) on a span in an **li** element.</span></span> |
| <span data-ttu-id="59c54-390">id</span><span class="sxs-lookup"><span data-stu-id="59c54-390">id</span></span> | <span data-ttu-id="59c54-391">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-391">A unique, generated ID for the element.</span></span> <span data-ttu-id="59c54-392">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="59c54-392">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="59c54-393">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-393">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-394">style</span><span class="sxs-lookup"><span data-stu-id="59c54-394">style</span></span> | <span data-ttu-id="59c54-395">O **list-style-type** e as propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-395">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="59c54-396">No HTML de saída, as configurações no nível de lista são retornadas em itens de lista.</span><span class="sxs-lookup"><span data-stu-id="59c54-396">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="59c54-397">As propriedades padrão não são retornadas.</span><span class="sxs-lookup"><span data-stu-id="59c54-397">Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="59c54-398">Estilos de lista</span><span class="sxs-lookup"><span data-stu-id="59c54-398">List styles</span></span>

<span data-ttu-id="59c54-399">As APIs do OneNote no Microsoft Graph dão suporte aos seguintes estilos de lista:</span><span class="sxs-lookup"><span data-stu-id="59c54-399">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="59c54-400">Lista ordenada</span><span class="sxs-lookup"><span data-stu-id="59c54-400">Ordered list</span></span>|<span data-ttu-id="59c54-401">Lista não ordenada</span><span class="sxs-lookup"><span data-stu-id="59c54-401">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-402">none</span><span class="sxs-lookup"><span data-stu-id="59c54-402">none</span></span> | <span data-ttu-id="59c54-403">none</span><span class="sxs-lookup"><span data-stu-id="59c54-403">none</span></span> |
| <span data-ttu-id="59c54-404">decimal (default)</span><span class="sxs-lookup"><span data-stu-id="59c54-404">decimal (default)</span></span> | <span data-ttu-id="59c54-405">disc (default)</span><span class="sxs-lookup"><span data-stu-id="59c54-405">disc (default)</span></span> |
| <span data-ttu-id="59c54-406">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="59c54-406">lower-alpha</span></span> | <span data-ttu-id="59c54-407">circle</span><span class="sxs-lookup"><span data-stu-id="59c54-407">circle</span></span> |
| <span data-ttu-id="59c54-408">lower-roman</span><span class="sxs-lookup"><span data-stu-id="59c54-408">lower-roman</span></span> | <span data-ttu-id="59c54-409">square</span><span class="sxs-lookup"><span data-stu-id="59c54-409">square</span></span> |
| <span data-ttu-id="59c54-410">upper-alpha</span><span class="sxs-lookup"><span data-stu-id="59c54-410">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="59c54-411">upper-roman</span><span class="sxs-lookup"><span data-stu-id="59c54-411">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="59c54-412">Você pode aplicar estilos globais para uma lista no elemento **ol** ou **ul** no HTML de entrada, mas estilos são retornados nos elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="59c54-412">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="59c54-413">Estilo de lista homogêneo</span><span class="sxs-lookup"><span data-stu-id="59c54-413">Homogenous list style</span></span>

<span data-ttu-id="59c54-414">Este exemplo mostra o HTML de entrada que define o tipo de estilo de lista no elemento **ol** e estilos CSS em itens de lista individuais.</span><span class="sxs-lookup"><span data-stu-id="59c54-414">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="59c54-415">Este é o HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-415">This is the output HTML.</span></span> <span data-ttu-id="59c54-416">Observe que os estilos são retornados embutidos nos elementos **li** ou **span** individuais.</span><span class="sxs-lookup"><span data-stu-id="59c54-416">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="59c54-417">Estilos de lista variáveis</span><span class="sxs-lookup"><span data-stu-id="59c54-417">Variable list styles</span></span>

<span data-ttu-id="59c54-418">Este exemplo mostra o HTML de entrada que define diferentes tipos de estilo de lista nos elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="59c54-418">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="59c54-419">Este é o HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-419">This is the output HTML.</span></span> <span data-ttu-id="59c54-420">Observe que os estilos são retornados embutidos nos elementos **li** ou **span** individuais.</span><span class="sxs-lookup"><span data-stu-id="59c54-420">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="59c54-421">Tabelas</span><span class="sxs-lookup"><span data-stu-id="59c54-421">Tables</span></span>

<span data-ttu-id="59c54-422">As tabelas são representadas como elementos **table** que podem conter elementos **tr** e **td**.</span><span class="sxs-lookup"><span data-stu-id="59c54-422">Tables are represented as **table** elements that can contain **tr** and **td** elements.</span></span> <span data-ttu-id="59c54-423">Há suporte para tabelas aninhadas.</span><span class="sxs-lookup"><span data-stu-id="59c54-423">Nested tables are supported.</span></span>

<span data-ttu-id="59c54-424">As tabelas podem conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="59c54-424">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="59c54-425">As APIs do OneNote não dão suporte aos atributos **rowspan** ou **colspan**.</span><span class="sxs-lookup"><span data-stu-id="59c54-425">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="59c54-426">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-426">Input attributes</span></span>

|<span data-ttu-id="59c54-427">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="59c54-427">Input attribute</span></span>|<span data-ttu-id="59c54-428">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-428">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-429">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-429">data-id</span></span> | <span data-ttu-id="59c54-430">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-430">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-431">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-431">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-432">style</span><span class="sxs-lookup"><span data-stu-id="59c54-432">style</span></span> | <span data-ttu-id="59c54-433">As propriedades [style](#styles) do CSS do elemento e também:</span><span class="sxs-lookup"><span data-stu-id="59c54-433">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="59c54-434">- **border**.</span><span class="sxs-lookup"><span data-stu-id="59c54-434">- **border**.</span></span> <span data-ttu-id="59c54-435">Pode ser 0px ou 1px.</span><span class="sxs-lookup"><span data-stu-id="59c54-435">Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="59c54-436">- **width**.</span><span class="sxs-lookup"><span data-stu-id="59c54-436">- **width**.</span></span> <span data-ttu-id="59c54-437">Com suporte de **table** e **td** como pixels ou porcentagem de largura da página.</span><span class="sxs-lookup"><span data-stu-id="59c54-437">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="59c54-438">Exemplo: `width="100px"` ou `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="59c54-438">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="59c54-439">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-439">Output attributes</span></span>

|<span data-ttu-id="59c54-440">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="59c54-440">Output attribute</span></span>|<span data-ttu-id="59c54-441">Descrição</span><span class="sxs-lookup"><span data-stu-id="59c54-441">Description</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-442">data-id</span><span class="sxs-lookup"><span data-stu-id="59c54-442">data-id</span></span> | <span data-ttu-id="59c54-443">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-443">A reference for the element.</span></span><br/><br/><span data-ttu-id="59c54-444">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-444">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-445">id</span><span class="sxs-lookup"><span data-stu-id="59c54-445">id</span></span> | <span data-ttu-id="59c54-446">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-446">A unique, generated ID for the element.</span></span> <span data-ttu-id="59c54-447">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="59c54-447">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="59c54-448">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-448">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="59c54-449">style</span><span class="sxs-lookup"><span data-stu-id="59c54-449">style</span></span> | <span data-ttu-id="59c54-450">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="59c54-450">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="59c54-451">Os exemplos a seguir mostram HTML de entrada que usa maneiras diferentes de definir estilos em tabelas e o HTML de saída que é retornado.</span><span class="sxs-lookup"><span data-stu-id="59c54-451">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="59c54-452">HTML de entrada com configurações opcionais em níveis diferentes.</span><span class="sxs-lookup"><span data-stu-id="59c54-452">Input HTML with optional settings at different levels</span></span>

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
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="59c54-453">HTML de saída com estilos CSS retornados embutidos nos elementos td.</span><span class="sxs-lookup"><span data-stu-id="59c54-453">Output HTML with CSS styles returned inline on the td elements</span></span>

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


## <a name="styles"></a><span data-ttu-id="59c54-454">Estilos</span><span class="sxs-lookup"><span data-stu-id="59c54-454">Styles</span></span>

<span data-ttu-id="59c54-455">As APIs do OneNote no Microsoft Graph dão suporte as propriedades **style** do CSS embutidas a seguir para elementos no corpo da página, como **body**, **div**, **p**, **li** e **span**.</span><span class="sxs-lookup"><span data-stu-id="59c54-455">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="59c54-456">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59c54-456">Property</span></span>|<span data-ttu-id="59c54-457">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59c54-457">Example</span></span>|
|:------|:------|
| <span data-ttu-id="59c54-458">background-color</span><span class="sxs-lookup"><span data-stu-id="59c54-458">background-color</span></span> | <span data-ttu-id="59c54-459">`style="background-color:#66cc66"` (o padrão é branco)</span><span class="sxs-lookup"><span data-stu-id="59c54-459">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="59c54-460">Há suporte para cores nomeadas e formato hexadecimal.</span><span class="sxs-lookup"><span data-stu-id="59c54-460">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="59c54-461">color</span><span class="sxs-lookup"><span data-stu-id="59c54-461">color</span></span> | <span data-ttu-id="59c54-462">`style="color:#ffffff"` (o padrão é preto)</span><span class="sxs-lookup"><span data-stu-id="59c54-462">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="59c54-463">font-family</span><span class="sxs-lookup"><span data-stu-id="59c54-463">font-family</span></span> | <span data-ttu-id="59c54-464">`style="font-family:Courier"` (o padrão é Calibri)</span><span class="sxs-lookup"><span data-stu-id="59c54-464">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="59c54-465">font-size</span><span class="sxs-lookup"><span data-stu-id="59c54-465">font-size</span></span> | <span data-ttu-id="59c54-466">`style="font-size:10pt"` (o padrão é 11pt)</span><span class="sxs-lookup"><span data-stu-id="59c54-466">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="59c54-467">As APIs aceitam o tamanho da fonte em *pt* ou *px*, mas converte *px* em *pt*.</span><span class="sxs-lookup"><span data-stu-id="59c54-467">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="59c54-468">Valores decimais são arredondados para o n,0pt ou n,5pt mais próximo.</span><span class="sxs-lookup"><span data-stu-id="59c54-468">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="59c54-469">font-style</span><span class="sxs-lookup"><span data-stu-id="59c54-469">font-style</span></span> | <span data-ttu-id="59c54-470">`style="font-style:italic"` (somente normal ou itálico)</span><span class="sxs-lookup"><span data-stu-id="59c54-470">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="59c54-471">font-weight</span><span class="sxs-lookup"><span data-stu-id="59c54-471">font-weight</span></span> | <span data-ttu-id="59c54-472">`style="font-weight:bold"` (somente normal ou negrito)</span><span class="sxs-lookup"><span data-stu-id="59c54-472">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="59c54-473">strike-through</span><span class="sxs-lookup"><span data-stu-id="59c54-473">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="59c54-474">text-align</span><span class="sxs-lookup"><span data-stu-id="59c54-474">text-align</span></span> | <span data-ttu-id="59c54-475">`style="text-align:center"` (somente para elementos de bloco)</span><span class="sxs-lookup"><span data-stu-id="59c54-475">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="59c54-476">text-decoration</span><span class="sxs-lookup"><span data-stu-id="59c54-476">text-decoration</span></span> | <span data-ttu-id="59c54-477">`style="text-decoration:underline"` (somente nenhum ou sublinhado)</span><span class="sxs-lookup"><span data-stu-id="59c54-477">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="59c54-478">Os seguintes estilos de caractere embutidos também têm suporte:</span><span class="sxs-lookup"><span data-stu-id="59c54-478">The following inline character styles are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="59c54-479"><b></span><span class="sxs-lookup"><span data-stu-id="59c54-479"><b></span></span></td>
<td id="simplecell"><span data-ttu-id="59c54-480"><i></span><span class="sxs-lookup"><span data-stu-id="59c54-480"><i></span></span></td>
<td id="simplecell"><span data-ttu-id="59c54-481"><u></span><span class="sxs-lookup"><span data-stu-id="59c54-481"><u></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="59c54-482"><em></span><span class="sxs-lookup"><span data-stu-id="59c54-482"><em></span></span></td>
<td id="simplecell"><span data-ttu-id="59c54-483"><strong></span><span class="sxs-lookup"><span data-stu-id="59c54-483"><strong></span></span></td>
<td id="simplecell"><span data-ttu-id="59c54-484"><strike></span><span class="sxs-lookup"><span data-stu-id="59c54-484"><strike></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="59c54-485"><sup></span><span class="sxs-lookup"><span data-stu-id="59c54-485"><sup></span></span></td>
<td id="simplecell"><span data-ttu-id="59c54-486"><sub></span><span class="sxs-lookup"><span data-stu-id="59c54-486"><sub></span></span></td>
<td id="simplecell"><span data-ttu-id="59c54-487"><del></span><span class="sxs-lookup"><span data-stu-id="59c54-487"><del></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="59c54-488"><cite></span><span class="sxs-lookup"><span data-stu-id="59c54-488"><cite></span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="59c54-489">Exemplo de HTML de entrada e saída</span><span class="sxs-lookup"><span data-stu-id="59c54-489">Input and output HTML example</span></span>

<span data-ttu-id="59c54-490">A imagem a seguir mostra uma página simples que foi criada com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="59c54-490">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Imagem de uma página do OneNote com notas de conteúdo do estudo da Wikipédia](images/onenote-sample-image.png)

<span data-ttu-id="59c54-492">Este é o HTML de entrada enviado no corpo da mensagem para criar a página.</span><span class="sxs-lookup"><span data-stu-id="59c54-492">This is the input HTML sent in the message body to create the page.</span></span>

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
        <img alt="Apollo 11 commemorative stamp." src="https://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<br/>

<span data-ttu-id="59c54-493">Este é o HTML de saída que o Microsoft Graph retorna quando você [obtém o conteúdo da página](onenote-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="59c54-493">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="59c54-494">**Observação:** quando você [cria uma página](onenote-create-page.md) ou [obtém metadados de página](/graph/api/page-get?view=graph-rest-1.0), a API retorna a URL de ponto de extremidade do *conteúdo* da página na propriedade **contentUrl**.</span><span class="sxs-lookup"><span data-stu-id="59c54-494">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](/graph/api/page-get?view=graph-rest-1.0), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
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
            <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="59c54-495">Confira também</span><span class="sxs-lookup"><span data-stu-id="59c54-495">See also</span></span>

- [<span data-ttu-id="59c54-496">Obter a estrutura e o conteúdo do OneNote</span><span class="sxs-lookup"><span data-stu-id="59c54-496">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="59c54-497">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="59c54-497">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="59c54-498">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="59c54-498">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="59c54-499">Adicionar imagens, vídeos e arquivos</span><span class="sxs-lookup"><span data-stu-id="59c54-499">Add images, videos, and files</span></span>](onenote-images-files.md)
