
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a><span data-ttu-id="3f66b-101">Criar elementos posicionados absolutos nas páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="3f66b-101">Create absolute positioned elements in OneNote pages</span></span>

<span data-ttu-id="3f66b-102">O corpo de uma página do OneNote pode conter vários elementos filhos diretos `div`, `img` e `object` que podem ser posicionados de forma independente na página.</span><span class="sxs-lookup"><span data-stu-id="3f66b-102">The body of a OneNote page can contain multiple direct `div`, `img`, and `object` child elements that can be positioned independently on the page.</span></span>

<a name="attributes"></a>
## <a name="attributes-and-positioning-behavior"></a><span data-ttu-id="3f66b-103">Atributos e comportamento de posicionamento</span><span class="sxs-lookup"><span data-stu-id="3f66b-103">Attributes and positioning behavior</span></span>

<span data-ttu-id="3f66b-104">Use os atributos `data-absolute-enabled` e [`style`](#supported-css-style-attributes) para criar elementos posicionados absolutos em uma página, da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="3f66b-104">Use the `data-absolute-enabled` and [`style`](#supported-css-style-attributes) attributes to create absolute positioned elements on a page, as follows:</span></span>

- <span data-ttu-id="3f66b-105">O elemento do corpo deve especificar `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="3f66b-105">The body element must specify `data-absolute-enabled="true"`.</span></span> <span data-ttu-id="3f66b-106">Se omitido ou definido como `false`, todo o conteúdo do corpo será processado dentro de um div posicionado absoluto `_default` que a API cria e todas as configurações de posição serão ignoradas.</span><span class="sxs-lookup"><span data-stu-id="3f66b-106">If omitted or set to `false`, all body content is rendered inside a `_default` absolute positioned div that the API creates, and all position settings are ignored.</span></span>

- <span data-ttu-id="3f66b-107">Apenas os elementos `div`, `img` e `object` podem incluir elementos posicionados absolutos.</span><span class="sxs-lookup"><span data-stu-id="3f66b-107">Only `div`, `img`, and `object` elements can be absolute positioned elements.</span></span> 

- <span data-ttu-id="3f66b-108">Os elementos posicionados absolutos devem especificar `style="position:absolute"`.</span><span class="sxs-lookup"><span data-stu-id="3f66b-108">Absolute positioned elements must specify `style="position:absolute"`.</span></span>

- <span data-ttu-id="3f66b-109">Os elementos posicionados absolutos devem ser filhos diretos do elemento `body`.</span><span class="sxs-lookup"><span data-stu-id="3f66b-109">Absolute positioned elements must be direct children of the `body` element.</span></span> <span data-ttu-id="3f66b-110">Quaisquer filhos diretos do corpo que não sejam elementos posicionados absolutos `div`, `img` ou `object` serão processados como conteúdo estático no div posicionado absoluto `_default`.</span><span class="sxs-lookup"><span data-stu-id="3f66b-110">Any direct children of the body that aren't absolute positioned `div`, `img`, or `object` elements are rendered as static content inside the absolute positioned `_default` div.</span></span>

- <span data-ttu-id="3f66b-111">Os elementos posicionados absolutos são colocados nas coordenadas especificadas superiores e esquerdas, relativas à posição inicial 0:0 no canto superior esquerdo da página, acima da área de título.</span><span class="sxs-lookup"><span data-stu-id="3f66b-111">Absolute positioned elements are positioned at their specified top and left coordinates, relative to the 0:0 starting position at the top, left corner of the page above the title area.</span></span>

- <span data-ttu-id="3f66b-112">Quando um elemento com posicionamento absoluto omite coordenada esquerda ou superior, a coordenada ausente está definida com o valor padrão: `top:120px` ou `left:48px`.</span><span class="sxs-lookup"><span data-stu-id="3f66b-112">If an absolute positioned element omits the top or left coordinate, the missing coordinate is set to its default value: `top:120px` or `left:48px`.</span></span> <span data-ttu-id="3f66b-113">Essas coordenadas padrão especificam uma posição abaixo da área de título.</span><span class="sxs-lookup"><span data-stu-id="3f66b-113">These default coordinates specify a position just below the title area.</span></span> <span data-ttu-id="3f66b-114">Lembre-se de que omitir coordenadas pode resultar em elementos empilhados.</span><span class="sxs-lookup"><span data-stu-id="3f66b-114">Be aware that omitting coordinates can result in elements that are stacked on top of each other.</span></span>

- <span data-ttu-id="3f66b-115">Os elementos posicionados absolutos não podem ser aninhados, nem conter elementos posicionados.</span><span class="sxs-lookup"><span data-stu-id="3f66b-115">Absolute positioned elements cannot be nested or contain positioned elements.</span></span> <span data-ttu-id="3f66b-116">A API ignora as configurações de posição especificadas em elementos aninhados dentro do div posicionado absoluto, processa o conteúdo aninhado dentro do div pai posicionado absoluto e retorna um aviso na propriedade **api.diagnostics** na resposta.</span><span class="sxs-lookup"><span data-stu-id="3f66b-116">The API ignores any position settings specified on nested elements inside an absolute positioned div, renders the nested content inside the absolute positioned parent div, and returns a warning in the **api.diagnostics** property in the response.</span></span>


# <a name="example"></a><span data-ttu-id="3f66b-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f66b-117">Example</span></span>

 <span data-ttu-id="3f66b-118">O exemplo a seguir contém um filho `p` direto, um div posicionado absoluto e um div posicionado não absoluto.</span><span class="sxs-lookup"><span data-stu-id="3f66b-118">The following example contains a direct `p` child, an absolute positioned div, and a non-absolute positioned div.</span></span>

## <a name="input-html"></a><span data-ttu-id="3f66b-119">HTML de entrada</span><span class="sxs-lookup"><span data-stu-id="3f66b-119">Input HTML</span></span>  

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

<span data-ttu-id="3f66b-120">A API processa o div posicionado não absoluto no div padrão.</span><span class="sxs-lookup"><span data-stu-id="3f66b-120">The API renders the non-absolute positioned div in the default div.</span></span> <span data-ttu-id="3f66b-121">Observe que as marcas aninhadas `<div>` são descartadas porque não definem informações semânticas (como `data-id`).</span><span class="sxs-lookup"><span data-stu-id="3f66b-121">Note that the nested  `<div>` tags are discarded because they do not define any semantic information (such as `data-id`).</span></span>

## <a name="output-html"></a><span data-ttu-id="3f66b-122">HTML de saída</span><span class="sxs-lookup"><span data-stu-id="3f66b-122">Output HTML</span></span> 

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

## <a name="example"></a><span data-ttu-id="3f66b-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f66b-123">Example</span></span>

 <span data-ttu-id="3f66b-124">O exemplo a seguir cria uma página que contém um div posicionado absoluto e uma imagem posicionada absoluta.</span><span class="sxs-lookup"><span data-stu-id="3f66b-124">The following example creates a page that contains one absolute positioned div and one absolute positioned image.</span></span>


### <a name="input-html"></a><span data-ttu-id="3f66b-125">HTML de entrada</span><span class="sxs-lookup"><span data-stu-id="3f66b-125">Input HTML</span></span>  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="http://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="http://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
<span data-ttu-id="3f66b-126">A API do OneNote avalia o HTML de entrada e preserva todo o conteúdo semântico e qualquer informação estrutural compatível com o OneNote.</span><span class="sxs-lookup"><span data-stu-id="3f66b-126">The OneNote API evaluates the input HTML and preserves all semantic content and any structural information that is supported by OneNote.</span></span> <span data-ttu-id="3f66b-127">A página resultante processa conforme mostrado na imagem a seguir, mas sem as bordas visíveis do div e da imagem.</span><span class="sxs-lookup"><span data-stu-id="3f66b-127">The resulting page renders as shown in the following image (but without the visible borders for the div and image).</span></span> 

![A página resultante com o div posicionado absoluto e a imagem](images/abs-pos.PNG)

<span data-ttu-id="3f66b-129">Observe as alterações no div aninhado não contribuidor do HTML de entrada.</span><span class="sxs-lookup"><span data-stu-id="3f66b-129">Notice the changes to the non-contributing, nested div from the input HTML.</span></span> <span data-ttu-id="3f66b-130">A API preserva o conteúdo do div, mas descarta as marcas `<div>` porque o div não define informações semânticas (como `data-id`).</span><span class="sxs-lookup"><span data-stu-id="3f66b-130">The API preserves the div's content but discards the `<div>` tags because the div doesn't define semantic information (such as `data-id`).</span></span>

<span data-ttu-id="3f66b-131">Saiba mais sobre como a API do OneNote lida com HTML de entrada e saída em [HTML de entrada e de saída para páginas do OneNote](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="3f66b-131">For more information about how the OneNote API handles input and output HTML, see [Input and output HTML for OneNote pages](onenote_input_output_html.md).</span></span>

<a name="style-attributes"></a>
### <a name="supported-css-style-attributes"></a><span data-ttu-id="3f66b-132">Atributos de estilos CSS compatíveis</span><span class="sxs-lookup"><span data-stu-id="3f66b-132">Supported CSS style attributes</span></span>

<span data-ttu-id="3f66b-133">Todos os elementos posicionados absolutos podem especificar as posições superiores e esquerdas.</span><span class="sxs-lookup"><span data-stu-id="3f66b-133">All absolute positioned elements can specify top and left positions.</span></span> <span data-ttu-id="3f66b-134">Divs e imagens podem especificar a largura e as imagens também podem especificar a altura.</span><span class="sxs-lookup"><span data-stu-id="3f66b-134">Divs and images can specify width, and images can also specify height.</span></span> <span data-ttu-id="3f66b-135">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="3f66b-135">For example:</span></span>

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| <span data-ttu-id="3f66b-136">Atributo</span><span class="sxs-lookup"><span data-stu-id="3f66b-136">Attribute</span></span> | <span data-ttu-id="3f66b-137">Elemento compatível</span><span class="sxs-lookup"><span data-stu-id="3f66b-137">Supported element</span></span> | <span data-ttu-id="3f66b-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f66b-138">Description</span></span> |  
|:------|:------|:------|  
| <span data-ttu-id="3f66b-139">top</span><span class="sxs-lookup"><span data-stu-id="3f66b-139">top</span></span> | <span data-ttu-id="3f66b-140">div, img, object</span><span class="sxs-lookup"><span data-stu-id="3f66b-140">div, img, object</span></span> | <span data-ttu-id="3f66b-141">A coordenada do eixo Y da borda superior do elemento, somente em pixels.</span><span class="sxs-lookup"><span data-stu-id="3f66b-141">The y-axis coordinate of the element's top border, in pixels only.</span></span> <span data-ttu-id="3f66b-142">O padrão é 120 pixels.</span><span class="sxs-lookup"><span data-stu-id="3f66b-142">Default is 120 pixels.</span></span><p><span data-ttu-id="3f66b-143">Exemplo: `top:140px`</span><span class="sxs-lookup"><span data-stu-id="3f66b-143">Example: `top:140px`</span></span></p> |  
| <span data-ttu-id="3f66b-144">left</span><span class="sxs-lookup"><span data-stu-id="3f66b-144">left</span></span> |  <span data-ttu-id="3f66b-145">div, img, object</span><span class="sxs-lookup"><span data-stu-id="3f66b-145">div, img, object</span></span>  | <span data-ttu-id="3f66b-146">A coordenada do eixo X da borda esquerda do elemento, somente em pixels.</span><span class="sxs-lookup"><span data-stu-id="3f66b-146">The x-axis coordinate of the element's left border, in pixels only.</span></span> <span data-ttu-id="3f66b-147">O padrão é 48 pixels.</span><span class="sxs-lookup"><span data-stu-id="3f66b-147">Default is 48 pixels.</span></span><p><span data-ttu-id="3f66b-148">Exemplo: `left:95px`</span><span class="sxs-lookup"><span data-stu-id="3f66b-148">Example: `left:95px`</span></span></p> |  
| <span data-ttu-id="3f66b-149">width</span><span class="sxs-lookup"><span data-stu-id="3f66b-149">width</span></span> |  <span data-ttu-id="3f66b-150">div, img</span><span class="sxs-lookup"><span data-stu-id="3f66b-150">div, img</span></span>  | <span data-ttu-id="3f66b-151">A largura do elemento, somente em pixels.</span><span class="sxs-lookup"><span data-stu-id="3f66b-151">The width of the thumbnail, in pixels.</span></span><p><span data-ttu-id="3f66b-152">Exemplo: `width:480px`</span><span class="sxs-lookup"><span data-stu-id="3f66b-152">Example: `width:480px`</span></span></p> |  
| <span data-ttu-id="3f66b-153">height</span><span class="sxs-lookup"><span data-stu-id="3f66b-153">height</span></span> | <span data-ttu-id="3f66b-154">img</span><span class="sxs-lookup"><span data-stu-id="3f66b-154">img</span></span> | <span data-ttu-id="3f66b-155">A altura do elemento, somente em pixels.</span><span class="sxs-lookup"><span data-stu-id="3f66b-155">The height of the thumbnail, in pixels.</span></span> <span data-ttu-id="3f66b-156">Para divs, a altura é calculada no tempo de execução e qualquer valor de altura especificado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="3f66b-156">For divs, height is calculated at runtime and any specified height value is ignored.</span></span><p><span data-ttu-id="3f66b-157">Exemplo: `height:665px`</span><span class="sxs-lookup"><span data-stu-id="3f66b-157">Example: `height:665px`</span></span></p> |  
 
<span data-ttu-id="3f66b-158">Outros atributos de posição, como `z-index`, são ignorados.</span><span class="sxs-lookup"><span data-stu-id="3f66b-158">Other position attributes, such as `z-index`, are ignored.</span></span> <span data-ttu-id="3f66b-159">As imagens posicionadas absolutas podem usar o atributo `data-render-src` ou `src`.</span><span class="sxs-lookup"><span data-stu-id="3f66b-159">Absolute positioned images can use either the `data-render-src` or `src` attribute.</span></span>


<a name="request-response-info"></a>
## <a name="response-information"></a><span data-ttu-id="3f66b-160">Informações de resposta</span><span class="sxs-lookup"><span data-stu-id="3f66b-160">Response information</span></span>
<span data-ttu-id="3f66b-161">A API do OneNote retorna as seguintes informações na resposta.</span><span class="sxs-lookup"><span data-stu-id="3f66b-161">The OneNote API returns the following information in the response.</span></span>

| <span data-ttu-id="3f66b-162">Dados de resposta</span><span class="sxs-lookup"><span data-stu-id="3f66b-162">Response data</span></span> | <span data-ttu-id="3f66b-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f66b-163">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="3f66b-164">Código de êxito</span><span class="sxs-lookup"><span data-stu-id="3f66b-164">Success code</span></span> | <span data-ttu-id="3f66b-165">Um código de status HTTP 201 para uma solicitação POST bem-sucedida e um código de status HTTP 204 para uma solicitação PATCH bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="3f66b-165">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="3f66b-166">Erros</span><span class="sxs-lookup"><span data-stu-id="3f66b-166">Errors</span></span> | <span data-ttu-id="3f66b-167">Leia [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote_error_codes.md) para saber mais sobre erros do OneNote que poderão ser retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3f66b-167">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
  


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="3f66b-168">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f66b-168">Permissions</span></span>

<span data-ttu-id="3f66b-169">Para criar ou atualizar páginas do OneNote, solicite permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="3f66b-169">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="3f66b-170">Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="3f66b-170">Choose the lowest level of permissions that your app needs to do its work.</span></span>

### <a name="permissions-for-post-pages"></a><span data-ttu-id="3f66b-171">Permissões para _páginas POST_</span><span class="sxs-lookup"><span data-stu-id="3f66b-171">Permissions for _POST pages_</span></span> 
- <span data-ttu-id="3f66b-172">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="3f66b-172">Notes.Create</span></span>
- <span data-ttu-id="3f66b-173">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f66b-173">Notes.ReadWrite</span></span>
- <span data-ttu-id="3f66b-174">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f66b-174">Notes.ReadWrite.All</span></span>  


### <a name="permissions-for-patch-pages"></a><span data-ttu-id="3f66b-175">Permissões para _páginas PATCH_</span><span class="sxs-lookup"><span data-stu-id="3f66b-175">Permissions for _PATCH pages_</span></span> 

- <span data-ttu-id="3f66b-176">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f66b-176">Notes.ReadWrite</span></span>
- <span data-ttu-id="3f66b-177">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f66b-177">Notes.ReadWrite.All</span></span>

<span data-ttu-id="3f66b-178">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="3f66b-178">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="3f66b-179">Recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="3f66b-179">Additional resources</span></span>

- [<span data-ttu-id="3f66b-180">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="3f66b-180">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="3f66b-181">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="3f66b-181">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="3f66b-182">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="3f66b-182">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="3f66b-183">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="3f66b-183">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="3f66b-184">Perguntas sobre desenvolvimento do OneNote no Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="3f66b-184">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="3f66b-185">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="3f66b-185">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  

