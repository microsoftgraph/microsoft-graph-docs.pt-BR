---
title: HTML de entrada e saída nas páginas do OneNote
description: 'O HTML que define o conteúdo e a estrutura da página quando você cria ou atualiza uma página do OneNote é chamado de *HTML de entrada*. '
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: fcb4a8127b633ba309212a7160c9e5548836466c
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639214"
---
# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="35f3e-103">HTML de entrada e saída nas páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="35f3e-103">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="35f3e-104">O HTML que define o conteúdo e a estrutura da página quando você [cria](onenote-create-page.md) ou [atualiza](onenote-update-page.md) uma página do OneNote é chamado de *HTML de entrada*.</span><span class="sxs-lookup"><span data-stu-id="35f3e-104">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote-update-page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="35f3e-105">O HTML que é retornado quando você [obtém o conteúdo da página](onenote-get-content.md) é chamado de *HTML de saída*.</span><span class="sxs-lookup"><span data-stu-id="35f3e-105">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*.</span></span> <span data-ttu-id="35f3e-106">O HTML de saída não será igual ao HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="35f3e-106">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="35f3e-107">As APIs do OneNote no Microsoft Graph preservam o conteúdo semântico e a estrutura básica do HTML de entrada, mas os convertem em um conjunto de [elementos HTML e propriedades CSS com suporte](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="35f3e-107">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="35f3e-108">As APIs também adicionam atributos personalizados que dão suporte a recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="35f3e-108">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="35f3e-109">Este artigo descreve os principais elementos e atributos do HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-109">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="35f3e-110">Pode ser útil entender o HTML de entrada quando você estiver criando ou atualizando o conteúdo da página e o HTML de saída quando estiver analisando o conteúdo da página retornado.</span><span class="sxs-lookup"><span data-stu-id="35f3e-110">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="35f3e-111">Elemento body</span><span class="sxs-lookup"><span data-stu-id="35f3e-111">body element</span></span>

<span data-ttu-id="35f3e-112">O conteúdo HTML no corpo da página representa o conteúdo e a estrutura da página, inclusive os recursos de imagem e arquivo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-112">The HTML content in the page body represents the page content and structure, including image and file resources.</span></span> <span data-ttu-id="35f3e-113">O elemento **body** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-113">The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="35f3e-114">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-114">Input attributes</span></span>

|<span data-ttu-id="35f3e-115">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-115">Input attribute</span></span>|<span data-ttu-id="35f3e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-116">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-117">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="35f3e-117">data-absolute-enabled</span></span> | <span data-ttu-id="35f3e-118">Indica se o corpo da entrada dá suporte a elementos [posicionados absolutos](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-118">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="35f3e-119">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-119">style</span></span> | <p><span data-ttu-id="35f3e-120">As propriedades [style](#styles) do CSS do corpo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-120">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="35f3e-121">No HTML de saída, as configurações de entrada podem ser retornadas embutidas em elementos filho apropriados.</span><span class="sxs-lookup"><span data-stu-id="35f3e-121">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="35f3e-122">Atualmente, a cor da tela de fundo não tem suporte para o elemento **body**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-122">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="35f3e-123">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-123">Output attributes</span></span>

|<span data-ttu-id="35f3e-124">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-124">Output attribute</span></span>|<span data-ttu-id="35f3e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-125">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-126">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="35f3e-126">data-absolute-enabled</span></span> | <span data-ttu-id="35f3e-127">Indica se o corpo dá suporte a elementos [posicionados absolutos](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-127">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> <span data-ttu-id="35f3e-128">Sempre **true** no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-128">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="35f3e-129">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-129">style</span></span> | <span data-ttu-id="35f3e-130">As propriedades **font-family** e **font-size** do corpo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-130">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="35f3e-131">Elementos Div</span><span class="sxs-lookup"><span data-stu-id="35f3e-131">div elements</span></span>

<span data-ttu-id="35f3e-132">Os elementos **Div** contêm texto, imagens e outros tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-132">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="35f3e-133">Um elemento **div** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-133">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="35f3e-134">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-134">Input attributes</span></span>

|<span data-ttu-id="35f3e-135">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-135">Input attribute</span></span>|<span data-ttu-id="35f3e-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-136">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-137">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-137">data-id</span></span> | <span data-ttu-id="35f3e-138">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-138">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-139">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-139">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-140">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="35f3e-140">data-render-fallback</span></span> | <span data-ttu-id="35f3e-141">A ação de fallback se [extraction](onenote-extract-data.md) falhar: **render** (padrão) ou **none**</span><span class="sxs-lookup"><span data-stu-id="35f3e-141">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**</span></span> |
| <span data-ttu-id="35f3e-142">data-render-method</span><span class="sxs-lookup"><span data-stu-id="35f3e-142">data-render-method</span></span> | <span data-ttu-id="35f3e-143">O método [extraction](onenote-extract-data.md) a ser executado, por exemplo:</span><span class="sxs-lookup"><span data-stu-id="35f3e-143">The [extraction](onenote-extract-data.md) method to perform, for example:</span></span><br/><span data-ttu-id="35f3e-144">`extract.businesscard` ou `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="35f3e-144">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="35f3e-145">data-render-src</span><span class="sxs-lookup"><span data-stu-id="35f3e-145">data-render-src</span></span> | <span data-ttu-id="35f3e-146">A fonte de conteúdo para [extraction](onenote-extract-data.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-146">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="35f3e-147">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-147">style</span></span> | <span data-ttu-id="35f3e-148">As propriedades de posição, tamanho, fonte e cor para o div:</span><span class="sxs-lookup"><span data-stu-id="35f3e-148">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="35f3e-149">**posição** (**absoluto** somente), **esquerdo**, **superior** e **largura** (a altura é automaticamente configurada para divs)</span><span class="sxs-lookup"><span data-stu-id="35f3e-149">**position** (**absolute** only), **left**, **top**, and **width** (height is auto-configured for divs)</span></span><br/><br/><span data-ttu-id="35f3e-150">Usado para criar um div [posicionado absoluto](onenote-abs-pos.md), somente se o div for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="35f3e-150">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="35f3e-151">Exemplo: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="35f3e-151">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="35f3e-152">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-152">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="35f3e-153">No HTML de saída, esses valores são retornados embutidos em elementos filho apropriados.</span><span class="sxs-lookup"><span data-stu-id="35f3e-153">In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="35f3e-154">As APIs do OneNote no Microsoft Graph encapsulam todo o conteúdo do corpo em pelo menos um div.</span><span class="sxs-lookup"><span data-stu-id="35f3e-154">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="35f3e-155">A API cria um div padrão (atribuído com `data-id="_default"`) para incluir o conteúdo do corpo se:</span><span class="sxs-lookup"><span data-stu-id="35f3e-155">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="35f3e-156">O atributo **data-absolute-enabled** do elemento body de entrada for omitido ou definido como **false**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-156">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**.</span></span> <span data-ttu-id="35f3e-157">Nesse caso, todo o conteúdo do corpo é colocado no div padrão.</span><span class="sxs-lookup"><span data-stu-id="35f3e-157">In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="35f3e-158">O atributo **data-absolute-enabled** do elemento body de entrada for **true**, mas o HTML de entrada contiver filhos diretos que não são [elementos](onenote-abs-pos.md)&nbsp;**div**, **img** ou **object** posicionados de forma absoluta.</span><span class="sxs-lookup"><span data-stu-id="35f3e-158">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="35f3e-159">Nesse caso, os filhos diretos que não forem [elementos](onenote-abs-pos.md)&nbsp;**div**, **img** ou **object** posicionados de forma absoluta serão colocados no div padrão.</span><span class="sxs-lookup"><span data-stu-id="35f3e-159">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="35f3e-160">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-160">Output attributes</span></span>

|<span data-ttu-id="35f3e-161">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-161">Output attribute</span></span>|<span data-ttu-id="35f3e-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-162">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-163">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-163">data-id</span></span> | <span data-ttu-id="35f3e-164">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-164">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-165">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-165">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-166">id</span><span class="sxs-lookup"><span data-stu-id="35f3e-166">id</span></span> | <span data-ttu-id="35f3e-167">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-167">A unique, generated ID for the element.</span></span> <span data-ttu-id="35f3e-168">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="35f3e-168">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="35f3e-169">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-169">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-170">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-170">style</span></span> | <span data-ttu-id="35f3e-171">As propriedades de tamanho e posição do div.</span><span class="sxs-lookup"><span data-stu-id="35f3e-171">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="35f3e-172">Divs não contribuintes</span><span class="sxs-lookup"><span data-stu-id="35f3e-172">Non-contributing divs</span></span>

<span data-ttu-id="35f3e-173">Quando um elemento **div** no HTML de entrada não contribui com a estrutura da página nem carrega informações usadas pelo OneNote, a API move o conteúdo do div para o div pai ou padrão.</span><span class="sxs-lookup"><span data-stu-id="35f3e-173">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="35f3e-174">Isso é ilustrado nos exemplos a seguir.</span><span class="sxs-lookup"><span data-stu-id="35f3e-174">This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="35f3e-175">HTML de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-175">Input HTML</span></span>

<span data-ttu-id="35f3e-176">Contém um div aninhado não contribuinte.</span><span class="sxs-lookup"><span data-stu-id="35f3e-176">Contains a non-contributing, nested div.</span></span>

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

#### <a name="output-html"></a><span data-ttu-id="35f3e-177">HTML de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-177">Output HTML</span></span>

> <span data-ttu-id="35f3e-178">**Observação**: o conteúdo do div foi movido para o div pai e as marcas `<div>` aninhadas foram removidas.</span><span class="sxs-lookup"><span data-stu-id="35f3e-178">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="35f3e-179">O div seria preservado se definisse qualquer informação semântica, como **data-id** (exemplo: `<div data-id="keep-me">`).</span><span class="sxs-lookup"><span data-stu-id="35f3e-179">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

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


## <a name="img-elements"></a><span data-ttu-id="35f3e-180">Elementos img</span><span class="sxs-lookup"><span data-stu-id="35f3e-180">img elements</span></span>

<span data-ttu-id="35f3e-181">Imagens em páginas do OneNote são representadas pelos elementos **img**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-181">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="35f3e-182">Um elemento **img** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-182">An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="35f3e-183">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-183">Input attributes</span></span>

|<span data-ttu-id="35f3e-184">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-184">Input attribute</span></span>|<span data-ttu-id="35f3e-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-185">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-186">alt</span><span class="sxs-lookup"><span data-stu-id="35f3e-186">alt</span></span> | <span data-ttu-id="35f3e-187">O texto Alt fornecido para a imagem.</span><span class="sxs-lookup"><span data-stu-id="35f3e-187">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="35f3e-188">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-188">data-id</span></span> | <span data-ttu-id="35f3e-189">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-189">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-190">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-190">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-191">data-render-src</span><span class="sxs-lookup"><span data-stu-id="35f3e-191">data-render-src</span></span> |<span data-ttu-id="35f3e-192">Ou **data-render-src** ou **src** é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35f3e-192">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="35f3e-193">A página da Web a ser renderizada como uma imagem mapeada por bit na página do OneNote:</span><span class="sxs-lookup"><span data-stu-id="35f3e-193">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="35f3e-194">- `data-render-src="https://..."` para uma URL pública.</span><span class="sxs-lookup"><span data-stu-id="35f3e-194">- `data-render-src="https://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="35f3e-195">- `data-render-src="name:BlockName"` para parte de uma imagem no bloco "Apresentação" de uma [solicitação de partes múltiplas](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span><span class="sxs-lookup"><span data-stu-id="35f3e-195">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span><br/><br/><span data-ttu-id="35f3e-196">Esse método é útil quando a página da Web é mais complexa que a página que o OneNote pode renderizar fielmente ou quando a página exige credenciais de logon.</span><span class="sxs-lookup"><span data-stu-id="35f3e-196">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="35f3e-197">data-tag</span><span class="sxs-lookup"><span data-stu-id="35f3e-197">data-tag</span></span> | <span data-ttu-id="35f3e-198">Uma [marca de anotação](onenote-note-tags.md) no elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-198">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="35f3e-199">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-199">style</span></span> |<span data-ttu-id="35f3e-200">As propriedades de posição e tamanho para a imagem: **position** (somente **absolute**), **left**, **top**, **width** e **height**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-200">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="35f3e-201">O tamanho pode ser definido em qualquer imagem.</span><span class="sxs-lookup"><span data-stu-id="35f3e-201">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="35f3e-202">As propriedades de posição serão usadas para criar uma imagem [posicionada absoluta](onenote-abs-pos.md), somente se a imagem for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="35f3e-202">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="35f3e-203">Exemplo: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="35f3e-203">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="35f3e-204">No HTML de saída, o tamanho da imagem é retornado separadamente nos atributos **width** e **height**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-204">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="35f3e-205">src</span><span class="sxs-lookup"><span data-stu-id="35f3e-205">src</span></span> |<span data-ttu-id="35f3e-206">Ou **src** ou **data-render-src** é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35f3e-206">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="35f3e-207">A imagem a ser renderizada na página do OneNote:</span><span class="sxs-lookup"><span data-stu-id="35f3e-207">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="35f3e-208">- `src="https://..."` para uma URL para uma imagem publicamente disponível na Internet.</span><span class="sxs-lookup"><span data-stu-id="35f3e-208">- `src="https://..."` for a URL to a publicly available image on the Internet.</span></span><br/><br/> <span data-ttu-id="35f3e-209">- `src="name:BlockName"` para uma parte nomeada em uma solicitação de partes múltiplas que representa a imagem.</span><span class="sxs-lookup"><span data-stu-id="35f3e-209">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="35f3e-210">width, height</span><span class="sxs-lookup"><span data-stu-id="35f3e-210">width, height</span></span> | <span data-ttu-id="35f3e-211">A largura ou altura da imagem, em pixels, mas sem o px.</span><span class="sxs-lookup"><span data-stu-id="35f3e-211">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="35f3e-212">Exemplo: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="35f3e-212">Example: `width="400"`</span></span> |
 
> <span data-ttu-id="35f3e-213">**Observação:** as APIs do OneNote detectam automaticamente o tipo de imagem de entrada e o retornam como o **data-fullres-src-type** no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-213">**Note:** The OneNote APIs automatically detect the input image type, and return it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="35f3e-214">A API também retorna o tipo de imagem da imagem otimizada em **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-214">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="35f3e-215">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-215">Output attributes</span></span>

|<span data-ttu-id="35f3e-216">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-216">Output attribute</span></span>|<span data-ttu-id="35f3e-217">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-217">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-218">alt</span><span class="sxs-lookup"><span data-stu-id="35f3e-218">alt</span></span> | <span data-ttu-id="35f3e-219">O texto Alt fornecido para a imagem.</span><span class="sxs-lookup"><span data-stu-id="35f3e-219">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="35f3e-220">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-220">data-id</span></span> | <span data-ttu-id="35f3e-221">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-221">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-222">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-222">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-223">data-index</span><span class="sxs-lookup"><span data-stu-id="35f3e-223">data-index</span></span> | <span data-ttu-id="35f3e-224">A posição da imagem.</span><span class="sxs-lookup"><span data-stu-id="35f3e-224">The position of the image.</span></span> <span data-ttu-id="35f3e-225">Para suporte à [divisão de imagem](#split-images).</span><span class="sxs-lookup"><span data-stu-id="35f3e-225">For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="35f3e-226">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="35f3e-226">data-fullres-src</span></span> | <span data-ttu-id="35f3e-227">O ponto de extremidade para a versão do recurso de imagem que foi originalmente inserido na página.</span><span class="sxs-lookup"><span data-stu-id="35f3e-227">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="35f3e-228">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="35f3e-228">data-fullres-src-type</span></span> | <span data-ttu-id="35f3e-229">O tipo de mídia do recurso **data-fullres-src**, por exemplo: `image/png` ou `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="35f3e-229">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="35f3e-230">data-options</span><span class="sxs-lookup"><span data-stu-id="35f3e-230">data-options</span></span> | <span data-ttu-id="35f3e-231">O tipo de fonte: **printout** para arquivos PDF ou **splitimage** para todos os outros.</span><span class="sxs-lookup"><span data-stu-id="35f3e-231">The source type: **printout** for PDF files or **splitimage** for all others.</span></span> <span data-ttu-id="35f3e-232">Aplica-se somente à [divisão de imagens](#split-images) criada com o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-232">Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="35f3e-233">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="35f3e-233">data-render-original-src</span></span> | <span data-ttu-id="35f3e-234">A URL de origem original da imagem, se a imagem da origem for da Internet pública e tiver sido criada com o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-234">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="35f3e-235">data-src-type</span><span class="sxs-lookup"><span data-stu-id="35f3e-235">data-src-type</span></span> | <span data-ttu-id="35f3e-236">O tipo de mídia do recurso **src**, por exemplo: `image/png` ou `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="35f3e-236">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="35f3e-237">data-tag</span><span class="sxs-lookup"><span data-stu-id="35f3e-237">data-tag</span></span> | <span data-ttu-id="35f3e-238">Uma [marca de anotação](onenote-note-tags.md) no elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-238">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="35f3e-239">id</span><span class="sxs-lookup"><span data-stu-id="35f3e-239">id</span></span> | <span data-ttu-id="35f3e-240">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-240">A unique, generated ID for the element.</span></span> <span data-ttu-id="35f3e-241">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="35f3e-241">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="35f3e-242">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-242">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-243">src</span><span class="sxs-lookup"><span data-stu-id="35f3e-243">src</span></span> | <span data-ttu-id="35f3e-244">O ponto de extremidade para a versão do recurso de imagem que foi otimizada para navegadores da Web, bem como para fatores forma de dispositivos móveis e tablet.</span><span class="sxs-lookup"><span data-stu-id="35f3e-244">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="35f3e-245">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-245">style</span></span> | <span data-ttu-id="35f3e-246">As propriedades de posição da imagem.</span><span class="sxs-lookup"><span data-stu-id="35f3e-246">The position properties of the image.</span></span> |
| <span data-ttu-id="35f3e-247">width, height</span><span class="sxs-lookup"><span data-stu-id="35f3e-247">width, height</span></span> | <span data-ttu-id="35f3e-248">A largura ou altura da imagem, em pixels.</span><span class="sxs-lookup"><span data-stu-id="35f3e-248">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="35f3e-249">Exemplos de HTML de saída para imagens</span><span class="sxs-lookup"><span data-stu-id="35f3e-249">Output HTML examples for images</span></span>

<span data-ttu-id="35f3e-250">Os elementos **img** de saída contêm pontos de extremidade para recursos de arquivo de imagem e o tipo de imagem, como mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-250">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="35f3e-251">Você pode fazer [solicitações GET separadas a pontos de extremidade de recurso de imagem](/graph/api/resource-get?view=graph-rest-1.0) para recuperar os respectivos conteúdos binários.</span><span class="sxs-lookup"><span data-stu-id="35f3e-251">You can make separate [GET requests to image resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="35f3e-252">Os exemplos a seguir mostram as informações que um elemento **img** pode conter no HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-252">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="35f3e-253">Imagem com recursos de resolução alta e prontos para Web</span><span class="sxs-lookup"><span data-stu-id="35f3e-253">Image with web-ready and high resolution resources</span></span>

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

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="35f3e-254">Imagem criada usando o atributo *data-render-src*</span><span class="sxs-lookup"><span data-stu-id="35f3e-254">Image created by using the *data-render-src* attribute</span></span>

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

### <a name="split-images"></a><span data-ttu-id="35f3e-255">Dividir imagens</span><span class="sxs-lookup"><span data-stu-id="35f3e-255">Split images</span></span>

<span data-ttu-id="35f3e-256">As imagens que são criadas usando o atributo **data-render-src** (de uma URL de página da Web ou de uma parte nomeada) podem ser divididas em várias imagens de componente por motivos de desempenho e renderização.</span><span class="sxs-lookup"><span data-stu-id="35f3e-256">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons.</span></span> <span data-ttu-id="35f3e-257">Todas as imagens de componente recebem o mesmo valor de **data-id**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-257">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="35f3e-258">Cada imagem de componente tem um atributo de índice por dados com base zero que define o layout vertical original.</span><span class="sxs-lookup"><span data-stu-id="35f3e-258">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="35f3e-259">Dividir imagem com três imagens de componente</span><span class="sxs-lookup"><span data-stu-id="35f3e-259">Split image with three component images</span></span>

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

<span data-ttu-id="35f3e-260">Como os usuários podem mover as imagens na página, os índices retornados podem estar fora de ordem.</span><span class="sxs-lookup"><span data-stu-id="35f3e-260">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="35f3e-261">A ordenação deve estar na ordem y, de cima para baixo, e na ordem x, da esquerda para a direita, se houver conflitos na ordem y.</span><span class="sxs-lookup"><span data-stu-id="35f3e-261">Ordering should be in top to bottom y-order, and then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="35f3e-262">Elementos iframe</span><span class="sxs-lookup"><span data-stu-id="35f3e-262">iframe elements</span></span>

<span data-ttu-id="35f3e-263">As páginas do OneNote podem conter vídeos inseridos representados pelos elementos **iframe**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-263">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="35f3e-264">**Observação:** você também pode [anexar um arquivo de vídeo usando um elemento **object**](onenote-images-files.md#adding-files).</span><span class="sxs-lookup"><span data-stu-id="35f3e-264">**Note:** You can also [attach a video file using an **object** element](onenote-images-files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="35f3e-265">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-265">Input attributes</span></span>

|<span data-ttu-id="35f3e-266">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-266">Input attribute</span></span>|<span data-ttu-id="35f3e-267">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-267">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-268">data-original-src</span><span class="sxs-lookup"><span data-stu-id="35f3e-268">data-original-src</span></span> | <span data-ttu-id="35f3e-269">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35f3e-269">Required.</span></span> <span data-ttu-id="35f3e-270">A URL da fonte do vídeo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-270">The URL of the video source.</span></span> <span data-ttu-id="35f3e-271">Veja a [lista de fontes de vídeo com suporte](onenote-images-files.md#adding-videos).</span><span class="sxs-lookup"><span data-stu-id="35f3e-271">See the [list of supported video sources](onenote-images-files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="35f3e-272">Exemplo: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="35f3e-272">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="35f3e-273">width, height</span><span class="sxs-lookup"><span data-stu-id="35f3e-273">width, height</span></span> | <span data-ttu-id="35f3e-274">A largura ou altura do iframe, em pixels.</span><span class="sxs-lookup"><span data-stu-id="35f3e-274">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="35f3e-275">Exemplo: `width=300`</span><span class="sxs-lookup"><span data-stu-id="35f3e-275">Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="35f3e-276">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-276">Output attributes</span></span>

|<span data-ttu-id="35f3e-277">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-277">Output attribute</span></span>|<span data-ttu-id="35f3e-278">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-278">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-279">data-original-src</span><span class="sxs-lookup"><span data-stu-id="35f3e-279">data-original-src</span></span> | <span data-ttu-id="35f3e-280">A URL da fonte do vídeo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-280">The URL of the video source.</span></span> |
| <span data-ttu-id="35f3e-281">src</span><span class="sxs-lookup"><span data-stu-id="35f3e-281">src</span></span> | <span data-ttu-id="35f3e-282">O link para o vídeo que é inserido na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="35f3e-282">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="35f3e-283">width, height</span><span class="sxs-lookup"><span data-stu-id="35f3e-283">width, height</span></span> | <span data-ttu-id="35f3e-284">A largura ou altura do iframe, em pixels.</span><span class="sxs-lookup"><span data-stu-id="35f3e-284">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="35f3e-285">Exemplo: `width=300`</span><span class="sxs-lookup"><span data-stu-id="35f3e-285">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="35f3e-286">Exemplo de HTML de saída para vídeos</span><span class="sxs-lookup"><span data-stu-id="35f3e-286">Output HTML example for videos</span></span>

<span data-ttu-id="35f3e-287">Os elementos **iframe** de saída contêm pontos de extremidade que se vinculam à página e ao vídeo da fonte, como mostrado.</span><span class="sxs-lookup"><span data-stu-id="35f3e-287">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="35f3e-288">Elementos object</span><span class="sxs-lookup"><span data-stu-id="35f3e-288">object elements</span></span>

<span data-ttu-id="35f3e-289">As páginas do OneNote contêm anexos de arquivo representados pelos elementos **object**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-289">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="35f3e-290">Um elemento **object** pode conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-290">An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="35f3e-291">**Observação:** As APIs do OneNote também podem renderizar conteúdo de arquivo como imagens em uma página quando o arquivo é enviado como uma imagem e usa o atributo **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-291">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="35f3e-292">Exemplo: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="35f3e-292">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="35f3e-293">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-293">Input attributes</span></span>

|<span data-ttu-id="35f3e-294">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-294">Input attribute</span></span>|<span data-ttu-id="35f3e-295">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-295">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-296">data</span><span class="sxs-lookup"><span data-stu-id="35f3e-296">data</span></span> | <span data-ttu-id="35f3e-297">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35f3e-297">Required.</span></span> <span data-ttu-id="35f3e-298">O nome da parte que representa o arquivo na [solicitação de partes múltiplas](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span><span class="sxs-lookup"><span data-stu-id="35f3e-298">The name of the part that represents the file in the [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span> |
| <span data-ttu-id="35f3e-299">data-attachment</span><span class="sxs-lookup"><span data-stu-id="35f3e-299">data-attachment</span></span> | <span data-ttu-id="35f3e-300">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35f3e-300">Required.</span></span> <span data-ttu-id="35f3e-301">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-301">The file name.</span></span> |
| <span data-ttu-id="35f3e-302">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-302">data-id</span></span> | <span data-ttu-id="35f3e-303">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-303">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-304">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-304">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-305">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-305">style</span></span> | <span data-ttu-id="35f3e-306">As propriedades de posição e tamanho para o objeto: **position** (somente **absolute**), **left**, **top** e **width**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-306">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="35f3e-307">Usado para criar um objeto [posicionado absoluto](onenote-abs-pos.md), somente se o objeto for um filho direto do corpo quando o corpo define `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="35f3e-307">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="35f3e-308">Exemplo: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="35f3e-308">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="35f3e-309">type</span><span class="sxs-lookup"><span data-stu-id="35f3e-309">type</span></span> | <span data-ttu-id="35f3e-310">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35f3e-310">Required.</span></span><br/><br/><span data-ttu-id="35f3e-311">O tipo de arquivo de mídia padrão.</span><span class="sxs-lookup"><span data-stu-id="35f3e-311">The standard media file type.</span></span> <span data-ttu-id="35f3e-312">Os tipos de arquivo conhecidos exibem o ícone associado ao tipo de arquivo na página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="35f3e-312">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="35f3e-313">Os tipos de arquivo desconhecidos exibem um ícone de arquivo genérico.</span><span class="sxs-lookup"><span data-stu-id="35f3e-313">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="35f3e-314">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-314">Output attributes</span></span>

|<span data-ttu-id="35f3e-315">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-315">Output attribute</span></span>|<span data-ttu-id="35f3e-316">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-316">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-317">data</span><span class="sxs-lookup"><span data-stu-id="35f3e-317">data</span></span> | <span data-ttu-id="35f3e-318">O ponto de extremidade para o recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-318">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="35f3e-319">data-attachment</span><span class="sxs-lookup"><span data-stu-id="35f3e-319">data-attachment</span></span> | <span data-ttu-id="35f3e-320">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-320">The file name.</span></span> |
| <span data-ttu-id="35f3e-321">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-321">data-id</span></span> | <span data-ttu-id="35f3e-322">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-322">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-323">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-323">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-324">id</span><span class="sxs-lookup"><span data-stu-id="35f3e-324">id</span></span> | <span data-ttu-id="35f3e-325">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-325">A unique, generated ID for the element.</span></span> <span data-ttu-id="35f3e-326">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="35f3e-326">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="35f3e-327">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-327">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-328">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-328">style</span></span> | <span data-ttu-id="35f3e-329">As propriedades de posição do objeto.</span><span class="sxs-lookup"><span data-stu-id="35f3e-329">The position properties of the object.</span></span> |
| <span data-ttu-id="35f3e-330">type</span><span class="sxs-lookup"><span data-stu-id="35f3e-330">type</span></span> | <span data-ttu-id="35f3e-331">O tipo de arquivo de mídia padrão.</span><span class="sxs-lookup"><span data-stu-id="35f3e-331">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="35f3e-332">Exemplo de HTML de saída para objetos</span><span class="sxs-lookup"><span data-stu-id="35f3e-332">Output HTML example for objects</span></span>

<span data-ttu-id="35f3e-333">Os elementos **object** de saída contêm pontos de extremidade que se vinculam aos recursos de arquivo na página, como mostrado.</span><span class="sxs-lookup"><span data-stu-id="35f3e-333">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="35f3e-334">Você pode fazer [solicitações GET separadas a pontos de extremidade de recurso de arquivo](/graph/api/resource-get?view=graph-rest-1.0) para recuperar os respectivos conteúdos binários.</span><span class="sxs-lookup"><span data-stu-id="35f3e-334">You can make separate [GET requests to file resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="35f3e-335">Parágrafos e cabeçalhos</span><span class="sxs-lookup"><span data-stu-id="35f3e-335">Paragraphs and headings</span></span>

<span data-ttu-id="35f3e-336">Os parágrafos, cabeçalhos e outros contêineres de texto podem incluir os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-336">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="35f3e-337">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-337">Input attributes</span></span>

|<span data-ttu-id="35f3e-338">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-338">Input attribute</span></span>|<span data-ttu-id="35f3e-339">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-339">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-340">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-340">data-id</span></span> | <span data-ttu-id="35f3e-341">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-341">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-342">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-342">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-343">data-tag</span><span class="sxs-lookup"><span data-stu-id="35f3e-343">data-tag</span></span> | <span data-ttu-id="35f3e-344">Uma [marca de anotação](onenote-note-tags.md) em um elemento **p** ou **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-344">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="35f3e-345">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-345">style</span></span> | <span data-ttu-id="35f3e-346">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-346">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="35f3e-347">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-347">Output attributes</span></span>

|<span data-ttu-id="35f3e-348">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-348">Output attribute</span></span>|<span data-ttu-id="35f3e-349">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-349">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-350">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-350">data-id</span></span> | <span data-ttu-id="35f3e-351">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-351">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-352">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-352">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-353">data-tag</span><span class="sxs-lookup"><span data-stu-id="35f3e-353">data-tag</span></span> | <span data-ttu-id="35f3e-354">Uma [marca de anotação](onenote-note-tags.md) em um elemento **p** ou **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-354">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="35f3e-355">id</span><span class="sxs-lookup"><span data-stu-id="35f3e-355">id</span></span> | <span data-ttu-id="35f3e-356">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-356">A unique, generated ID for the element.</span></span> <span data-ttu-id="35f3e-357">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="35f3e-357">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="35f3e-358">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-358">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-359">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-359">style</span></span> | <span data-ttu-id="35f3e-360">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-360">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="35f3e-361">No HTML de saída, esses valores podem ser retornados embutidos em elementos filho apropriados ou em elementos **span**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-361">In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="35f3e-362">Os exemplos a seguir mostram HTML de entrada que usa maneiras diferentes de definir estilos em contêineres de texto e o HTML de saída que é retornado.</span><span class="sxs-lookup"><span data-stu-id="35f3e-362">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="35f3e-363">HTML de entrada com estilos definidos usando estilos de caractere embutidos, na marca de início, e dentro de um elemento span.</span><span class="sxs-lookup"><span data-stu-id="35f3e-363">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="35f3e-364">Saída HTML com o estilo de caractere `<i>` e as configurações de fonte na marca de início `<p>` retornadas como estilos CSS embutidos em elementos span.</span><span class="sxs-lookup"><span data-stu-id="35f3e-364">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="35f3e-365">Listas</span><span class="sxs-lookup"><span data-stu-id="35f3e-365">Lists</span></span>

<span data-ttu-id="35f3e-366">As listas são representadas como elementos **ol** ou **ul** que contêm itens de lista representados como elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-366">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="35f3e-367">Listas e itens de lista podem conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-367">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="35f3e-368">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-368">Input attributes</span></span>

|<span data-ttu-id="35f3e-369">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-369">Input attribute</span></span>|<span data-ttu-id="35f3e-370">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-370">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-371">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-371">data-id</span></span> | <span data-ttu-id="35f3e-372">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-372">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-373">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-373">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-374">data-tag</span><span class="sxs-lookup"><span data-stu-id="35f3e-374">data-tag</span></span> | <span data-ttu-id="35f3e-375">Uma [marca de anotação](onenote-note-tags.md) em um elemento **ul**, **ol** ou **li**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-375">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="35f3e-376">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-376">style</span></span> | <span data-ttu-id="35f3e-377">O **list-style-type** e as propriedades [style](#styles) do CSS para a lista ou o item de lista.</span><span class="sxs-lookup"><span data-stu-id="35f3e-377">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="35f3e-378">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-378">Output attributes</span></span>

|<span data-ttu-id="35f3e-379">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-379">Output attribute</span></span>|<span data-ttu-id="35f3e-380">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-380">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-381">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-381">data-id</span></span> | <span data-ttu-id="35f3e-382">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-382">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-383">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-383">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-384">data-tag</span><span class="sxs-lookup"><span data-stu-id="35f3e-384">data-tag</span></span> |  <span data-ttu-id="35f3e-385">Uma [marca de anotação](onenote-note-tags.md) em um período em um elemento **li**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-385">A [note tag](onenote-note-tags.md) on a span in an **li** element.</span></span> |
| <span data-ttu-id="35f3e-386">id</span><span class="sxs-lookup"><span data-stu-id="35f3e-386">id</span></span> | <span data-ttu-id="35f3e-387">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-387">A unique, generated ID for the element.</span></span> <span data-ttu-id="35f3e-388">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="35f3e-388">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="35f3e-389">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-389">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-390">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-390">style</span></span> | <span data-ttu-id="35f3e-391">O **list-style-type** e as propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-391">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="35f3e-392">No HTML de saída, as configurações no nível de lista são retornadas em itens de lista.</span><span class="sxs-lookup"><span data-stu-id="35f3e-392">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="35f3e-393">As propriedades padrão não são retornadas.</span><span class="sxs-lookup"><span data-stu-id="35f3e-393">Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="35f3e-394">Estilos de lista</span><span class="sxs-lookup"><span data-stu-id="35f3e-394">List styles</span></span>

<span data-ttu-id="35f3e-395">As APIs do OneNote no Microsoft Graph dão suporte aos seguintes estilos de lista:</span><span class="sxs-lookup"><span data-stu-id="35f3e-395">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="35f3e-396">Lista ordenada</span><span class="sxs-lookup"><span data-stu-id="35f3e-396">Ordered list</span></span>|<span data-ttu-id="35f3e-397">Lista não ordenada</span><span class="sxs-lookup"><span data-stu-id="35f3e-397">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-398">none</span><span class="sxs-lookup"><span data-stu-id="35f3e-398">none</span></span> | <span data-ttu-id="35f3e-399">none</span><span class="sxs-lookup"><span data-stu-id="35f3e-399">none</span></span> |
| <span data-ttu-id="35f3e-400">decimal (default)</span><span class="sxs-lookup"><span data-stu-id="35f3e-400">decimal (default)</span></span> | <span data-ttu-id="35f3e-401">disc (default)</span><span class="sxs-lookup"><span data-stu-id="35f3e-401">disc (default)</span></span> |
| <span data-ttu-id="35f3e-402">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="35f3e-402">lower-alpha</span></span> | <span data-ttu-id="35f3e-403">circle</span><span class="sxs-lookup"><span data-stu-id="35f3e-403">circle</span></span> |
| <span data-ttu-id="35f3e-404">lower-roman</span><span class="sxs-lookup"><span data-stu-id="35f3e-404">lower-roman</span></span> | <span data-ttu-id="35f3e-405">square</span><span class="sxs-lookup"><span data-stu-id="35f3e-405">square</span></span> |
| <span data-ttu-id="35f3e-406">upper-alpha</span><span class="sxs-lookup"><span data-stu-id="35f3e-406">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="35f3e-407">upper-roman</span><span class="sxs-lookup"><span data-stu-id="35f3e-407">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="35f3e-408">Você pode aplicar estilos globais para uma lista no elemento **ol** ou **ul** no HTML de entrada, mas estilos são retornados nos elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-408">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="35f3e-409">Estilo de lista homogêneo</span><span class="sxs-lookup"><span data-stu-id="35f3e-409">Homogenous list style</span></span>

<span data-ttu-id="35f3e-410">Este exemplo mostra o HTML de entrada que define o tipo de estilo de lista no elemento **ol** e estilos CSS em itens de lista individuais.</span><span class="sxs-lookup"><span data-stu-id="35f3e-410">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="35f3e-411">Este é o HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-411">This is the output HTML.</span></span> <span data-ttu-id="35f3e-412">Observe que os estilos são retornados embutidos nos elementos **li** ou **span** individuais.</span><span class="sxs-lookup"><span data-stu-id="35f3e-412">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="35f3e-413">Estilos de lista variáveis</span><span class="sxs-lookup"><span data-stu-id="35f3e-413">Variable list styles</span></span>

<span data-ttu-id="35f3e-414">Este exemplo mostra o HTML de entrada que define diferentes tipos de estilo de lista nos elementos **li**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-414">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="35f3e-415">Este é o HTML de saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-415">This is the output HTML.</span></span> <span data-ttu-id="35f3e-416">Observe que os estilos são retornados embutidos nos elementos **li** ou **span** individuais.</span><span class="sxs-lookup"><span data-stu-id="35f3e-416">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="35f3e-417">Tabelas</span><span class="sxs-lookup"><span data-stu-id="35f3e-417">Tables</span></span>

<span data-ttu-id="35f3e-418">As tabelas são representadas como elementos **table** que podem conter elementos **tr** e **td**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-418">Tables are represented as **table** elements that can contain **tr** and **td** elements.</span></span> <span data-ttu-id="35f3e-419">Há suporte para tabelas aninhadas.</span><span class="sxs-lookup"><span data-stu-id="35f3e-419">Nested tables are supported.</span></span>

<span data-ttu-id="35f3e-420">As tabelas podem conter os atributos a seguir no HTML de entrada e saída.</span><span class="sxs-lookup"><span data-stu-id="35f3e-420">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="35f3e-421">As APIs do OneNote não dão suporte aos atributos **rowspan** ou **colspan**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-421">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="35f3e-422">Atributos de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-422">Input attributes</span></span>

|<span data-ttu-id="35f3e-423">Atributo de entrada</span><span class="sxs-lookup"><span data-stu-id="35f3e-423">Input attribute</span></span>|<span data-ttu-id="35f3e-424">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-424">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-425">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-425">data-id</span></span> | <span data-ttu-id="35f3e-426">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-426">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-427">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-427">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-428">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-428">style</span></span> | <span data-ttu-id="35f3e-429">As propriedades [style](#styles) do CSS do elemento e também:</span><span class="sxs-lookup"><span data-stu-id="35f3e-429">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="35f3e-430">- **border**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-430">- **border**.</span></span> <span data-ttu-id="35f3e-431">Pode ser 0px ou 1px.</span><span class="sxs-lookup"><span data-stu-id="35f3e-431">Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="35f3e-432">- **width**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-432">- **width**.</span></span> <span data-ttu-id="35f3e-433">Com suporte de **table** e **td** como pixels ou porcentagem de largura da página.</span><span class="sxs-lookup"><span data-stu-id="35f3e-433">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="35f3e-434">Exemplo: `width="100px"` ou `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="35f3e-434">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="35f3e-435">Atributos de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-435">Output attributes</span></span>

|<span data-ttu-id="35f3e-436">Atributo de saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-436">Output attribute</span></span>|<span data-ttu-id="35f3e-437">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f3e-437">Description</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-438">data-id</span><span class="sxs-lookup"><span data-stu-id="35f3e-438">data-id</span></span> | <span data-ttu-id="35f3e-439">Uma referência para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-439">A reference for the element.</span></span><br/><br/><span data-ttu-id="35f3e-440">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-440">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-441">id</span><span class="sxs-lookup"><span data-stu-id="35f3e-441">id</span></span> | <span data-ttu-id="35f3e-442">Uma ID exclusiva, gerada para o elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-442">A unique, generated ID for the element.</span></span> <span data-ttu-id="35f3e-443">Retornado por [solicitações GET a um ponto de extremidade de *conteúdo* da página](/graph/api/page-get?view=graph-rest-1.0) quando a opção de consulta `includeIDs=true` é usada.</span><span class="sxs-lookup"><span data-stu-id="35f3e-443">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="35f3e-444">Usado para [atualizar conteúdo da página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-444">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="35f3e-445">style</span><span class="sxs-lookup"><span data-stu-id="35f3e-445">style</span></span> | <span data-ttu-id="35f3e-446">As propriedades [style](#styles) do CSS do elemento.</span><span class="sxs-lookup"><span data-stu-id="35f3e-446">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="35f3e-447">Os exemplos a seguir mostram HTML de entrada que usa maneiras diferentes de definir estilos em tabelas e o HTML de saída que é retornado.</span><span class="sxs-lookup"><span data-stu-id="35f3e-447">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="35f3e-448">HTML de entrada com configurações opcionais em níveis diferentes.</span><span class="sxs-lookup"><span data-stu-id="35f3e-448">Input HTML with optional settings at different levels</span></span>

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
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="35f3e-449">HTML de saída com estilos CSS retornados embutidos nos elementos td.</span><span class="sxs-lookup"><span data-stu-id="35f3e-449">Output HTML with CSS styles returned inline on the td elements</span></span>

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


## <a name="styles"></a><span data-ttu-id="35f3e-450">Estilos</span><span class="sxs-lookup"><span data-stu-id="35f3e-450">Styles</span></span>

<span data-ttu-id="35f3e-451">As APIs do OneNote no Microsoft Graph dão suporte as propriedades **style** do CSS embutidas a seguir para elementos no corpo da página, como **body**, **div**, **p**, **li** e **span**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-451">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="35f3e-452">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35f3e-452">Property</span></span>|<span data-ttu-id="35f3e-453">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35f3e-453">Example</span></span>|
|:------|:------|
| <span data-ttu-id="35f3e-454">background-color</span><span class="sxs-lookup"><span data-stu-id="35f3e-454">background-color</span></span> | <span data-ttu-id="35f3e-455">`style="background-color:#66cc66"` (o padrão é branco)</span><span class="sxs-lookup"><span data-stu-id="35f3e-455">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="35f3e-456">Há suporte para cores nomeadas e formato hexadecimal.</span><span class="sxs-lookup"><span data-stu-id="35f3e-456">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="35f3e-457">color</span><span class="sxs-lookup"><span data-stu-id="35f3e-457">color</span></span> | <span data-ttu-id="35f3e-458">`style="color:#ffffff"` (o padrão é preto)</span><span class="sxs-lookup"><span data-stu-id="35f3e-458">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="35f3e-459">font-family</span><span class="sxs-lookup"><span data-stu-id="35f3e-459">font-family</span></span> | <span data-ttu-id="35f3e-460">`style="font-family:Courier"` (o padrão é Calibri)</span><span class="sxs-lookup"><span data-stu-id="35f3e-460">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="35f3e-461">font-size</span><span class="sxs-lookup"><span data-stu-id="35f3e-461">font-size</span></span> | <span data-ttu-id="35f3e-462">`style="font-size:10pt"` (o padrão é 11pt)</span><span class="sxs-lookup"><span data-stu-id="35f3e-462">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="35f3e-463">As APIs aceitam o tamanho da fonte em *pt* ou *px*, mas converte *px* em *pt*.</span><span class="sxs-lookup"><span data-stu-id="35f3e-463">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="35f3e-464">Valores decimais são arredondados para o n,0pt ou n,5pt mais próximo.</span><span class="sxs-lookup"><span data-stu-id="35f3e-464">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="35f3e-465">font-style</span><span class="sxs-lookup"><span data-stu-id="35f3e-465">font-style</span></span> | <span data-ttu-id="35f3e-466">`style="font-style:italic"` (somente normal ou itálico)</span><span class="sxs-lookup"><span data-stu-id="35f3e-466">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="35f3e-467">font-weight</span><span class="sxs-lookup"><span data-stu-id="35f3e-467">font-weight</span></span> | <span data-ttu-id="35f3e-468">`style="font-weight:bold"` (somente normal ou negrito)</span><span class="sxs-lookup"><span data-stu-id="35f3e-468">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="35f3e-469">strike-through</span><span class="sxs-lookup"><span data-stu-id="35f3e-469">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="35f3e-470">text-align</span><span class="sxs-lookup"><span data-stu-id="35f3e-470">text-align</span></span> | <span data-ttu-id="35f3e-471">`style="text-align:center"` (somente para elementos de bloco)</span><span class="sxs-lookup"><span data-stu-id="35f3e-471">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="35f3e-472">text-decoration</span><span class="sxs-lookup"><span data-stu-id="35f3e-472">text-decoration</span></span> | <span data-ttu-id="35f3e-473">`style="text-decoration:underline"` (somente nenhum ou sublinhado)</span><span class="sxs-lookup"><span data-stu-id="35f3e-473">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="35f3e-474">Os seguintes estilos de caractere embutidos também têm suporte:</span><span class="sxs-lookup"><span data-stu-id="35f3e-474">The following inline character styles are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="35f3e-475"><b></span><span class="sxs-lookup"><span data-stu-id="35f3e-475"><b></span></span></td>
<td id="simplecell"><span data-ttu-id="35f3e-476"><i></span><span class="sxs-lookup"><span data-stu-id="35f3e-476"><i></span></span></td>
<td id="simplecell"><span data-ttu-id="35f3e-477"><u></span><span class="sxs-lookup"><span data-stu-id="35f3e-477"><u></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="35f3e-478"><em></span><span class="sxs-lookup"><span data-stu-id="35f3e-478"><em></span></span></td>
<td id="simplecell"><span data-ttu-id="35f3e-479"><strong></span><span class="sxs-lookup"><span data-stu-id="35f3e-479"><strong></span></span></td>
<td id="simplecell"><span data-ttu-id="35f3e-480"><strike></span><span class="sxs-lookup"><span data-stu-id="35f3e-480"><strike></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="35f3e-481"><sup></span><span class="sxs-lookup"><span data-stu-id="35f3e-481"><sup></span></span></td>
<td id="simplecell"><span data-ttu-id="35f3e-482"><sub></span><span class="sxs-lookup"><span data-stu-id="35f3e-482"><sub></span></span></td>
<td id="simplecell"><span data-ttu-id="35f3e-483"><del></span><span class="sxs-lookup"><span data-stu-id="35f3e-483"><del></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="35f3e-484"><cite></span><span class="sxs-lookup"><span data-stu-id="35f3e-484"><cite></span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="35f3e-485">Exemplo de HTML de entrada e saída</span><span class="sxs-lookup"><span data-stu-id="35f3e-485">Input and output HTML example</span></span>

<span data-ttu-id="35f3e-486">A imagem a seguir mostra uma página simples que foi criada com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="35f3e-486">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Imagem de uma página do OneNote com notas de conteúdo do estudo da Wikipédia](images/onenote-sample-image.png)

<span data-ttu-id="35f3e-488">Este é o HTML de entrada enviado no corpo da mensagem para criar a página.</span><span class="sxs-lookup"><span data-stu-id="35f3e-488">This is the input HTML sent in the message body to create the page.</span></span>

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

<span data-ttu-id="35f3e-489">Este é o HTML de saída que o Microsoft Graph retorna quando você [obtém o conteúdo da página](onenote-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="35f3e-489">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="35f3e-490">**Observação:** quando você [cria uma página](onenote-create-page.md) ou [obtém metadados de página](/graph/api/page-get?view=graph-rest-1.0), a API retorna a URL de ponto de extremidade do *conteúdo* da página na propriedade **contentUrl**.</span><span class="sxs-lookup"><span data-stu-id="35f3e-490">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](/graph/api/page-get?view=graph-rest-1.0), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="35f3e-491">Confira também</span><span class="sxs-lookup"><span data-stu-id="35f3e-491">See also</span></span>

- [<span data-ttu-id="35f3e-492">Obter a estrutura e o conteúdo do OneNote</span><span class="sxs-lookup"><span data-stu-id="35f3e-492">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="35f3e-493">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="35f3e-493">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="35f3e-494">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="35f3e-494">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="35f3e-495">Adicionar imagens, vídeos e arquivos</span><span class="sxs-lookup"><span data-stu-id="35f3e-495">Add images, videos, and files</span></span>](onenote-images-files.md)
