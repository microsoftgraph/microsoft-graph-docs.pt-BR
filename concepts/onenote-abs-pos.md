---
title: Criar elementos posicionados absolutos nas páginas do OneNote
description: O corpo de uma página do OneNote pode conter vários elementos filhos diretos `div`, `img` e `object` que podem ser posicionados de forma independente na página.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: e21ad3fb97b807bc91ecf6a993483f3bb83c82b8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472836"
---
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a><span data-ttu-id="6266e-103">Criar elementos posicionados absolutos nas páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="6266e-103">Create absolute positioned elements in OneNote pages</span></span>

<span data-ttu-id="6266e-104">O corpo de uma página do OneNote pode conter vários elementos filhos diretos `div`, `img` e `object` que podem ser posicionados de forma independente na página.</span><span class="sxs-lookup"><span data-stu-id="6266e-104">The body of a OneNote page can contain multiple direct `div`, `img`, and `object` child elements that can be positioned independently on the page.</span></span>

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a><span data-ttu-id="6266e-105">Atributos e comportamento de posicionamento</span><span class="sxs-lookup"><span data-stu-id="6266e-105">Attributes and positioning behavior</span></span>

<span data-ttu-id="6266e-106">Use os atributos `data-absolute-enabled` e [`style`](#supported-css-style-attributes) para criar elementos posicionados absolutos em uma página, da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="6266e-106">Use the `data-absolute-enabled` and [`style`](#supported-css-style-attributes) attributes to create absolute positioned elements on a page, as follows:</span></span>

- <span data-ttu-id="6266e-107">O elemento do corpo deve especificar `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="6266e-107">The body element must specify `data-absolute-enabled="true"`.</span></span> <span data-ttu-id="6266e-108">Se omitido ou definido como `false`, todo o conteúdo do corpo será processado dentro de um div posicionado absoluto `_default` que a API cria e todas as configurações de posição serão ignoradas.</span><span class="sxs-lookup"><span data-stu-id="6266e-108">If omitted or set to `false`, all body content is rendered inside a `_default` absolute positioned div that the API creates, and all position settings are ignored.</span></span>

- <span data-ttu-id="6266e-109">Apenas os elementos `div`, `img` e `object` podem incluir elementos posicionados absolutos.</span><span class="sxs-lookup"><span data-stu-id="6266e-109">Only `div`, `img`, and `object` elements can be absolute positioned elements.</span></span> 

- <span data-ttu-id="6266e-110">Os elementos posicionados absolutos devem especificar `style="position:absolute"`.</span><span class="sxs-lookup"><span data-stu-id="6266e-110">Absolute positioned elements must specify `style="position:absolute"`.</span></span>

- <span data-ttu-id="6266e-111">Os elementos posicionados absolutos devem ser filhos diretos do elemento `body`.</span><span class="sxs-lookup"><span data-stu-id="6266e-111">Absolute positioned elements must be direct children of the `body` element.</span></span> <span data-ttu-id="6266e-112">Quaisquer filhos diretos do corpo que não sejam elementos posicionados absolutos `div`, `img` ou `object` serão processados como conteúdo estático no div posicionado absoluto `_default`.</span><span class="sxs-lookup"><span data-stu-id="6266e-112">Any direct children of the body that aren't absolute positioned `div`, `img`, or `object` elements are rendered as static content inside the absolute positioned `_default` div.</span></span>

- <span data-ttu-id="6266e-113">Os elementos posicionados absolutos são colocados nas coordenadas especificadas superiores e esquerdas, relativas à posição inicial 0:0 no canto superior esquerdo da página, acima da área de título.</span><span class="sxs-lookup"><span data-stu-id="6266e-113">Absolute positioned elements are positioned at their specified top and left coordinates, relative to the 0:0 starting position at the top, left corner of the page above the title area.</span></span>

- <span data-ttu-id="6266e-114">Quando um elemento com posicionamento absoluto omite coordenada esquerda ou superior, a coordenada ausente está definida com o valor padrão: `top:120px` ou `left:48px`.</span><span class="sxs-lookup"><span data-stu-id="6266e-114">If an absolute positioned element omits the top or left coordinate, the missing coordinate is set to its default value: `top:120px` or `left:48px`.</span></span> <span data-ttu-id="6266e-115">Essas coordenadas padrão especificam uma posição abaixo da área de título.</span><span class="sxs-lookup"><span data-stu-id="6266e-115">These default coordinates specify a position just below the title area.</span></span> <span data-ttu-id="6266e-116">Lembre-se de que omitir coordenadas pode resultar em elementos empilhados.</span><span class="sxs-lookup"><span data-stu-id="6266e-116">Be aware that omitting coordinates can result in elements that are stacked on top of each other.</span></span>

- <span data-ttu-id="6266e-117">Os elementos posicionados absolutos não podem ser aninhados, nem conter elementos posicionados.</span><span class="sxs-lookup"><span data-stu-id="6266e-117">Absolute positioned elements cannot be nested or contain positioned elements.</span></span> <span data-ttu-id="6266e-118">A API ignora as configurações de posição especificadas em elementos aninhados dentro do div posicionado absoluto, processa o conteúdo aninhado dentro do div pai posicionado absoluto e retorna um aviso na propriedade **api.diagnostics** na resposta.</span><span class="sxs-lookup"><span data-stu-id="6266e-118">The API ignores any position settings specified on nested elements inside an absolute positioned div, renders the nested content inside the absolute positioned parent div, and returns a warning in the **api.diagnostics** property in the response.</span></span>


### <a name="example"></a><span data-ttu-id="6266e-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6266e-119">Example</span></span>

<span data-ttu-id="6266e-120">O exemplo a seguir contém um filho `p` direto, um div posicionado absoluto e um div posicionado não absoluto.</span><span class="sxs-lookup"><span data-stu-id="6266e-120">The following example contains a direct `p` child, an absolute positioned div, and a non-absolute positioned div.</span></span>

#### <a name="input-html"></a><span data-ttu-id="6266e-121">HTML de entrada</span><span class="sxs-lookup"><span data-stu-id="6266e-121">Input HTML</span></span>  

   ```html 
   <body data-absolute-enabled="true">
       <p>This content will appear in the _default div.</p>
       <div style="position:absolute;top:175px;left:100px" data-id="div1">
         <p>This content will appear in an absolute positioned div.</p>
       </div>
       <div>
           <p>This content will also appear in the _default div.</p>
       </div>
   </body>
   ```

<span data-ttu-id="6266e-122">A API processa o div posicionado não absoluto no div padrão.</span><span class="sxs-lookup"><span data-stu-id="6266e-122">The API renders the non-absolute positioned div in the default div.</span></span> <span data-ttu-id="6266e-123">Observe que as marcas aninhadas `<div>` são descartadas porque não definem informações semânticas (como `data-id`).</span><span class="sxs-lookup"><span data-stu-id="6266e-123">Note that the nested `<div>` tags are discarded because they do not define any semantic information (such as `data-id`).</span></span>

#### <a name="output-html"></a><span data-ttu-id="6266e-124">HTML de saída</span><span class="sxs-lookup"><span data-stu-id="6266e-124">Output HTML</span></span> 

   ```html 
   <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
       <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
           <p>This content will appear in the _default div.</p>
           <p>This content will also appear in the _default div.</p>
       </div>
       <div data-id="div1" style="position:absolute;left:99px;top:174px;width:624px">
           <p>This content will appear in an absolute positioned div.</p>
       </div>
   </body>
   ```

### <a name="example"></a><span data-ttu-id="6266e-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6266e-125">Example</span></span>

<span data-ttu-id="6266e-126">O exemplo a seguir cria uma página que contém um div posicionado absoluto e uma imagem posicionada absoluta.</span><span class="sxs-lookup"><span data-stu-id="6266e-126">The following example creates a page that contains one absolute positioned div and one absolute positioned image.</span></span>


#### <a name="input-html"></a><span data-ttu-id="6266e-127">HTML de entrada</span><span class="sxs-lookup"><span data-stu-id="6266e-127">Input HTML</span></span>  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
<span data-ttu-id="6266e-128">A API do OneNote avalia o HTML de entrada e preserva todo o conteúdo semântico e qualquer informação estrutural compatível com o OneNote.</span><span class="sxs-lookup"><span data-stu-id="6266e-128">The OneNote API evaluates the input HTML and preserves all semantic content and any structural information that is supported by OneNote.</span></span> <span data-ttu-id="6266e-129">A página resultante processa conforme mostrado na imagem a seguir, mas sem as bordas visíveis do div e da imagem.</span><span class="sxs-lookup"><span data-stu-id="6266e-129">The resulting page renders as shown in the following image (but without the visible borders for the div and image).</span></span> 

![A página resultante com o div posicionado absoluto e a imagem](images/abs-pos.png)

<span data-ttu-id="6266e-131">Observe as alterações no div aninhado não contribuidor do HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="6266e-131">Notice the changes to the non-contributing, nested div from the input HTML.</span></span> <span data-ttu-id="6266e-132">A API preserva o conteúdo do div, mas descarta as marcas `<div>` porque o div não define informações semânticas (como `data-id`).</span><span class="sxs-lookup"><span data-stu-id="6266e-132">The API preserves the div's content but discards the `<div>` tags because the div doesn't define semantic information (such as `data-id`).</span></span>

<span data-ttu-id="6266e-133">Saiba mais sobre como a API do OneNote lida com HTML de entrada e saída em [HTML de entrada e de saída para páginas do OneNote](onenote-input-output-html.md).</span><span class="sxs-lookup"><span data-stu-id="6266e-133">For more information about how the OneNote API handles input and output HTML, see [Input and output HTML for OneNote pages](onenote-input-output-html.md).</span></span>

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a><span data-ttu-id="6266e-134">Atributos de estilos CSS compatíveis</span><span class="sxs-lookup"><span data-stu-id="6266e-134">Supported CSS style attributes</span></span>

<span data-ttu-id="6266e-135">Todos os elementos posicionados absolutos podem especificar as posições superiores e esquerdas.</span><span class="sxs-lookup"><span data-stu-id="6266e-135">All absolute positioned elements can specify top and left positions.</span></span> <span data-ttu-id="6266e-136">Divs e imagens podem especificar a largura e as imagens também podem especificar a altura.</span><span class="sxs-lookup"><span data-stu-id="6266e-136">Divs and images can specify width, and images can also specify height.</span></span> <span data-ttu-id="6266e-137">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="6266e-137">For example:</span></span>

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| <span data-ttu-id="6266e-138">Atributo</span><span class="sxs-lookup"><span data-stu-id="6266e-138">Attribute</span></span> | <span data-ttu-id="6266e-139">Elemento compatível</span><span class="sxs-lookup"><span data-stu-id="6266e-139">Supported element</span></span> | <span data-ttu-id="6266e-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="6266e-140">Description</span></span> |  
|:------|:------|:------|  
| <span data-ttu-id="6266e-141">top</span><span class="sxs-lookup"><span data-stu-id="6266e-141">top</span></span> | <span data-ttu-id="6266e-142">div, img, object</span><span class="sxs-lookup"><span data-stu-id="6266e-142">div, img, object</span></span> | <span data-ttu-id="6266e-143">A coordenada do eixo Y da borda superior do elemento, somente em pixels.</span><span class="sxs-lookup"><span data-stu-id="6266e-143">The y-axis coordinate of the element's top border, in pixels only.</span></span> <span data-ttu-id="6266e-144">O padrão é 120 pixels.</span><span class="sxs-lookup"><span data-stu-id="6266e-144">Default is 120 pixels.</span></span><br/><br/><span data-ttu-id="6266e-145">Exemplo: `top:140px`</span><span class="sxs-lookup"><span data-stu-id="6266e-145">Example: `top:140px`</span></span> |  
| <span data-ttu-id="6266e-146">left</span><span class="sxs-lookup"><span data-stu-id="6266e-146">left</span></span> |  <span data-ttu-id="6266e-147">div, img, object</span><span class="sxs-lookup"><span data-stu-id="6266e-147">div, img, object</span></span>  | <span data-ttu-id="6266e-148">A coordenada do eixo X da borda esquerda do elemento, somente em pixels.</span><span class="sxs-lookup"><span data-stu-id="6266e-148">The x-axis coordinate of the element's left border, in pixels only.</span></span> <span data-ttu-id="6266e-149">O padrão é 48 pixels.</span><span class="sxs-lookup"><span data-stu-id="6266e-149">Default is 48 pixels.</span></span><br/><br/><span data-ttu-id="6266e-150">Exemplo: `left:95px`</span><span class="sxs-lookup"><span data-stu-id="6266e-150">Example: `left:95px`</span></span> |  
| <span data-ttu-id="6266e-151">width</span><span class="sxs-lookup"><span data-stu-id="6266e-151">width</span></span> |  <span data-ttu-id="6266e-152">div, img</span><span class="sxs-lookup"><span data-stu-id="6266e-152">div, img</span></span>  | <span data-ttu-id="6266e-153">A largura do elemento, somente em pixels.</span><span class="sxs-lookup"><span data-stu-id="6266e-153">The width of the element, in pixels only.</span></span><br/><br/><span data-ttu-id="6266e-154">Exemplo: `width:480px`</span><span class="sxs-lookup"><span data-stu-id="6266e-154">Example: `width:480px`</span></span> |  
| <span data-ttu-id="6266e-155">height</span><span class="sxs-lookup"><span data-stu-id="6266e-155">height</span></span> | <span data-ttu-id="6266e-156">img</span><span class="sxs-lookup"><span data-stu-id="6266e-156">img</span></span> | <span data-ttu-id="6266e-157">A altura do elemento, somente em pixels.</span><span class="sxs-lookup"><span data-stu-id="6266e-157">The height of the element, in pixels only.</span></span> <span data-ttu-id="6266e-158">Para divs, a altura é calculada no tempo de execução e qualquer valor de altura especificado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="6266e-158">For divs, height is calculated at runtime and any specified height value is ignored.</span></span><br/><br/><span data-ttu-id="6266e-159">Exemplo: `height:665px`</span><span class="sxs-lookup"><span data-stu-id="6266e-159">Example: `height:665px`</span></span> |  
 
<span data-ttu-id="6266e-160">Outros atributos de posição, como `z-index`, são ignorados.</span><span class="sxs-lookup"><span data-stu-id="6266e-160">Other position attributes, such as `z-index`, are ignored.</span></span> <span data-ttu-id="6266e-161">As imagens posicionadas absolutas podem usar o atributo `data-render-src` ou `src`.</span><span class="sxs-lookup"><span data-stu-id="6266e-161">Absolute positioned images can use either the `data-render-src` or `src` attribute.</span></span>


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="6266e-162">Informações de resposta</span><span class="sxs-lookup"><span data-stu-id="6266e-162">Response information</span></span>

<span data-ttu-id="6266e-163">A API do OneNote retorna as seguintes informações na resposta.</span><span class="sxs-lookup"><span data-stu-id="6266e-163">The OneNote API returns the following information in the response.</span></span>

| <span data-ttu-id="6266e-164">Dados de resposta</span><span class="sxs-lookup"><span data-stu-id="6266e-164">Response data</span></span> | <span data-ttu-id="6266e-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="6266e-165">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="6266e-166">Código de êxito</span><span class="sxs-lookup"><span data-stu-id="6266e-166">Success code</span></span> | <span data-ttu-id="6266e-167">Um código de status HTTP 201 para uma solicitação POST bem-sucedida e um código de status HTTP 204 para uma solicitação PATCH bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="6266e-167">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="6266e-168">Erros</span><span class="sxs-lookup"><span data-stu-id="6266e-168">Errors</span></span> | <span data-ttu-id="6266e-169">Leia [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote-error-codes.md) para saber mais sobre erros do OneNote que poderão ser retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6266e-169">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="6266e-170">Permissões</span><span class="sxs-lookup"><span data-stu-id="6266e-170">Permissions</span></span>

<span data-ttu-id="6266e-171">Para criar ou atualizar páginas do OneNote, solicite permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="6266e-171">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="6266e-172">Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="6266e-172">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="6266e-173">Permissões para páginas POST</span><span class="sxs-lookup"><span data-stu-id="6266e-173">Permissions for POST pages</span></span> 

- <span data-ttu-id="6266e-174">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="6266e-174">Notes.Create</span></span>
- <span data-ttu-id="6266e-175">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6266e-175">Notes.ReadWrite</span></span>
- <span data-ttu-id="6266e-176">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6266e-176">Notes.ReadWrite.All</span></span>  


#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="6266e-177">Permissões para páginas PATCH</span><span class="sxs-lookup"><span data-stu-id="6266e-177">Permissions for PATCH pages</span></span> 

- <span data-ttu-id="6266e-178">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6266e-178">Notes.ReadWrite</span></span>
- <span data-ttu-id="6266e-179">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6266e-179">Notes.ReadWrite.All</span></span>

<span data-ttu-id="6266e-180">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="6266e-180">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="6266e-181">Confira também</span><span class="sxs-lookup"><span data-stu-id="6266e-181">See also</span></span>

- [<span data-ttu-id="6266e-182">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="6266e-182">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="6266e-183">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="6266e-183">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="6266e-184">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="6266e-184">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="6266e-185">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="6266e-185">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="6266e-186">Perguntas sobre desenvolvimento do OneNote no Microsoft Q&A</span><span class="sxs-lookup"><span data-stu-id="6266e-186">OneNote development questions on Microsoft Q&A</span></span>](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="6266e-187">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="6266e-187">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  

