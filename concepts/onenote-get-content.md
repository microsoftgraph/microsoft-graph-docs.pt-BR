---
title: Obter a estrutura e o conteúdo do OneNote com o Microsoft Graph
description: " Blocos de anotações empresariais no Microsoft 365"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: f3e40662d2e750514ef6c71b3faa604e13ccc773
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921655"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="c6a72-103">Obter a estrutura e o conteúdo do OneNote com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c6a72-103">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="c6a72-104">**Aplica-se a**: Blocos de anotações de consumidor no OneDrive | Blocos de anotações empresariais no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c6a72-104">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="c6a72-105">Para obter a estrutura e o conteúdo do OneNote, envie uma solicitação GET ao ponto de extremidade de destino.</span><span class="sxs-lookup"><span data-stu-id="c6a72-105">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="c6a72-106">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="c6a72-106">For example:</span></span>

`GET ../onenote/pages/{id}`

<span data-ttu-id="c6a72-107">Se a solicitação for bem-sucedida, o Microsoft Graph retornará um código de status de HTTP 200 e as entidades ou o conteúdo que você solicitou.</span><span class="sxs-lookup"><span data-stu-id="c6a72-107">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="c6a72-108">As entidades do OneNote são retornadas como objetos JSON que estão em conformidade com a especificação OData versão 4.0.</span><span class="sxs-lookup"><span data-stu-id="c6a72-108">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="c6a72-109">Usando as opções de cadeia de caracteres de consulta, você pode filtrar as consultas e melhorar o desempenho.</span><span class="sxs-lookup"><span data-stu-id="c6a72-109">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="c6a72-110">Construir a URI de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6a72-110">Construct the request URI</span></span>

<span data-ttu-id="c6a72-111">Para construir a URI de solicitação, comece com a URL raiz do serviço:</span><span class="sxs-lookup"><span data-stu-id="c6a72-111">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="c6a72-112">Em seguida, acrescente o ponto de extremidade do recurso que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="c6a72-112">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="c6a72-113">(Os [caminhos recurso](#resource-paths-for-get-requests) são mostrados na próxima seção).</span><span class="sxs-lookup"><span data-stu-id="c6a72-113">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>

<span data-ttu-id="c6a72-114">Sua URI de solicitação completa parecerá com um dos seguintes exemplos:</span><span class="sxs-lookup"><span data-stu-id="c6a72-114">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> <span data-ttu-id="c6a72-115">**Observação:** saiba mais sobre a [URL raiz de serviço](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="c6a72-115">**Note:** Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="c6a72-116">Caminhos de recursos para solicitações GET</span><span class="sxs-lookup"><span data-stu-id="c6a72-116">Resource paths for GET requests</span></span>

<span data-ttu-id="c6a72-117">Use os caminhos de recursos a seguir para obter páginas, seções, grupos de seções, blocos de anotações e recursos de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="c6a72-117">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

- [<span data-ttu-id="c6a72-118">Coleção de páginas</span><span class="sxs-lookup"><span data-stu-id="c6a72-118">Page collection</span></span>](#page-collection)
- [<span data-ttu-id="c6a72-119">Entidade Page</span><span class="sxs-lookup"><span data-stu-id="c6a72-119">Page entity</span></span>](#page-entity)
- [<span data-ttu-id="c6a72-120">Visualização de página</span><span class="sxs-lookup"><span data-stu-id="c6a72-120">Page preview</span></span>](#page-preview)
- [<span data-ttu-id="c6a72-121">Conteúdo HTML da página</span><span class="sxs-lookup"><span data-stu-id="c6a72-121">Page HTML content</span></span>](#page-html-content)
- [<span data-ttu-id="c6a72-122">Coleção Section</span><span class="sxs-lookup"><span data-stu-id="c6a72-122">Section collection</span></span>](#section-collection)
- [<span data-ttu-id="c6a72-123">Entidade Section</span><span class="sxs-lookup"><span data-stu-id="c6a72-123">Section entity</span></span>](#section-entity)
- [<span data-ttu-id="c6a72-124">Coleção SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c6a72-124">SectionGroup collection</span></span>](#sectiongroup-collection)
- [<span data-ttu-id="c6a72-125">Entidade SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c6a72-125">SectionGroup entity</span></span>](#sectiongroup-entity)
- [<span data-ttu-id="c6a72-126">Coleção de blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="c6a72-126">Notebook collection</span></span>](#notebook-collection)
- [<span data-ttu-id="c6a72-127">Entidade Notebook</span><span class="sxs-lookup"><span data-stu-id="c6a72-127">Notebook entity</span></span>](#notebook-entity)
- [<span data-ttu-id="c6a72-128">Imagem ou outro recurso de arquivo</span><span class="sxs-lookup"><span data-stu-id="c6a72-128">Image or other file resource</span></span>](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a><span data-ttu-id="c6a72-129">Coleção de páginas</span><span class="sxs-lookup"><span data-stu-id="c6a72-129">Page collection</span></span>

<span data-ttu-id="c6a72-130">Obter páginas (metadados) em todos os blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="c6a72-130">Get pages (metadata) across all notebooks.</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

<span data-ttu-id="c6a72-131">Obter páginas (metadados) de uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="c6a72-131">Get pages (metadata) from a specific section.</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
<span data-ttu-id="c6a72-132">A opção de cadeia de caracteres de consulta `search` está disponível somente para blocos de anotações de consumidor.</span><span class="sxs-lookup"><span data-stu-id="c6a72-132">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="c6a72-133">A ordem de classificação padrão é `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-133">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="c6a72-134">A consulta padrão expande a seção pai e seleciona as propriedades `id`, `name` e `self` da seção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-134">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="c6a72-135">Por padrão, somente as primeiras 20 entradas são retornadas para solicitações *GET pages*.</span><span class="sxs-lookup"><span data-stu-id="c6a72-135">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="c6a72-136">Solicitações que não especificam uma opção **principal** de sequência de caracteres de consulta retornam um link `@odata.nextLink` na resposta que você pode usar para obter as próximas 20 entradas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-136">Requests that don't specify a **top** query string option return an `@odata.nextLink` link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="c6a72-137">Para a coleção de páginas em uma seção, use **pagelevel** para retornar o nível de recuo de páginas e sua ordem dentro da seção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-137">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

#### <a name="example"></a><span data-ttu-id="c6a72-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a72-138">Example</span></span>

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a><span data-ttu-id="c6a72-139">Entidade Page</span><span class="sxs-lookup"><span data-stu-id="c6a72-139">Page entity</span></span>

<span data-ttu-id="c6a72-140">Obtenha os metadados de uma página específica.</span><span class="sxs-lookup"><span data-stu-id="c6a72-140">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

<span data-ttu-id="c6a72-141">As páginas podem expandir as propriedades **parentNotebook** e **parentSection**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-141">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="c6a72-142">A consulta padrão expande a seção pai e seleciona as propriedades `id`, `name` e `self` da seção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-142">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="c6a72-143">Use **pagelevel** para retornar o nível de recuo da página e sua ordem dentro da seção pai.</span><span class="sxs-lookup"><span data-stu-id="c6a72-143">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> 

#### <a name="example"></a><span data-ttu-id="c6a72-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a72-144">Example</span></span>

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a><span data-ttu-id="c6a72-145">Visualização de página</span><span class="sxs-lookup"><span data-stu-id="c6a72-145">Page preview</span></span>

<span data-ttu-id="c6a72-146">Obtenha conteúdo de visualização de texto e imagem de uma página.</span><span class="sxs-lookup"><span data-stu-id="c6a72-146">Get text and image preview content for a page.</span></span>

`../pages/{page-id}/preview`

<br/>


<span data-ttu-id="c6a72-147">A resposta JSON contém conteúdo de visualização que você pode usar para ajudar os usuários a identificar o que está na página.</span><span class="sxs-lookup"><span data-stu-id="c6a72-147">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

<span data-ttu-id="c6a72-148">A propriedade **previewText** contém um trecho de texto proveniente da página.</span><span class="sxs-lookup"><span data-stu-id="c6a72-148">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="c6a72-149">O Microsoft Graph retorna frases completas, no máximo de 300 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c6a72-149">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="c6a72-150">Se a página tem uma imagem que pode ser usada para criar uma IU de visualização, a propriedade **href** no objeto **previewImageUrl** contém um link para um [recurso de imagem](#image-or-other-file-resource) público.</span><span class="sxs-lookup"><span data-stu-id="c6a72-150">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="c6a72-151">Você pode usar esse link em HTML.</span><span class="sxs-lookup"><span data-stu-id="c6a72-151">You can use this link in HTML.</span></span> <span data-ttu-id="c6a72-152">Caso contrário, **href** retorna nulo.</span><span class="sxs-lookup"><span data-stu-id="c6a72-152">Otherwise, **href** returns null.</span></span>

#### <a name="example"></a><span data-ttu-id="c6a72-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a72-153">Example</span></span> 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a><span data-ttu-id="c6a72-154">Conteúdo HTML da página</span><span class="sxs-lookup"><span data-stu-id="c6a72-154">Page HTML content</span></span>

<span data-ttu-id="c6a72-155">Obtenha o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="c6a72-155">Get the HTML content of a page.</span></span>

`../pages/{page-id}/content[?includeIDs]`

<span data-ttu-id="c6a72-156">(*saiba mais sobre [conteúdo HTML retornado](onenote-input-output-html.md)*)</span><span class="sxs-lookup"><span data-stu-id="c6a72-156">(*learn more about [returned HTML content](onenote-input-output-html.md)*)</span></span> 

<br/>

<span data-ttu-id="c6a72-157">Use a opção de cadeia de caracteres de consulta **includeIDs=true** para obter IDs gerados usados para [atualizar a página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="c6a72-157">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote-update-page.md).</span></span>



<a name="get-sections"></a>

### <a name="section-collection"></a><span data-ttu-id="c6a72-158">Conjunto da seção</span><span class="sxs-lookup"><span data-stu-id="c6a72-158">Section collection</span></span>

<span data-ttu-id="c6a72-159">Obtenha todas as seções de todos os blocos de anotações de propriedade de um usuário, incluindo seções em grupos de seções aninhadas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-159">Get all sections from all notebooks that are owned by the user, including sections in nested section groups.</span></span>

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c6a72-160">Obtenha todas as seções que estão diretamente em um grupo de seções específico.</span><span class="sxs-lookup"><span data-stu-id="c6a72-160">Get all sections that are directly under a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c6a72-161">Obtenha todas as seções que estão diretamente em um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="c6a72-161">Get all sections that are directly under a specific notebook.</span></span>

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c6a72-162">As seções podem expandir as propriedades **parentNotebook** e **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-162">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="c6a72-163">A ordem de classificação padrão para seções é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-163">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="c6a72-164">A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section"></a>

### <a name="section-entity"></a><span data-ttu-id="c6a72-165">Entidade Section</span><span class="sxs-lookup"><span data-stu-id="c6a72-165">Section entity</span></span>

<span data-ttu-id="c6a72-166">Obtenha uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="c6a72-166">Get a specific section.</span></span>

`../sections/{section-id}[?select,expand]` 

<br/>

<span data-ttu-id="c6a72-167">As seções podem expandir as propriedades **parentNotebook** e **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-167">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="c6a72-168">A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a><span data-ttu-id="c6a72-169">Coleção SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c6a72-169">SectionGroup collection</span></span>

<span data-ttu-id="c6a72-170">Obtenha todos os grupos de seções de todos os blocos de anotações que são de propriedade de um usuário, incluindo grupos de seções aninhadas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-170">Get all section groups from all notebooks that are owned by the user, including nested section groups.</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c6a72-171">Obtenha todos os grupos de seções que estão diretamente em um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="c6a72-171">Get all section groups that are directly under a specific notebook.</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c6a72-172">Os grupos de seções podem expandir as propriedades **sections**, **sectionGroups**, **parentNotebook** e **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-172">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="c6a72-173">A ordem de classificação padrão para grupos de seções é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-173">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="c6a72-174">A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-174">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a><span data-ttu-id="c6a72-175">Entidade SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c6a72-175">SectionGroup entity</span></span>

<span data-ttu-id="c6a72-176">Obtenha um grupo de seções específico.</span><span class="sxs-lookup"><span data-stu-id="c6a72-176">Get a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

<span data-ttu-id="c6a72-177">Os grupos de seções podem expandir as propriedades **sections**, **sectionGroups**, **parentNotebook** e **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-177">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="c6a72-178">A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-178">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a><span data-ttu-id="c6a72-179">Coleção de blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="c6a72-179">Notebook collection</span></span>

<span data-ttu-id="c6a72-180">Obtenha todos os blocos de anotações de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6a72-180">Get all the notebooks that are owned by the user.</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c6a72-181">Os blocos de anotações podem expandir as propriedades **sections** e **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-181">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="c6a72-182">A ordem de classificação padrão para blocos de anotações é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-182">The default sort order for notebooks is `name asc`.</span></span> 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a><span data-ttu-id="c6a72-183">Entidade Notebook</span><span class="sxs-lookup"><span data-stu-id="c6a72-183">Notebook entity</span></span>

<span data-ttu-id="c6a72-184">Obtenha um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="c6a72-184">Get a specific notebook.</span></span>

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

<span data-ttu-id="c6a72-185">Os blocos de anotações podem expandir as propriedades **sections** e **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-185">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a><span data-ttu-id="c6a72-186">Imagem ou outro recurso de arquivo</span><span class="sxs-lookup"><span data-stu-id="c6a72-186">Image or other file resource</span></span>

<span data-ttu-id="c6a72-187">Obtenha os dados binários de um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="c6a72-187">Get the binary data of a specific resource.</span></span> 

`../resources/{resource-id}/$value` 

<br/>

<span data-ttu-id="c6a72-188">Você pode encontrar a URI do recurso do arquivo na página de [HTML de saída](onenote-input-output-html.md).</span><span class="sxs-lookup"><span data-stu-id="c6a72-188">You can find the file's resource URI in the page's [output HTML](onenote-input-output-html.md).</span></span>

<span data-ttu-id="c6a72-189">Por exemplo, um rótulo **img** inclui os pontos de extremidade para a imagem original no atributo **data-fullres-src** e a imagem otimizada no atributo **src**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-189">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="c6a72-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a72-190">Example</span></span>

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="c6a72-191">E um rótulo **object** inclui o ponto de extremidade para o recurso do arquivo no atributo **data**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-191">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="c6a72-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a72-192">Example</span></span>

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

> <span data-ttu-id="c6a72-193">**Observação:** não há suporte para obter uma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="c6a72-193">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="c6a72-194">Quando um recurso de arquivo é obtido, não é necessário incluir um tipo de conteúdo **Accept** na solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6a72-194">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="c6a72-195">Para obter mais informações sobre solicitações GET, confira os seguintes recursos na referência do Microsoft Graph API REST:</span><span class="sxs-lookup"><span data-stu-id="c6a72-195">For more information about GET requests, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="c6a72-196">GET Pages</span><span class="sxs-lookup"><span data-stu-id="c6a72-196">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="c6a72-197">GET Sections</span><span class="sxs-lookup"><span data-stu-id="c6a72-197">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="c6a72-198">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="c6a72-198">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="c6a72-199">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="c6a72-199">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a><span data-ttu-id="c6a72-200">Exemplo de solicitações GET</span><span class="sxs-lookup"><span data-stu-id="c6a72-200">Example GET requests</span></span>

<span data-ttu-id="c6a72-201">Você pode consultar entidades do OneNote e o conteúdo de página de pesquisa para obter apenas as informações que você precisa.</span><span class="sxs-lookup"><span data-stu-id="c6a72-201">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="c6a72-202">Os exemplos a seguir mostram algumas maneiras de usar [opções de cadeia de caracteres de consulta com suporte](#supported-odata-query-string-options) em solicitações GET para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c6a72-202">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="c6a72-203">**Lembre-se:**</span><span class="sxs-lookup"><span data-stu-id="c6a72-203">**Remember:**</span></span>

- <span data-ttu-id="c6a72-204">Todas as solicitações GET começam com a [URL raiz de serviço raiz](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="c6a72-204">All GET requests start with the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span> <br/><br/><span data-ttu-id="c6a72-205">**Exemplos**: `https://www.onenote.com/api/v1.0/me/notes` e `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span><span class="sxs-lookup"><span data-stu-id="c6a72-205">**Examples**: `https://www.onenote.com/api/v1.0/me/notes` and `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span></span>

- <span data-ttu-id="c6a72-206">Os espaços na cadeia de caracteres de consulta da URL devem usar a codificação de %20.</span><span class="sxs-lookup"><span data-stu-id="c6a72-206">Spaces in the URL query string must use %20 encoding.</span></span><br/><br/><span data-ttu-id="c6a72-207">**Exemplo**: `filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="c6a72-207">**Example**: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="c6a72-208">Os nomes de propriedade e as comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-208">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="c6a72-209">É recomendável usar a função **tolower** do OData para comparações de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="c6a72-209">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="c6a72-210">**Exemplo**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="c6a72-210">**Example**: `filter=tolower(name) eq 'spring'`</span></span>
 

### <a name="search--filter"></a><span data-ttu-id="c6a72-211">search e filter</span><span class="sxs-lookup"><span data-stu-id="c6a72-211">search & filter</span></span>  

<span data-ttu-id="c6a72-212">Obtenha todas as páginas que contêm o termo *recipe* que foram criadas por um aplicativo específico (`search` está disponível somente para blocos de anotações de consumidor).</span><span class="sxs-lookup"><span data-stu-id="c6a72-212">Get all pages that contain the term *recipe* that were created by a specific app (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a><span data-ttu-id="c6a72-213">search e select</span><span class="sxs-lookup"><span data-stu-id="c6a72-213">search & select</span></span>  

<span data-ttu-id="c6a72-214">Obtenha o título, links de cliente do OneNote e o link **contentUrl** para todas as páginas que contêm o termo *golgi app* (`search` está disponível somente para blocos de anotações de consumidor).</span><span class="sxs-lookup"><span data-stu-id="c6a72-214">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app* (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a><span data-ttu-id="c6a72-215">expand</span><span class="sxs-lookup"><span data-stu-id="c6a72-215">expand</span></span> 

<span data-ttu-id="c6a72-216">Obtenha todos os blocos de anotações e expanda suas seções e grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="c6a72-216">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="c6a72-217">Obtenha um grupo de seções específico e expanda suas seções e grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="c6a72-217">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="c6a72-218">Obtenha uma página e expanda sua seção pai e o bloco de anotações pai.</span><span class="sxs-lookup"><span data-stu-id="c6a72-218">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a><span data-ttu-id="c6a72-219">expand (vários níveis)</span><span class="sxs-lookup"><span data-stu-id="c6a72-219">expand (multiple levels)</span></span>  

<span data-ttu-id="c6a72-220">Obtenha todos os blocos de anotações e expanda suas seções e grupos de seções, e expanda todas as seções em cada grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="c6a72-220">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> <span data-ttu-id="c6a72-221">**Observação:** expandir pais de entidades filho ou filhos de entidades pai cria uma referência circular e não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6a72-221">**Note:** Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
### <a name="expand--select-multiple-levels"></a><span data-ttu-id="c6a72-222">expand e select (vários níveis)</span><span class="sxs-lookup"><span data-stu-id="c6a72-222">expand & select (multiple levels)</span></span>  

<span data-ttu-id="c6a72-223">Obtenha o nome e o link **self** para um grupo de seções específico, e obtenha o nome e os links **self** para todas as suas seções.</span><span class="sxs-lookup"><span data-stu-id="c6a72-223">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

<span data-ttu-id="c6a72-224">Obtenha o nome e o link **self** para todas as seções e o nome e o tempo criados de cada bloco de anotações pai da seção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-224">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
<span data-ttu-id="c6a72-225">Obtenha o título e uma ID de todas as páginas, e o nome da seção pai e do bloco de anotações pai.</span><span class="sxs-lookup"><span data-stu-id="c6a72-225">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a><span data-ttu-id="c6a72-226">expand e levels (vários níveis)</span><span class="sxs-lookup"><span data-stu-id="c6a72-226">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="c6a72-227">Obtenha todos os blocos de anotações, seções e grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-227">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a><span data-ttu-id="c6a72-228">filter</span><span class="sxs-lookup"><span data-stu-id="c6a72-228">filter</span></span>

<span data-ttu-id="c6a72-229">Obtenha todas as seções que foram criadas em outubro de 2014.</span><span class="sxs-lookup"><span data-stu-id="c6a72-229">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

<span data-ttu-id="c6a72-230">Obtenha as páginas que foram criadas por um aplicativo específico desde 1º de janeiro de 2015.</span><span class="sxs-lookup"><span data-stu-id="c6a72-230">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a><span data-ttu-id="c6a72-231">filter e expand</span><span class="sxs-lookup"><span data-stu-id="c6a72-231">filter & expand</span></span>  

<span data-ttu-id="c6a72-232">Obtenha todas as páginas em um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="c6a72-232">Get all pages in a specific notebook.</span></span> <span data-ttu-id="c6a72-233">A API retorna 20 entradas por padrão.</span><span class="sxs-lookup"><span data-stu-id="c6a72-233">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

<span data-ttu-id="c6a72-234">Obtenha o nome e o link **pagesUrl** para todas as seções do bloco de anotações *School*.</span><span class="sxs-lookup"><span data-stu-id="c6a72-234">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="c6a72-235">Comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas, portanto, use a função **tolower** como uma prática recomendada.</span><span class="sxs-lookup"><span data-stu-id="c6a72-235">OData string comparisons are case-sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a><span data-ttu-id="c6a72-236">filter, select e orderby</span><span class="sxs-lookup"><span data-stu-id="c6a72-236">filter & select & orderby</span></span>   

<span data-ttu-id="c6a72-237">Obtenha o nome e o link **pagesUrl** para todas as seções que contêm o termo *spring* no nome da seção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-237">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name.</span></span> <span data-ttu-id="c6a72-238">Ordenar seções de pedidos por última data modificada.</span><span class="sxs-lookup"><span data-stu-id="c6a72-238">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a><span data-ttu-id="c6a72-239">orderby</span><span class="sxs-lookup"><span data-stu-id="c6a72-239">orderby</span></span>

<span data-ttu-id="c6a72-240">Obtenha as primeiras 20 páginas pela propriedade **createdByAppId** e, depois, pela hora de criação mais recente.</span><span class="sxs-lookup"><span data-stu-id="c6a72-240">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time.</span></span> <span data-ttu-id="c6a72-241">A API retorna 20 entradas por padrão.</span><span class="sxs-lookup"><span data-stu-id="c6a72-241">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a><span data-ttu-id="c6a72-242">search, filter e top</span><span class="sxs-lookup"><span data-stu-id="c6a72-242">search & filter & top</span></span> 

<span data-ttu-id="c6a72-243">Obtenha as cinco páginas mais recentemente criadas desde 1º de janeiro de 2015 com a frase *cell division*.</span><span class="sxs-lookup"><span data-stu-id="c6a72-243">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="c6a72-244">A API retorna 20 entradas por padrão com um máximo de 100.</span><span class="sxs-lookup"><span data-stu-id="c6a72-244">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="c6a72-245">A ordem de classificação padrão de páginas é `lastModifiedTime desc` (`search` está disponível somente para blocos de anotações de consumidor).</span><span class="sxs-lookup"><span data-stu-id="c6a72-245">The default sort order for pages is `lastModifiedTime desc` (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a><span data-ttu-id="c6a72-246">search, filter, top e skip</span><span class="sxs-lookup"><span data-stu-id="c6a72-246">search & filter & top & skip</span></span>  

<span data-ttu-id="c6a72-247">Obtenha as cinco próximas páginas do conjunto de resultados (`search` está disponível somente para blocos de anotações de consumidor).</span><span class="sxs-lookup"><span data-stu-id="c6a72-247">Get the next five pages in the result set (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

<span data-ttu-id="c6a72-248">E as cinco seguintes (`search` está disponível somente para blocos de anotações de consumidor).</span><span class="sxs-lookup"><span data-stu-id="c6a72-248">And the next five (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="c6a72-249">**Observação:** se **search** e **filter** são aplicadas à mesma solicitação, os resultados incluem apenas as entidades que correspondem aos dois critérios.</span><span class="sxs-lookup"><span data-stu-id="c6a72-249">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
### <a name="select"></a><span data-ttu-id="c6a72-250">select</span><span class="sxs-lookup"><span data-stu-id="c6a72-250">select</span></span>

<span data-ttu-id="c6a72-251">Obtenha nome, hora de criação e link **self** de todas as seções nos blocos de anotações do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6a72-251">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

<span data-ttu-id="c6a72-252">Obtenha título, hora de criação e links do cliente do OneNote para uma página específica.</span><span class="sxs-lookup"><span data-stu-id="c6a72-252">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a><span data-ttu-id="c6a72-253">select, expand e filter (vários níveis)</span><span class="sxs-lookup"><span data-stu-id="c6a72-253">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="c6a72-254">Obtenha nome e link **pagesUrl** para todas as seções do bloco de anotações do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6a72-254">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a><span data-ttu-id="c6a72-255">top, select e orderby</span><span class="sxs-lookup"><span data-stu-id="c6a72-255">top & select & orderby</span></span> 

<span data-ttu-id="c6a72-256">Obtenha o título e o link **self** das 50 primeiras páginas, classificadas em ordem alfabética por título.</span><span class="sxs-lookup"><span data-stu-id="c6a72-256">Get the title and **self** link for the first 50 pages, ordered alphabetically by title.</span></span> <span data-ttu-id="c6a72-257">A API retorna 20 entradas por padrão com um máximo de 100.</span><span class="sxs-lookup"><span data-stu-id="c6a72-257">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="c6a72-258">A ordem de classificação padrão é `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-258">The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a><span data-ttu-id="c6a72-259">skip, top, select e orderby</span><span class="sxs-lookup"><span data-stu-id="c6a72-259">skip & top & select & orderby</span></span>  

<span data-ttu-id="c6a72-260">Obtenha páginas de 51 a 100.</span><span class="sxs-lookup"><span data-stu-id="c6a72-260">Get pages 51 to 100.</span></span> <span data-ttu-id="c6a72-261">A API retorna 20 entradas por padrão com um máximo de 100.</span><span class="sxs-lookup"><span data-stu-id="c6a72-261">The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="c6a72-262">**Observação:** As solicitações GET para páginas que recuperam o número padrão de entradas (ou seja, elas não especificam uma expressão **top**) retornam um link **\@odata.nextLink** na resposta que você pode usar para obter as próximas 20 entradas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-262">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **\@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a><span data-ttu-id="c6a72-263">Opções de cadeia de caracteres de consulta OData com suporte.</span><span class="sxs-lookup"><span data-stu-id="c6a72-263">Supported OData query string options</span></span>

<span data-ttu-id="c6a72-264">Quando enviar solicitações GET para Microsoft Graph, você pode usar as opções de cadeia de caracteres de consulta de OData para personalizar sua consulta e obter apenas as informações que você precisa.</span><span class="sxs-lookup"><span data-stu-id="c6a72-264">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="c6a72-265">Também podem melhorar o desempenho, reduzindo o número de chamadas para o serviço e o tamanho da carga de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6a72-265">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="c6a72-266">**Observação:** para facilitar a leitura, os exemplos neste artigo não usam a codificação de %20 necessária para espaços na cadeia de caracteres de consulta da URL: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="c6a72-266">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="c6a72-267">Opção de consulta</span><span class="sxs-lookup"><span data-stu-id="c6a72-267">Query option</span></span> | <span data-ttu-id="c6a72-268">Exemplo e descrição</span><span class="sxs-lookup"><span data-stu-id="c6a72-268">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="c6a72-269">count</span><span class="sxs-lookup"><span data-stu-id="c6a72-269">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="c6a72-270">A contagem de entidades da coleção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-270">The count of entities in the collection.</span></span> <span data-ttu-id="c6a72-271">O valor é retornado na propriedade **odata.coun\@** t na resposta.</span><span class="sxs-lookup"><span data-stu-id="c6a72-271">The value is returned in the **\@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="c6a72-272">expand</span><span class="sxs-lookup"><span data-stu-id="c6a72-272">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="c6a72-273">Propriedades de navegação para retornar embutidas na resposta.</span><span class="sxs-lookup"><span data-stu-id="c6a72-273">The navigation properties to return inline in the response.</span></span> <span data-ttu-id="c6a72-274">As propriedades a seguir têm suporte para expressões **expand**:</span><span class="sxs-lookup"><span data-stu-id="c6a72-274">The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="c6a72-275">– Páginas: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="c6a72-275">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="c6a72-276">– Seções: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="c6a72-276">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="c6a72-277">– Grupos de seções: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="c6a72-277">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="c6a72-278">– Blocos de anotações: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="c6a72-278">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="c6a72-279">Por padrão, as solicitações GET de páginas expandem **parentSection** e selecionam as propriedades **id**, **name** e **self**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-279">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties.</span></span> <span data-ttu-id="c6a72-280">Solicitações GET padrão de seções e grupos de seções expandem **parentNotebook** e **parentSectionGroup** e selecionam as propriedades pai **id**, **name** e **self**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-280">Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties.</span></span> </p><p><span data-ttu-id="c6a72-281">Pode ser usado para uma única entidade ou uma coleção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-281">Can be used for a single entity or a collection.</span></span><br /><span data-ttu-id="c6a72-282">Separar com vírgulas várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="c6a72-282">Separate multiple properties with commas.</span></span><br /><span data-ttu-id="c6a72-283">Os nomes de propriedades diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-283">Property names are case-sensitive.</span></span></p> |   
| <span data-ttu-id="c6a72-284">filter</span><span class="sxs-lookup"><span data-stu-id="c6a72-284">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="c6a72-285">Uma expressão booliana para se deseja incluir uma entrada no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c6a72-285">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="c6a72-286">Compatível com os seguintes operadores e funções OData:</span><span class="sxs-lookup"><span data-stu-id="c6a72-286">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="c6a72-287">– Operadores de comparação: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span><span class="sxs-lookup"><span data-stu-id="c6a72-287">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="c6a72-288">– Operadores lógicos: **and**, **or**, **not**</span><span class="sxs-lookup"><span data-stu-id="c6a72-288">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="c6a72-289">– Funções de cadeia de caracteres: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span><span class="sxs-lookup"><span data-stu-id="c6a72-289">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="c6a72-290">Os nomes de [propriedade](#onenote-entity-properties) e as comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-290">[Property](#onenote-entity-properties) names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="c6a72-291">É recomendável usar a função **tolower** do OData para comparações de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="c6a72-291">We recommend using the OData **tolower** function for string comparisons.</span></span><br /><br /><span data-ttu-id="c6a72-292">**Exemplo**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="c6a72-292">**Example**: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="c6a72-293">orderby</span><span class="sxs-lookup"><span data-stu-id="c6a72-293">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="c6a72-294">As [propriedades](#onenote-entity-properties) para classificar por, com uma ordem de classificação opcional **asc** (padrão) ou **desc**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-294">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order.</span></span> <span data-ttu-id="c6a72-295">Você pode classificar por qualquer propriedade da entidade na coleção solicitada.</span><span class="sxs-lookup"><span data-stu-id="c6a72-295">You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="c6a72-296">A ordem de classificação padrão para blocos de anotações, grupos de seções e seções é `name asc`, e para páginas é `lastModifiedTime desc` (última página modificada primeiro).</span><span class="sxs-lookup"><span data-stu-id="c6a72-296">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="c6a72-297">Separe as várias propriedades com vírgulas e liste-as na ordem de aplicação desejada.</span><span class="sxs-lookup"><span data-stu-id="c6a72-297">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="c6a72-298">Os nomes de propriedades diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-298">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="c6a72-299">search</span><span class="sxs-lookup"><span data-stu-id="c6a72-299">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="c6a72-300">Disponível somente para blocos de anotações de consumidor.</span><span class="sxs-lookup"><span data-stu-id="c6a72-300">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="c6a72-301">O termo ou frase para pesquisar no título da página, corpo da página, texto alt da imagem e texto da imagem OCR.</span><span class="sxs-lookup"><span data-stu-id="c6a72-301">The term or phrase to search for in the page title, page body, image alt text, and image OCR text.</span></span> <span data-ttu-id="c6a72-302">Por padrão, consultas de pesquisa retornam resultados classificados por relevância.</span><span class="sxs-lookup"><span data-stu-id="c6a72-302">By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="c6a72-303">O OneNote usa a pesquisa de texto completo do Bing para dar suporte a pesquisa de frase, lematização, tolerância de ortografia, relevância e classificação, quebra de palavras, vários idiomas e outros recursos de pesquisa de texto completo.</span><span class="sxs-lookup"><span data-stu-id="c6a72-303">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="c6a72-304">As cadeias de caracteres de pesquisa diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-304">Search strings are case-insensitive.</span></span></p><p><span data-ttu-id="c6a72-305">Aplica-se somente a páginas em blocos de anotações de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6a72-305">Applies only to pages in notebooks owned by the user.</span></span> <span data-ttu-id="c6a72-306">O conteúdo indexado é privado e só pode ser acessado pelo proprietário.</span><span class="sxs-lookup"><span data-stu-id="c6a72-306">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="c6a72-307">As páginas protegidas por senha não são indexadas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-307">Password-protected pages are not indexed.</span></span> <span data-ttu-id="c6a72-308">Aplicável somente ao ponto de extremidade `pages`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-308">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="c6a72-309">select</span><span class="sxs-lookup"><span data-stu-id="c6a72-309">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="c6a72-310">As [propriedades](#onenote-entity-properties) a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-310">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="c6a72-311">Pode ser usado para uma única entidade ou para uma coleção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-311">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="c6a72-312">Separar com vírgulas várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="c6a72-312">Separate multiple properties with commas.</span></span> <span data-ttu-id="c6a72-313">Os nomes de propriedades diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-313">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="c6a72-314">skip</span><span class="sxs-lookup"><span data-stu-id="c6a72-314">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="c6a72-315">O número de entradas para ignorar no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c6a72-315">The number of entries to skip in the result set.</span></span> <span data-ttu-id="c6a72-316">Costumam ser usadas para resultados de paginação.</span><span class="sxs-lookup"><span data-stu-id="c6a72-316">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="c6a72-317">top</span><span class="sxs-lookup"><span data-stu-id="c6a72-317">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="c6a72-318">O número de entradas para retornar do conjunto de resultados, até um máximo de 100.</span><span class="sxs-lookup"><span data-stu-id="c6a72-318">The number of entries to return in the result set, up to a maximum of 100.</span></span> <span data-ttu-id="c6a72-319">O valor padrão é 20.</span><span class="sxs-lookup"><span data-stu-id="c6a72-319">The default value is 20.</span></span></p> |  

<span data-ttu-id="c6a72-320">O Microsoft Graph também fornece a opção de cadeia de caracteres de consulta `pagelevel` que você pode usar para obter o nível e ordem das páginas dentro da seção pai.</span><span class="sxs-lookup"><span data-stu-id="c6a72-320">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="c6a72-321">Aplicam-se apenas às consultas de páginas em uma seção específica ou consultas para uma página específica.</span><span class="sxs-lookup"><span data-stu-id="c6a72-321">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

#### <a name="examples"></a><span data-ttu-id="c6a72-322">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c6a72-322">Examples</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="c6a72-323">Funções e operadores de OData compatíveis</span><span class="sxs-lookup"><span data-stu-id="c6a72-323">Supported OData operators and functions</span></span>

<span data-ttu-id="c6a72-324">Microsoft Graph é compatível com os seguintes operadores e funções do OData nas expressões de **filter**.</span><span class="sxs-lookup"><span data-stu-id="c6a72-324">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="c6a72-325">Ao usar expressões de OData, lembre-se:</span><span class="sxs-lookup"><span data-stu-id="c6a72-325">When using OData expressions, remember:</span></span>

- <span data-ttu-id="c6a72-326">Os espaços na cadeia de caracteres de consulta da URL devem ser substituídos pela codificação `%20`.</span><span class="sxs-lookup"><span data-stu-id="c6a72-326">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span><br/><br/><span data-ttu-id="c6a72-327">**Exemplo:** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="c6a72-327">**Example:** `filter=isDefault%20eq%20true`</span></span>

- <span data-ttu-id="c6a72-328">Os nomes de propriedade e as comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-328">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="c6a72-329">É recomendável usar a função **tolower** do OData para comparações de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="c6a72-329">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="c6a72-330">**Exemplo:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="c6a72-330">**Example:** `filter=tolower(name) eq 'spring'`</span></span>


| <span data-ttu-id="c6a72-331">Operador de comparação</span><span class="sxs-lookup"><span data-stu-id="c6a72-331">Comparison operator</span></span> | <span data-ttu-id="c6a72-332">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a72-332">Example</span></span> |  
|------|------|  
| <span data-ttu-id="c6a72-333">eq</span><span class="sxs-lookup"><span data-stu-id="c6a72-333">eq</span></span><br /><span data-ttu-id="c6a72-334">(igual a)</span><span class="sxs-lookup"><span data-stu-id="c6a72-334">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="c6a72-335">ne</span><span class="sxs-lookup"><span data-stu-id="c6a72-335">ne</span></span><br /><span data-ttu-id="c6a72-336">(é diferente de)</span><span class="sxs-lookup"><span data-stu-id="c6a72-336">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="c6a72-337">gt</span><span class="sxs-lookup"><span data-stu-id="c6a72-337">gt</span></span><br /><span data-ttu-id="c6a72-338">(maior que)</span><span class="sxs-lookup"><span data-stu-id="c6a72-338">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="c6a72-339">ge</span><span class="sxs-lookup"><span data-stu-id="c6a72-339">ge</span></span><br /><span data-ttu-id="c6a72-340">(maior que ou igual a)</span><span class="sxs-lookup"><span data-stu-id="c6a72-340">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="c6a72-341">lt</span><span class="sxs-lookup"><span data-stu-id="c6a72-341">lt</span></span><br /><span data-ttu-id="c6a72-342">(menor que)</span><span class="sxs-lookup"><span data-stu-id="c6a72-342">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="c6a72-343">le</span><span class="sxs-lookup"><span data-stu-id="c6a72-343">le</span></span><br /><span data-ttu-id="c6a72-344">(menor que ou igual a)</span><span class="sxs-lookup"><span data-stu-id="c6a72-344">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  

<br/>

| <span data-ttu-id="c6a72-345">Operador lógico</span><span class="sxs-lookup"><span data-stu-id="c6a72-345">Logical operator</span></span> | <span data-ttu-id="c6a72-346">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a72-346">Example</span></span> |  
|------|------|  
| <span data-ttu-id="c6a72-347">e</span><span class="sxs-lookup"><span data-stu-id="c6a72-347">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="c6a72-348">or</span><span class="sxs-lookup"><span data-stu-id="c6a72-348">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="c6a72-349">not</span><span class="sxs-lookup"><span data-stu-id="c6a72-349">not</span></span> | `not contains(tolower(title),'school')` |  

<br/>
  
| <span data-ttu-id="c6a72-350">Função da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6a72-350">String function</span></span> | <span data-ttu-id="c6a72-351">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a72-351">Example</span></span> |  
|------|------|   
| <span data-ttu-id="c6a72-352">contains</span><span class="sxs-lookup"><span data-stu-id="c6a72-352">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="c6a72-353">endswith</span><span class="sxs-lookup"><span data-stu-id="c6a72-353">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="c6a72-354">startswith</span><span class="sxs-lookup"><span data-stu-id="c6a72-354">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="c6a72-355">length</span><span class="sxs-lookup"><span data-stu-id="c6a72-355">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="c6a72-356">indexof</span><span class="sxs-lookup"><span data-stu-id="c6a72-356">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="c6a72-357">substring</span><span class="sxs-lookup"><span data-stu-id="c6a72-357">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="c6a72-358">tolower</span><span class="sxs-lookup"><span data-stu-id="c6a72-358">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="c6a72-359">toupper</span><span class="sxs-lookup"><span data-stu-id="c6a72-359">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="c6a72-360">trim</span><span class="sxs-lookup"><span data-stu-id="c6a72-360">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="c6a72-361">concat</span><span class="sxs-lookup"><span data-stu-id="c6a72-361">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a><span data-ttu-id="c6a72-362">Propriedades de entidade do OneNote</span><span class="sxs-lookup"><span data-stu-id="c6a72-362">OneNote entity properties</span></span>

<span data-ttu-id="c6a72-363">As expressões de consulta **filter**, **select**, **expand** e **orderby** podem incluir propriedades de entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c6a72-363">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

#### <a name="example"></a><span data-ttu-id="c6a72-364">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6a72-364">Example</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="c6a72-365">Os nomes de propriedades diferenciam maiúsculas de minúsculas em expressões de consulta.</span><span class="sxs-lookup"><span data-stu-id="c6a72-365">Property names are case-sensitive in query expressions.</span></span>

<span data-ttu-id="c6a72-366">Para obter a lista de propriedades e seus tipos, confira os seguintes recursos na referência do Microsoft Graph API REST:</span><span class="sxs-lookup"><span data-stu-id="c6a72-366">For the list of properties and property types, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="c6a72-367">GET Pages</span><span class="sxs-lookup"><span data-stu-id="c6a72-367">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="c6a72-368">GET Sections</span><span class="sxs-lookup"><span data-stu-id="c6a72-368">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="c6a72-369">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="c6a72-369">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="c6a72-370">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="c6a72-370">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 



<span data-ttu-id="c6a72-371">A opção de cadeia de caracteres de consulta **expand** pode ser usada com as seguintes propriedades de navegação:</span><span class="sxs-lookup"><span data-stu-id="c6a72-371">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="c6a72-372">Páginas: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="c6a72-372">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="c6a72-373">Seções: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="c6a72-373">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="c6a72-374">Grupos de seções: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="c6a72-374">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="c6a72-375">Blocos de anotações: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="c6a72-375">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="c6a72-376">Informações de solicitação e resposta para solicitações de *GET*</span><span class="sxs-lookup"><span data-stu-id="c6a72-376">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="c6a72-377">Dados da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6a72-377">Request data</span></span> | <span data-ttu-id="c6a72-378">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6a72-378">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c6a72-379">Protocolo</span><span class="sxs-lookup"><span data-stu-id="c6a72-379">Protocol</span></span> | <span data-ttu-id="c6a72-380">Todas as solicitações usam o protocolo HTTPS de SSL/TLS.</span><span class="sxs-lookup"><span data-stu-id="c6a72-380">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="c6a72-381">Cabeçalho de autorização</span><span class="sxs-lookup"><span data-stu-id="c6a72-381">Authorization header</span></span> | <p><span data-ttu-id="c6a72-382">`Bearer {token}`, onde `{token}` é um token de acesso do OAuth 2.0 válido para o aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="c6a72-382">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="c6a72-383">Se ele estiver ausente ou for inválido, a solicitação falhará com um código de status 401.</span><span class="sxs-lookup"><span data-stu-id="c6a72-383">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="c6a72-384">Confira [Autenticação e permissões](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6a72-384">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="c6a72-385">Cabeçalho Accept</span><span class="sxs-lookup"><span data-stu-id="c6a72-385">Accept header</span></span> | <p> <span data-ttu-id="c6a72-386">`application/json` para entidades e conjuntos de entidades do OneNote</span><span class="sxs-lookup"><span data-stu-id="c6a72-386">`application/json` for OneNote entities and entity sets</span></span></p><p> <span data-ttu-id="c6a72-387">`text/html` para conteúdo de página</span><span class="sxs-lookup"><span data-stu-id="c6a72-387">`text/html` for page content</span></span></p> | 

<br/>

| <span data-ttu-id="c6a72-388">Dados de resposta</span><span class="sxs-lookup"><span data-stu-id="c6a72-388">Response data</span></span> | <span data-ttu-id="c6a72-389">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6a72-389">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c6a72-390">Código de êxito</span><span class="sxs-lookup"><span data-stu-id="c6a72-390">Success code</span></span> | <span data-ttu-id="c6a72-391">Um código de status de HTTP 200.</span><span class="sxs-lookup"><span data-stu-id="c6a72-391">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="c6a72-392">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="c6a72-392">Response body</span></span> | <span data-ttu-id="c6a72-393">Uma representação de OData da entidade ou conjunto de entidades no formato JSON, da página HTML ou dados binários do recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="c6a72-393">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="c6a72-394">Erros</span><span class="sxs-lookup"><span data-stu-id="c6a72-394">Errors</span></span> | <span data-ttu-id="c6a72-395">Se a solicitação falhar, a API retornará erros no objeto [errors](onenote-error-codes.md) no **\@@api.diagnostics** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6a72-395">If the request fails, the API returns [errors](onenote-error-codes.md) in the **\@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="c6a72-396">Cabeçalho X-CorrelationId</span><span class="sxs-lookup"><span data-stu-id="c6a72-396">X-CorrelationId header</span></span> | <span data-ttu-id="c6a72-397">Um GUID que identifica de forma exclusiva a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6a72-397">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="c6a72-398">Você pode usar esse valor juntamente com o valor do cabeçalho Data ao trabalhar com o suporte da Microsoft para solucionar problemas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-398">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="c6a72-399">Criar a URL raiz do serviço de anotações do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c6a72-399">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="c6a72-400">A URL raiz do serviço de anotações do Microsoft Graph usa o formato a seguir para todas as chamadas para o Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="c6a72-400">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="c6a72-401">O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="c6a72-401">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="c6a72-402">Use `v1.0` para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="c6a72-402">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="c6a72-403">Use `beta` para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="c6a72-403">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="c6a72-404">Os recursos e a funcionalidade na versão beta podem mudar, por isso, você não deve usá-la no código de produção.</span><span class="sxs-lookup"><span data-stu-id="c6a72-404">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="c6a72-405">Use `me` para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="c6a72-405">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="c6a72-406">Use `users/{id}` para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="c6a72-406">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="c6a72-407">Use o [Microsoft Graph](https://graph.microsoft.com/v1.0/users) para obter as IDs de usuário.</span><span class="sxs-lookup"><span data-stu-id="c6a72-407">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a><span data-ttu-id="c6a72-408">Permissões para solicitações GET</span><span class="sxs-lookup"><span data-stu-id="c6a72-408">Permissions for GET requests</span></span>

<span data-ttu-id="c6a72-409">Para obter conteúdo ou estrutura do OneNote, você vai precisar solicitar as permissões adequadas.</span><span class="sxs-lookup"><span data-stu-id="c6a72-409">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="c6a72-410">Os seguintes escopos permitem solicitações GET para Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c6a72-410">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="c6a72-411">Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="c6a72-411">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="c6a72-412">Escolha entre:</span><span class="sxs-lookup"><span data-stu-id="c6a72-412">Choose from:</span></span>

- <span data-ttu-id="c6a72-413">Notes.read</span><span class="sxs-lookup"><span data-stu-id="c6a72-413">Notes.read</span></span>
- <span data-ttu-id="c6a72-414">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6a72-414">Notes.ReadWrite</span></span>
- <span data-ttu-id="c6a72-415">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6a72-415">Notes.ReadWrite.All</span></span>

<span data-ttu-id="c6a72-416">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Referência de permissões do Microsoft Graph](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6a72-416">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="c6a72-417">Confira também</span><span class="sxs-lookup"><span data-stu-id="c6a72-417">See also</span></span>

- [<span data-ttu-id="c6a72-418">HTML de entrada e saída para páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="c6a72-418">Input and output HTML for OneNote pages</span></span>](onenote-input-output-html.md)
- [<span data-ttu-id="c6a72-419">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="c6a72-419">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="c6a72-420">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="c6a72-420">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="c6a72-421">Perguntas de desenvolvimento do OneNote no Microsoft Q&A</span><span class="sxs-lookup"><span data-stu-id="c6a72-421">OneNote development questions on Microsoft Q&A</span></span>](/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="c6a72-422">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="c6a72-422">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)