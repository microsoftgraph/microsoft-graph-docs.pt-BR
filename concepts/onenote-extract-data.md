---
title: 'Usar marcas DIV da API do OneNote para extrair dados de capturas '
description: " Notebooks empresariais no Microsoft 365"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 601ada5a98e42aeb1e0e1eb19dfd225451a6a27d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474964"
---
# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a><span data-ttu-id="c45ec-103">Usar marcas DIV da API do OneNote para extrair dados de capturas</span><span class="sxs-lookup"><span data-stu-id="c45ec-103">Use OneNote API div tags to extract data from captures</span></span> 

<span data-ttu-id="c45ec-104">**Aplica-se a** notebooks do consumidor no OneDrive | Notebooks empresariais no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c45ec-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="c45ec-105">Use a API do OneNote para extrair dados do cartão de visitas de uma imagem ou dados de receita e produto de uma URL.</span><span class="sxs-lookup"><span data-stu-id="c45ec-105">Use the OneNote API to extract business card data from an image, or recipe and product data from a URL.</span></span>

<a name="attributes"></a>

## <a name="extraction-attributes"></a><span data-ttu-id="c45ec-106">Atributos de extração</span><span class="sxs-lookup"><span data-stu-id="c45ec-106">Extraction attributes</span></span>

<span data-ttu-id="c45ec-107">Para extrair e transformar dados, basta incluir um div que especifique o conteúdo de origem, o método de extração e o comportamento de fallback na sua solicitação [create-page](onenote-create-page.md) ou [update-page](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="c45ec-107">To extract and transform data, simply include a div that specifies the source content, extraction method, and fallback behavior in your [create-page](onenote-create-page.md) or [update-page](onenote-update-page.md) request.</span></span> <span data-ttu-id="c45ec-108">A API processa dados extraídos da página em um formato que é fácil de ler.</span><span class="sxs-lookup"><span data-stu-id="c45ec-108">The API renders extracted data on the page in an easy-to-read format.</span></span> 

```html
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

### <a name="data-render-src"></a><span data-ttu-id="c45ec-109">data-render-src</span><span class="sxs-lookup"><span data-stu-id="c45ec-109">data-render-src</span></span>

<span data-ttu-id="c45ec-110">A fonte de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c45ec-110">The content source.</span></span> <span data-ttu-id="c45ec-111">Pode ser uma imagem de um cartão de visitas ou uma URL absoluta de muitos sites populares de receitas ou produtos.</span><span class="sxs-lookup"><span data-stu-id="c45ec-111">This can be an image of a business card or an absolute URL from many popular recipe or product websites.</span></span> <span data-ttu-id="c45ec-112">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c45ec-112">Required.</span></span>

<span data-ttu-id="c45ec-113">Para obter melhores resultados ao especificar uma URL, use a URL canônica definida no HTML da página da Web de origem, caso houver uma URL definida.</span><span class="sxs-lookup"><span data-stu-id="c45ec-113">For best results when specifying a URL, use the canonical URL defined in the HTML of the source webpage, if one is defined.</span></span> <span data-ttu-id="c45ec-114">Por exemplo, uma URL canônica pode estar definida na página da Web de origem da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="c45ec-114">For example, a canonical URL might be defined in the source webpage like this:</span></span>

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


### <a name="data-render-method"></a><span data-ttu-id="c45ec-115">data-render-method</span><span class="sxs-lookup"><span data-stu-id="c45ec-115">data-render-method</span></span>

<span data-ttu-id="c45ec-116">O método de extração a ser executado.</span><span class="sxs-lookup"><span data-stu-id="c45ec-116">The extraction method to run.</span></span> <span data-ttu-id="c45ec-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c45ec-117">Required.</span></span>

| <span data-ttu-id="c45ec-118">Valor</span><span class="sxs-lookup"><span data-stu-id="c45ec-118">Value</span></span> | <span data-ttu-id="c45ec-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c45ec-119">Description</span></span> |
|:------|:------|
| <span data-ttu-id="c45ec-120">extract.businesscard</span><span class="sxs-lookup"><span data-stu-id="c45ec-120">extract.businesscard</span></span> | <span data-ttu-id="c45ec-121">A extração de um cartão de visita.</span><span class="sxs-lookup"><span data-stu-id="c45ec-121">A business card extraction.</span></span> |
| <span data-ttu-id="c45ec-122">extract.recipe</span><span class="sxs-lookup"><span data-stu-id="c45ec-122">extract.recipe</span></span> | <span data-ttu-id="c45ec-123">Uma extração de receita.</span><span class="sxs-lookup"><span data-stu-id="c45ec-123">A recipe extraction.</span></span> |
| <span data-ttu-id="c45ec-124">extract.product</span><span class="sxs-lookup"><span data-stu-id="c45ec-124">extract.product</span></span> | <span data-ttu-id="c45ec-125">A extração de uma lista de produtos.</span><span class="sxs-lookup"><span data-stu-id="c45ec-125">A product listing extraction.</span></span> |
| <span data-ttu-id="c45ec-126">extract</span><span class="sxs-lookup"><span data-stu-id="c45ec-126">extract</span></span> | <span data-ttu-id="c45ec-127">Um tipo de extração desconhecida.</span><span class="sxs-lookup"><span data-stu-id="c45ec-127">An unknown extraction type.</span></span> |

<span data-ttu-id="c45ec-128">Para obter melhores resultados, especifique o tipo de conteúdo (`extract.businesscard`, `extract.recipe` ou `extract.product`) se você conhecê-lo.</span><span class="sxs-lookup"><span data-stu-id="c45ec-128">For best results, specify the content type (`extract.businesscard`, `extract.recipe`, or `extract.product`) if you know it.</span></span> <span data-ttu-id="c45ec-129">Se o tipo for desconhecido, use o método `extract` e a API do OneNote tentará detectar o tipo automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c45ec-129">If the type is unknown, use the `extract` method, and the OneNote API will try to auto-detect the type.</span></span>

### <a name="data-render-fallback"></a><span data-ttu-id="c45ec-130">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="c45ec-130">data-render-fallback</span></span>

<span data-ttu-id="c45ec-131">O comportamento de fallback se a extração falhar.</span><span class="sxs-lookup"><span data-stu-id="c45ec-131">The fallback behavior if the extraction fails.</span></span> <span data-ttu-id="c45ec-132">Usa o padrão **renderizar** caso seja omitido.</span><span class="sxs-lookup"><span data-stu-id="c45ec-132">Defaults to **render** if omitted.</span></span> 

| <span data-ttu-id="c45ec-133">Valor</span><span class="sxs-lookup"><span data-stu-id="c45ec-133">Value</span></span> | <span data-ttu-id="c45ec-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c45ec-134">Description</span></span> |
|:------|:------|
| <span data-ttu-id="c45ec-135">render</span><span class="sxs-lookup"><span data-stu-id="c45ec-135">render</span></span> | <span data-ttu-id="c45ec-136">Renderiza a imagem de origem ou um instantâneo da página do produto ou receita.</span><span class="sxs-lookup"><span data-stu-id="c45ec-136">Renders the source image or a snapshot of the recipe or product webpage.</span></span> |
| <span data-ttu-id="c45ec-137">nenhum</span><span class="sxs-lookup"><span data-stu-id="c45ec-137">none</span></span> | <span data-ttu-id="c45ec-138">Não faz nada.</span><span class="sxs-lookup"><span data-stu-id="c45ec-138">Does nothing.</span></span><br /><br /><span data-ttu-id="c45ec-139">Essa opção é útil se você quiser sempre incluir um instantâneo do cartão de visitas ou da página da Web na página, além de outro conteúdo extraído.</span><span class="sxs-lookup"><span data-stu-id="c45ec-139">This option is useful if you want to always include a snapshot of the business card or webpage on the page in addition to any extracted content.</span></span> <span data-ttu-id="c45ec-140">Certifique-se enviar um elemento `img` separado na solicitação, conforme mostrado nos exemplos.</span><span class="sxs-lookup"><span data-stu-id="c45ec-140">Be sure to send a separate `img` element in the request, as shown in the examples.</span></span> |

<a name="biz-card"></a>

## <a name="business-card-extractions"></a><span data-ttu-id="c45ec-141">Extrações de cartões de visita</span><span class="sxs-lookup"><span data-stu-id="c45ec-141">Business card extractions</span></span>

<span data-ttu-id="c45ec-142">A API do OneNote tenta localizar e renderizar as seguintes informações de contato com base em uma imagem do cartão de visitas de uma pessoa ou empresa.</span><span class="sxs-lookup"><span data-stu-id="c45ec-142">The OneNote API tries to find and render the following contact information based on an image of a person's or company's business card.</span></span>

- <span data-ttu-id="c45ec-143">Nome</span><span class="sxs-lookup"><span data-stu-id="c45ec-143">Name</span></span>
- <span data-ttu-id="c45ec-144">Título</span><span class="sxs-lookup"><span data-stu-id="c45ec-144">Title</span></span>
- <span data-ttu-id="c45ec-145">Organização</span><span class="sxs-lookup"><span data-stu-id="c45ec-145">Organization</span></span>
- <span data-ttu-id="c45ec-146">Números de telefone e fax</span><span class="sxs-lookup"><span data-stu-id="c45ec-146">Phone and fax numbers</span></span>
- <span data-ttu-id="c45ec-147">Endereços para correspondência e físicos</span><span class="sxs-lookup"><span data-stu-id="c45ec-147">Mailing and physical addresses</span></span>
- <span data-ttu-id="c45ec-148">Emails</span><span class="sxs-lookup"><span data-stu-id="c45ec-148">Email addresses</span></span>
- <span data-ttu-id="c45ec-149">Sites</span><span class="sxs-lookup"><span data-stu-id="c45ec-149">Websites</span></span>



<img alt="An example business card extraction" src="images/biz-card-extraction.png" width="200">

<span data-ttu-id="c45ec-150">Um vCard (arquivo .VCF) com as informações de contato extraídas também é incorporado na página.</span><span class="sxs-lookup"><span data-stu-id="c45ec-150">A vCard (.VCF file) with the extracted contact information is also embedded in the page.</span></span> <span data-ttu-id="c45ec-151">O vCard é uma maneira conveniente de obter as informações de contato ao recuperar o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="c45ec-151">The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span>

### <a name="common-scenarios-for-business-card-extractions"></a><span data-ttu-id="c45ec-152">Cenários comuns para extrações de cartões de visita</span><span class="sxs-lookup"><span data-stu-id="c45ec-152">Common scenarios for business card extractions</span></span>

#### <a name="extract-business-card-information-and-also-render-the-business-card-image"></a><span data-ttu-id="c45ec-153">Extrair informações do cartão de visitas e também renderizar a imagem do cartão de visitas</span><span class="sxs-lookup"><span data-stu-id="c45ec-153">Extract business card information, and also render the business card image</span></span>

<span data-ttu-id="c45ec-154">Especifique o método `extract.businesscard` e o fallback `none`.</span><span class="sxs-lookup"><span data-stu-id="c45ec-154">Specify the `extract.businesscard` method and the `none` fallback.</span></span> <span data-ttu-id="c45ec-155">Envie também um elemento `img` com o atributo `src` que também faz referência à imagem.</span><span class="sxs-lookup"><span data-stu-id="c45ec-155">Also send an `img` element with the `src` attribute that also references the image.</span></span> <span data-ttu-id="c45ec-156">Se a API não conseguir extrair conteúdo, ela renderizará apenas a imagem do cartão de visita.</span><span class="sxs-lookup"><span data-stu-id="c45ec-156">If the API is unable to extract any content, it renders the business card image only.</span></span>

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


#### <a name="extract-business-card-information-and-render-the-business-card-image-only-if-the-extraction-fails"></a><span data-ttu-id="c45ec-157">Extrair informações do cartão de visitas e renderizar a imagem do cartão de visitas apenas se a extração falhar</span><span class="sxs-lookup"><span data-stu-id="c45ec-157">Extract business card information, and render the business card image only if the extraction fails</span></span>

<span data-ttu-id="c45ec-158">Especifique o método `extract.businesscard` e use o fallback `render` padrão.</span><span class="sxs-lookup"><span data-stu-id="c45ec-158">Specify the `extract.businesscard` method and use the default `render` fallback.</span></span> <span data-ttu-id="c45ec-159">Se a API não conseguir extrair conteúdo, ela renderizará a imagem do cartão de visita.</span><span class="sxs-lookup"><span data-stu-id="c45ec-159">If the API is unable to extract any content, it renders the business card image instead.</span></span>

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
<span data-ttu-id="c45ec-160">Para extrações de cartão de visita, a imagem é enviada como uma parte nomeada em uma solicitação múltiplas.</span><span class="sxs-lookup"><span data-stu-id="c45ec-160">For business card extractions, the image is sent as a named part in a multipart request.</span></span> <span data-ttu-id="c45ec-161">Confira [Adicionar imagens e arquivos](onenote-images-files.md) para ver exemplos que mostram como enviar uma imagem em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c45ec-161">See [Add images and files](onenote-images-files.md) for examples that show how to send an image in a request.</span></span>


<a name="recipe"></a>

## <a name="recipe-extractions"></a><span data-ttu-id="c45ec-162">Extrações receitas</span><span class="sxs-lookup"><span data-stu-id="c45ec-162">Recipe extractions</span></span>

<span data-ttu-id="c45ec-163">A API do OneNote tenta localizar e renderizar as seguintes informações com base na URL de uma receita.</span><span class="sxs-lookup"><span data-stu-id="c45ec-163">The OneNote API tries to find and render the following information based on a recipe's URL.</span></span>

- <span data-ttu-id="c45ec-164">Imagem Hero</span><span class="sxs-lookup"><span data-stu-id="c45ec-164">Hero image</span></span>
- <span data-ttu-id="c45ec-165">Classificação</span><span class="sxs-lookup"><span data-stu-id="c45ec-165">Rating</span></span>
- <span data-ttu-id="c45ec-166">Ingredientes</span><span class="sxs-lookup"><span data-stu-id="c45ec-166">Ingredients</span></span>
- <span data-ttu-id="c45ec-167">Instruções</span><span class="sxs-lookup"><span data-stu-id="c45ec-167">Instructions</span></span>
- <span data-ttu-id="c45ec-168">Preparação, instruções sobre como cozinhar e tempos totais</span><span class="sxs-lookup"><span data-stu-id="c45ec-168">Prep, cook, and total times</span></span>
- <span data-ttu-id="c45ec-169">Porções</span><span class="sxs-lookup"><span data-stu-id="c45ec-169">Servings</span></span>


<img alt="An example recipe extraction" src="images/recipe-extraction.png" width="200">

<span data-ttu-id="c45ec-170">A API é otimizada para receitas de muitos sites populares, como *Allrecipes.com*, *FoodNetwork.com* e *SeriousEats.com*.</span><span class="sxs-lookup"><span data-stu-id="c45ec-170">The API is optimized for recipes from many popular sites such as *Allrecipes.com*, *FoodNetwork.com*, and *SeriousEats.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="c45ec-171">Cenários comuns para extrações de receitas</span><span class="sxs-lookup"><span data-stu-id="c45ec-171">Common scenarios for recipe extractions</span></span>

#### <a name="extract-recipe-information-and-also-render-a-snapshot-of-the-recipe-webpage"></a><span data-ttu-id="c45ec-172">Extrair informações da receita e também renderizar um instantâneo da página da receita</span><span class="sxs-lookup"><span data-stu-id="c45ec-172">Extract recipe information, and also render a snapshot of the recipe webpage</span></span>

<span data-ttu-id="c45ec-173">Especifique o método `extract.recipe` e o fallback `none`.</span><span class="sxs-lookup"><span data-stu-id="c45ec-173">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="c45ec-174">Envie também um elemento `img` com o atributo `data-render-src` definido como URL da receita.</span><span class="sxs-lookup"><span data-stu-id="c45ec-174">Also send an `img` element with the `data-render-src` attribute set to the recipe URL.</span></span> <span data-ttu-id="c45ec-175">Se a API não conseguir extrair conteúdo, ela renderizará apenas um instantâneo da página da Web da receita.</span><span class="sxs-lookup"><span data-stu-id="c45ec-175">If the API is unable to extract any content, it renders a snapshot of the recipe webpage only.</span></span>

<span data-ttu-id="c45ec-176">Este cenário potencialmente fornece mais informações porque a página da Web pode incluir informações adicionais, como comentários e sugestões de clientes.</span><span class="sxs-lookup"><span data-stu-id="c45ec-176">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="https://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="https://allrecipes.com/recipe/guacamole/" />
```
 

#### <a name="extract-recipe-information-and-render-a-snapshot-of-the-recipe-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="c45ec-177">Extrair informações da receita e renderizar um instantâneo da página da receita apenas se a extração falhar</span><span class="sxs-lookup"><span data-stu-id="c45ec-177">Extract recipe information, and render a snapshot of the recipe webpage only if the extraction fails</span></span>

<span data-ttu-id="c45ec-178">Especifique o método `extract.recipe` e use o fallback de renderização padrão.</span><span class="sxs-lookup"><span data-stu-id="c45ec-178">Specify the `extract.recipe` method and use the default render fallback.</span></span> <span data-ttu-id="c45ec-179">Se a API não conseguir extrair conteúdo, ela renderizará um instantâneo da página da Web da receita.</span><span class="sxs-lookup"><span data-stu-id="c45ec-179">If the API is unable to extract any content, it renders a snapshot of the recipe webpage instead.</span></span>

```html  
<div
    data-render-src="https://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


#### <a name="extract-recipe-information-and-also-render-a-link-to-the-recipe"></a><span data-ttu-id="c45ec-180">Extrair informações da receita e também renderizar um link para a receita</span><span class="sxs-lookup"><span data-stu-id="c45ec-180">Extract recipe information, and also render a link to the recipe</span></span>

<span data-ttu-id="c45ec-181">Especifique o método `extract.recipe` e o fallback `none`.</span><span class="sxs-lookup"><span data-stu-id="c45ec-181">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="c45ec-182">Envie também um elemento `a` com o atributo `src` definido com a URL da receita (ou você pode enviar qualquer outra informação que queira adicionar à página).</span><span class="sxs-lookup"><span data-stu-id="c45ec-182">Also send an `a` element with the `src` attribute set to the recipe URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="c45ec-183">Se a API não conseguir extrair conteúdo, apenas o link da receita será renderizado.</span><span class="sxs-lookup"><span data-stu-id="c45ec-183">If the API is unable to extract any content, only the recipe link is rendered.</span></span>

```html  
<div
    data-render-src="https://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="https://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>

## <a name="product-listing-extractions"></a><span data-ttu-id="c45ec-184">Extrações da lista de produtos</span><span class="sxs-lookup"><span data-stu-id="c45ec-184">Product listing extractions</span></span>

- <span data-ttu-id="c45ec-185">Título</span><span class="sxs-lookup"><span data-stu-id="c45ec-185">Title</span></span>
- <span data-ttu-id="c45ec-186">Classificação</span><span class="sxs-lookup"><span data-stu-id="c45ec-186">Rating</span></span>
- <span data-ttu-id="c45ec-187">Imagem principal</span><span class="sxs-lookup"><span data-stu-id="c45ec-187">Primary image</span></span>
- <span data-ttu-id="c45ec-188">Descrição</span><span class="sxs-lookup"><span data-stu-id="c45ec-188">Description</span></span>
- <span data-ttu-id="c45ec-189">Recursos</span><span class="sxs-lookup"><span data-stu-id="c45ec-189">Features</span></span>
- <span data-ttu-id="c45ec-190">Especificações</span><span class="sxs-lookup"><span data-stu-id="c45ec-190">Specifications</span></span>



<img alt="An example product listing extraction" src="images/product-extraction.png" width="200">

<span data-ttu-id="c45ec-191">A API é otimizada para produtos de muitos sites populares, como *Amazon.com* e *HomeDepot.com*.</span><span class="sxs-lookup"><span data-stu-id="c45ec-191">The API is optimized for products from many popular sites such as *Amazon.com* and *HomeDepot.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="c45ec-192">Cenários comuns para extrações de receitas</span><span class="sxs-lookup"><span data-stu-id="c45ec-192">Common scenarios for recipe extractions</span></span>

#### <a name="extract-product-information-and-also-render-a-snapshot-of-the-product-webpage"></a><span data-ttu-id="c45ec-193">Extrair informações do produto e também renderizar um instantâneo da página da Web do produto</span><span class="sxs-lookup"><span data-stu-id="c45ec-193">Extract product information, and also render a snapshot of the product webpage</span></span>

<span data-ttu-id="c45ec-194">Especifique o método `extract.product` e o fallback `none`.</span><span class="sxs-lookup"><span data-stu-id="c45ec-194">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="c45ec-195">Envie também um elemento `img` com o atributo `data-render-src` definido como URL do produto.</span><span class="sxs-lookup"><span data-stu-id="c45ec-195">Also send an `img` element with the `data-render-src` attribute set to the product URL.</span></span> <span data-ttu-id="c45ec-196">Se a API não conseguir extrair conteúdo, ela renderizará apenas um instantâneo da página da Web do produto.</span><span class="sxs-lookup"><span data-stu-id="c45ec-196">If the API is unable to extract any content, it renders a snapshot of the product webpage only.</span></span>

<span data-ttu-id="c45ec-197">Este cenário potencialmente fornece mais informações porque a página da Web pode incluir informações adicionais, como comentários e sugestões de clientes.</span><span class="sxs-lookup"><span data-stu-id="c45ec-197">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="https://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="https://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


#### <a name="extract-product-information-and-render-a-snapshot-of-the-product-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="c45ec-198">Extrair informações do produto e renderizar um instantâneo da página do produto apenas se a extração falhar</span><span class="sxs-lookup"><span data-stu-id="c45ec-198">Extract product information, and render a snapshot of the product webpage only if the extraction fails</span></span>

<span data-ttu-id="c45ec-199">Especifique o método `extract.product` e use o fallback de renderização padrão.</span><span class="sxs-lookup"><span data-stu-id="c45ec-199">Specify the `extract.product` method and use the default render fallback.</span></span> <span data-ttu-id="c45ec-200">Se a API não conseguir extrair conteúdo, ela renderizará um instantâneo da página da Web do produto.</span><span class="sxs-lookup"><span data-stu-id="c45ec-200">If the API is unable to extract any content, it renders a snapshot of the product webpage instead.</span></span>

```html 
<div
    data-render-src="https://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

#### <a name="extract-product-information-and-also-render-a-link-to-the-product"></a><span data-ttu-id="c45ec-201">Extrair informações do produto e também renderizar um link para o produto</span><span class="sxs-lookup"><span data-stu-id="c45ec-201">Extract product information, and also render a link to the product</span></span>

<span data-ttu-id="c45ec-202">Especifique o método `extract.product` e o fallback `none`.</span><span class="sxs-lookup"><span data-stu-id="c45ec-202">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="c45ec-203">Envie também um elemento `a` com o atributo `src` definido com a URL do produto (ou você pode enviar qualquer outra informação que queira adicionar à página).</span><span class="sxs-lookup"><span data-stu-id="c45ec-203">Also send an `a` element with the `src` attribute set to the product URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="c45ec-204">Se a API não conseguir extrair conteúdo, apenas o link da página será renderizado.</span><span class="sxs-lookup"><span data-stu-id="c45ec-204">If the API is unable to extract any content, only the page link is rendered.</span></span>

```html 
<div
    data-render-src="https://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="https://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 

## <a name="unknown-content-type-extractions"></a><span data-ttu-id="c45ec-205">Extrações de tipos de conteúdo desconhecidos</span><span class="sxs-lookup"><span data-stu-id="c45ec-205">Unknown content type extractions</span></span>

<span data-ttu-id="c45ec-206">Se você não souber o tipo de conteúdo (cartão de visita, receita ou produto) que está enviando, poderá usar o método não qualificado `extract` e permitir que a API do OneNote detecte automaticamente o tipo.</span><span class="sxs-lookup"><span data-stu-id="c45ec-206">If you don't know the content type (business card, recipe, or product) that you're sending, you can use the unqualified `extract` method and let the OneNote API automatically detect the type.</span></span> <span data-ttu-id="c45ec-207">É provável que você queira fazer isso se seu aplicativo enviar diferentes tipos de captura.</span><span class="sxs-lookup"><span data-stu-id="c45ec-207">You might want to do this if your app sends different capture types.</span></span>

> <span data-ttu-id="c45ec-208">**Observação:** se você souber o tipo de conteúdo que está enviando, use o método `extract.businesscard`, `extract.recipe` ou `extract.product`.</span><span class="sxs-lookup"><span data-stu-id="c45ec-208">**Note:** If you do know the content type that you're sending, you should use the `extract.businesscard`, `extract.recipe`, or `extract.product` method.</span></span> <span data-ttu-id="c45ec-209">Em alguns casos, isso pode ajudar a otimizar os resultados da extração.</span><span class="sxs-lookup"><span data-stu-id="c45ec-209">In some cases, this can help to optimize the extraction results.</span></span>
 
### <a name="common-scenarios-for-unknown-extractions"></a><span data-ttu-id="c45ec-210">Cenários comuns para extrações desconhecidas</span><span class="sxs-lookup"><span data-stu-id="c45ec-210">Common scenarios for unknown extractions</span></span>

#### <a name="send-an-image-or-a-url-and-render-the-supplied-image-or-a-snapshot-of-the-webpage-if-the-extraction-fails"></a><span data-ttu-id="c45ec-211">Enviar uma imagem ou uma URL e renderizar a imagem fornecida ou um instantâneo da página da Web se a extração falhar</span><span class="sxs-lookup"><span data-stu-id="c45ec-211">Send an image or a URL, and render the supplied image or a snapshot of the webpage if the extraction fails</span></span>

<span data-ttu-id="c45ec-212">Especifique o método `extract` para que a API detecte automaticamente o tipo de conteúdo e use o fallback de renderização padrão.</span><span class="sxs-lookup"><span data-stu-id="c45ec-212">Specify the `extract` method so the API automatically detects the content type, and use the default render fallback.</span></span> <span data-ttu-id="c45ec-213">Se a API não conseguir extrair conteúdo, ela renderizará a imagem fornecida ou o instantâneo da página da Web.</span><span class="sxs-lookup"><span data-stu-id="c45ec-213">If the API is unable to extract any content, it renders the supplied image or snapshot of the webpage instead.</span></span>

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="c45ec-214">Informações de resposta</span><span class="sxs-lookup"><span data-stu-id="c45ec-214">Response information</span></span>

| <span data-ttu-id="c45ec-215">Dados de resposta</span><span class="sxs-lookup"><span data-stu-id="c45ec-215">Response data</span></span> | <span data-ttu-id="c45ec-216">Descrição</span><span class="sxs-lookup"><span data-stu-id="c45ec-216">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c45ec-217">Código de êxito</span><span class="sxs-lookup"><span data-stu-id="c45ec-217">Success code</span></span> | <span data-ttu-id="c45ec-218">Um código de status HTTP 201 para uma solicitação POST bem-sucedida e um código de status HTTP 204 para uma solicitação PATCH bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c45ec-218">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="c45ec-219">Erros</span><span class="sxs-lookup"><span data-stu-id="c45ec-219">Errors</span></span>| <span data-ttu-id="c45ec-220">Leia [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote-error-codes.md) para saber mais sobre erros do OneNote que poderão ser retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c45ec-220">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="c45ec-221">Permissões</span><span class="sxs-lookup"><span data-stu-id="c45ec-221">Permissions</span></span>

<span data-ttu-id="c45ec-222">Para criar ou atualizar páginas do OneNote, solicite permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="c45ec-222">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="c45ec-223">Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="c45ec-223">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="c45ec-224">Permissões para páginas POST</span><span class="sxs-lookup"><span data-stu-id="c45ec-224">Permissions for POST pages</span></span>

- <span data-ttu-id="c45ec-225">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="c45ec-225">Notes.Create</span></span>
- <span data-ttu-id="c45ec-226">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c45ec-226">Notes.ReadWrite</span></span>
- <span data-ttu-id="c45ec-227">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c45ec-227">Notes.ReadWrite.All</span></span>  

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="c45ec-228">Permissões para páginas PATCH</span><span class="sxs-lookup"><span data-stu-id="c45ec-228">Permissions for PATCH pages</span></span>

- <span data-ttu-id="c45ec-229">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c45ec-229">Notes.ReadWrite</span></span>
- <span data-ttu-id="c45ec-230">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c45ec-230">Notes.ReadWrite.All</span></span>

<span data-ttu-id="c45ec-231">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Referência de permissões do Microsoft Graph](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c45ec-231">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="c45ec-232">Confira também</span><span class="sxs-lookup"><span data-stu-id="c45ec-232">See also</span></span>

- [<span data-ttu-id="c45ec-233">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="c45ec-233">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="c45ec-234">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="c45ec-234">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="c45ec-235">Adicionar imagens e arquivos</span><span class="sxs-lookup"><span data-stu-id="c45ec-235">Add images and files</span></span>](onenote-images-files.md)
- [<span data-ttu-id="c45ec-236">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="c45ec-236">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="c45ec-237">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="c45ec-237">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="c45ec-238">Perguntas sobre desenvolvimento do OneNote no Microsoft Q&A</span><span class="sxs-lookup"><span data-stu-id="c45ec-238">OneNote development questions on Microsoft Q&A</span></span>](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="c45ec-239">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="c45ec-239">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  

