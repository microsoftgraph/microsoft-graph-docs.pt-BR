# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="5988f-101">Obter a estrutura e o conteúdo do OneNote com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5988f-101">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="5988f-102">*__Aplica-se a:__ Bloco de anotações dos consumidores no OneDrive | Bloco de anotações empresariais no Office 365*</span><span class="sxs-lookup"><span data-stu-id="5988f-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="5988f-103">Para obter a estrutura e o conteúdo do OneNote, envie uma solicitação GET ao ponto de extremidade de destino.</span><span class="sxs-lookup"><span data-stu-id="5988f-103">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="5988f-104">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="5988f-104">For example:</span></span>

`GET ../onenote/pages/{id}`</p>

<span data-ttu-id="5988f-105">Se a solicitação for bem-sucedida, o Microsoft Graph retornará um código de status de HTTP 200 e as entidades ou o conteúdo que você solicitou.</span><span class="sxs-lookup"><span data-stu-id="5988f-105">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="5988f-106">As entidades do OneNote são retornadas como objetos JSON que estão em conformidade com a especificação OData versão 4.0.</span><span class="sxs-lookup"><span data-stu-id="5988f-106">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="5988f-107">Usando as opções de cadeia de caracteres de consulta, você pode filtrar as consultas e melhorar o desempenho.</span><span class="sxs-lookup"><span data-stu-id="5988f-107">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="5988f-108">Construir a URI de solicitação</span><span class="sxs-lookup"><span data-stu-id="5988f-108">Construct the request</span></span>

<span data-ttu-id="5988f-109">Para construir a URI de solicitação, comece com a URL raiz do serviço:</span><span class="sxs-lookup"><span data-stu-id="5988f-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="5988f-110">Em seguida, acrescente o ponto de extremidade do recurso que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="5988f-110">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="5988f-111">(Os [caminhos recurso](#resource-paths-for-get-requests) são mostrados na próxima seção).</span><span class="sxs-lookup"><span data-stu-id="5988f-111">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>


<span data-ttu-id="5988f-112">Sua URI de solicitação completa parecerá com um dos seguintes exemplos:</span><span class="sxs-lookup"><span data-stu-id="5988f-112">Your full request URI will look like one of these examples:</span></span>
- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`</p>

> <span data-ttu-id="5988f-113">**Observação:** saiba mais sobre a [URL raiz de serviço](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="5988f-113">**Note:** Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="resource-paths"></a>
## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="5988f-114">Caminhos de recursos para solicitações GET</span><span class="sxs-lookup"><span data-stu-id="5988f-114">Resource paths for GET requests</span></span>

<span data-ttu-id="5988f-115">Use os caminhos de recursos a seguir para obter páginas, seções, grupos de seções, blocos de anotações e recursos de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="5988f-115">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

<span data-ttu-id="5988f-116">[Coleção de páginas](#page-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Entidade Page](#page-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Visualização de página](#page-preview)&nbsp;&nbsp;|&nbsp;&nbsp;[Conteúdo HTML de página](#page-html-content)&nbsp;&nbsp;|&nbsp;&nbsp; [Coleção de seções](#section-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Entidade Section](#section-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Coleção SectionGroup](#sectiongroup-collection)&nbsp;&nbsp;|&nbsp;&nbsp; [Entidade SectionGroup](#sectiongroup-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Coleção de bloco de anotações](#notebook-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Entidade Notebook](#notebook-entity)&nbsp;&nbsp;|&nbsp;&nbsp; [Imagem ou outro recurso de arquivo](#image-or-other-file-resource)</span><span class="sxs-lookup"><span data-stu-id="5988f-116">[Page collection](#page-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Page entity](#page-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Page preview](#page-preview)&nbsp;&nbsp;|&nbsp;&nbsp;[Page HTML content](#page-html-content)&nbsp;&nbsp;|&nbsp;&nbsp; [Section collection](#section-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Section entity](#section-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[SectionGroup collection](#sectiongroup-collection)&nbsp;&nbsp;|&nbsp;&nbsp; [SectionGroup entity](#sectiongroup-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook collection](#notebook-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook entity](#notebook-entity)&nbsp;&nbsp;|&nbsp;&nbsp; [Image or other file resource](#image-or-other-file-resource)</span></span>

<a name="get-pages"></a>
### <a name="page-collection"></a><span data-ttu-id="5988f-117">Coleção de páginas</span><span class="sxs-lookup"><span data-stu-id="5988f-117">Page collection</span></span>

<span data-ttu-id="5988f-118">Obter páginas (metadados) em todos os blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="5988f-118">Get pages (metadata) across all notebooks</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<span data-ttu-id="5988f-119">Obter páginas (metadados) de uma seção específica</span><span class="sxs-lookup"><span data-stu-id="5988f-119">Get pages (metadata) from a specific section</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

 
<span data-ttu-id="5988f-120">A opção de cadeia de caracteres de consulta `search` está disponível somente para blocos de anotações de consumidor.</span><span class="sxs-lookup"><span data-stu-id="5988f-120">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="5988f-121">A ordem de classificação padrão é `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="5988f-121">The default sort order is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="5988f-122">A consulta padrão expande a seção pai e seleciona as propriedades `id`, `name` e `self` da seção.</span><span class="sxs-lookup"><span data-stu-id="5988f-122">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="5988f-123">Por padrão, somente as primeiras 20 entradas são retornadas para solicitações *GET pages*.</span><span class="sxs-lookup"><span data-stu-id="5988f-123">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="5988f-124">As solicitações que não especificam uma opção de cadeia de caracteres de consulta **top** retornam um link **@odata.nextLink** na resposta que você pode usar para acessar as próximas 20 entradas.</span><span class="sxs-lookup"><span data-stu-id="5988f-124">Requests that don't specify a **top** query string option return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="5988f-125">Para a coleção de páginas em uma seção, use **pagelevel** para retornar o nível de recuo de páginas e sua ordem dentro da seção.</span><span class="sxs-lookup"><span data-stu-id="5988f-125">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

<span data-ttu-id="5988f-126">**Exemplo:**  `GET ../sections/{section-id}/pages?pagelevel=true`.</span><span class="sxs-lookup"><span data-stu-id="5988f-126">Example</span></span>

- - -

<a name="get-page"></a> 
### <a name="page-entity"></a><span data-ttu-id="5988f-127">Entidade Page</span><span class="sxs-lookup"><span data-stu-id="5988f-127">Page entity</span></span>

<span data-ttu-id="5988f-128">Obtenha os metadados de uma página específica.</span><span class="sxs-lookup"><span data-stu-id="5988f-128">Get the metadata for a folder.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 


<span data-ttu-id="5988f-129">As páginas podem expandir as propriedades **parentNotebook** e **parentSection**.</span><span class="sxs-lookup"><span data-stu-id="5988f-129">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="5988f-130">A consulta padrão expande a seção pai e seleciona as propriedades `id`, `name` e `self` da seção.</span><span class="sxs-lookup"><span data-stu-id="5988f-130">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="5988f-131">Use **pagelevel** para retornar o nível de recuo da página e sua ordem dentro da seção pai.</span><span class="sxs-lookup"><span data-stu-id="5988f-131">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> <span data-ttu-id="5988f-132">Exemplo: `GET ../pages/{page-id}?pagelevel=true`.</span><span class="sxs-lookup"><span data-stu-id="5988f-132">Example: `GET ../pages/{page-id}?pagelevel=true`</span></span>

- - -

<a name="get-page-preview"></a> 
### <a name="page-preview"></a><span data-ttu-id="5988f-133">Visualização de página</span><span class="sxs-lookup"><span data-stu-id="5988f-133">Page break preview.</span></span>

<span data-ttu-id="5988f-134">Obter conteúdo de visualização de texto e imagem de uma página</span><span class="sxs-lookup"><span data-stu-id="5988f-134">Get text and image preview content for a page</span></span>

`../pages/{page-id}/preview`


<span data-ttu-id="5988f-135">A resposta JSON contém conteúdo de visualização que você pode usar para ajudar os usuários a identificar o que está na página.</span><span class="sxs-lookup"><span data-stu-id="5988f-135">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

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

<span data-ttu-id="5988f-136">A propriedade **previewText** contém um trecho de texto proveniente da página.</span><span class="sxs-lookup"><span data-stu-id="5988f-136">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="5988f-137">O Microsoft Graph retorna frases completas, no máximo de 300 caracteres.</span><span class="sxs-lookup"><span data-stu-id="5988f-137">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="5988f-138">Se a página tem uma imagem que pode ser usada para criar uma IU de visualização, a propriedade **href** no objeto **previewImageUrl** contém um link para um [recurso de imagem](#image-or-other-file-resource) público e pré-autenticado.</span><span class="sxs-lookup"><span data-stu-id="5988f-138">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="5988f-139">Você pode usar esse link em HTML,</span><span class="sxs-lookup"><span data-stu-id="5988f-139">You can use this link in HTML,</span></span>

<span data-ttu-id="5988f-140">**Exemplo:** `<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`.</span><span class="sxs-lookup"><span data-stu-id="5988f-140">Example</span></span> <span data-ttu-id="5988f-141">Caso contrário, **href** retorna nulo.</span><span class="sxs-lookup"><span data-stu-id="5988f-141">Otherwise, **href** returns null.</span></span>

- - -

<a name="get-page-content"></a> 
### <a name="page-html-content"></a><span data-ttu-id="5988f-142">Conteúdo HTML da página</span><span class="sxs-lookup"><span data-stu-id="5988f-142">Page HTML content</span></span>

<span data-ttu-id="5988f-143">Obter o conteúdo HTML da página `../pages/{page-id}/content[?includeIDs,preAuthenticated]`</span><span class="sxs-lookup"><span data-stu-id="5988f-143">Get the HTML content of a page `../pages/{page-id}/content[?includeIDs,preAuthenticated]`</span></span>

<span data-ttu-id="5988f-144">(*saiba mais sobre [conteúdo HTML retornado](onenote_input_output_html.md)*)</span><span class="sxs-lookup"><span data-stu-id="5988f-144">(*learn more about [returned HTML content](onenote_input_output_html.md)*)</span></span> 

 
<span data-ttu-id="5988f-145">Use a opção de cadeia de caracteres de consulta **includeIDs=true** para obter IDs gerados usados para [atualizar a página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="5988f-145">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote_update_page.md).</span></span>

<span data-ttu-id="5988f-146">Use a opção de cadeia de caracteres de consulta **preAuthenticated=true** para acessar as URLs públicas para os [recursos de imagem](#image-or-other-file-resource) que estejam na página.</span><span class="sxs-lookup"><span data-stu-id="5988f-146">Use the **preAuthenticated=true** query string option to get public URLs to the [image resources](#image-or-other-file-resource) that are on the page.</span></span> <span data-ttu-id="5988f-147">As URLs públicas são válidas por uma hora.</span><span class="sxs-lookup"><span data-stu-id="5988f-147">The public URLs that are returned are valid for one hour.</span></span> 

- - -

<a name="get-sections"></a>
### <a name="section-collection"></a><span data-ttu-id="5988f-148">Coleção Section</span><span class="sxs-lookup"><span data-stu-id="5988f-148">Section collection</span></span>

<span data-ttu-id="5988f-149">Obtenha todas as seções de todos os blocos de anotações de propriedade de um usuário, incluindo seções em grupos de seções aninhadas `../sections[?filter,orderby,select,top,skip,expand,count]`</span><span class="sxs-lookup"><span data-stu-id="5988f-149">Get all sections from all notebooks that are owned by the user, including sections in nested section groups `../sections[?filter,orderby,select,top,skip,expand,count]`</span></span> 

<span data-ttu-id="5988f-150">Obtenha todas as seções que estão diretamente em um grupo de seções específico</span><span class="sxs-lookup"><span data-stu-id="5988f-150">Get all sections that are directly under a specific section group</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="5988f-151">Obtenha todas as seções que estão diretamente em um bloco de anotações específico `../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]`</span><span class="sxs-lookup"><span data-stu-id="5988f-151">Get all sections that are directly under a specific notebook `../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]`</span></span> 

 
<span data-ttu-id="5988f-152">As seções podem expandir as propriedades**parentNotebook** e **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="5988f-152">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="5988f-153">A ordem de classificação padrão para seções é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="5988f-153">The default sort order is `name asc`.</span></span>

<span data-ttu-id="5988f-154">A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.</span><span class="sxs-lookup"><span data-stu-id="5988f-154">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section"></a>
### <a name="section-entity"></a><span data-ttu-id="5988f-155">Entidade Section</span><span class="sxs-lookup"><span data-stu-id="5988f-155">Section entity</span></span>

<span data-ttu-id="5988f-156">Obter uma seção específica</span><span class="sxs-lookup"><span data-stu-id="5988f-156">Get a specific entity</span></span>

`../sections/{section-id}[?select,expand]` 

 
<span data-ttu-id="5988f-157">As seções podem expandir as propriedades**parentNotebook** e **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="5988f-157">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="5988f-158">A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.</span><span class="sxs-lookup"><span data-stu-id="5988f-158">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section-groups"></a>
### <a name="sectiongroup-collection"></a><span data-ttu-id="5988f-159">Coleção SectionGroup</span><span class="sxs-lookup"><span data-stu-id="5988f-159">SectionGroup collection</span></span>

<span data-ttu-id="5988f-160">Obtenha todos os grupos de seções de todos os blocos de anotações que são de propriedade de um usuário, incluindo grupos de seções aninhadas</span><span class="sxs-lookup"><span data-stu-id="5988f-160">Get all section groups from all notebooks that are owned by the user, including nested section groups</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="5988f-161">Obtenha todos os grupos de seções que estão diretamente em um bloco de anotações específico</span><span class="sxs-lookup"><span data-stu-id="5988f-161">Get all section groups that are directly under a specific notebook</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="5988f-162">Os grupos de seções podem expandir as propriedades **sections**, **sectionGroups**, **parentNotebook** e **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="5988f-162">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="5988f-163">A ordem de classificação padrão para grupos de seções é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="5988f-163">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="5988f-164">A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.</span><span class="sxs-lookup"><span data-stu-id="5988f-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section-group"></a>
### <a name="sectiongroup-entity"></a><span data-ttu-id="5988f-165">Entidade SectionGroup</span><span class="sxs-lookup"><span data-stu-id="5988f-165">SectionGroup entity</span></span>

<span data-ttu-id="5988f-166">Obter um grupo de seções específico</span><span class="sxs-lookup"><span data-stu-id="5988f-166">Get a specific section group</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 


<span data-ttu-id="5988f-167">Os grupos de seções podem expandir as propriedades **sections**, **sectionGroups**, **parentNotebook** e **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="5988f-167">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="5988f-168">A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.</span><span class="sxs-lookup"><span data-stu-id="5988f-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-notebooks"></a>
### <a name="notebook-collection"></a><span data-ttu-id="5988f-169">Coleção de blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="5988f-169">notebook collection</span></span>

<span data-ttu-id="5988f-170">Obter todos os blocos de anotações de propriedade do usuário</span><span class="sxs-lookup"><span data-stu-id="5988f-170">Get all the notebooks that are owned by the user</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

 
<span data-ttu-id="5988f-171">Os blocos de anotações podem expandir as propriedades **sections** e **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="5988f-171">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="5988f-172">A ordem de classificação padrão para blocos de anotações é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="5988f-172">The default sort order is `name asc`.</span></span> 

- - -

<a name="get-notebook"></a>
### <a name="notebook-entity"></a><span data-ttu-id="5988f-173">Entidade Notebook</span><span class="sxs-lookup"><span data-stu-id="5988f-173">Notebook entity</span></span>

<span data-ttu-id="5988f-174">Obter um bloco de anotações `../notebooks/{notebook-id}[?select,expand]` específico</span><span class="sxs-lookup"><span data-stu-id="5988f-174">Get a specific notebook `../notebooks/{notebook-id}[?select,expand]`</span></span> 


<span data-ttu-id="5988f-175">Os blocos de anotações podem expandir as propriedades **sections** e **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="5988f-175">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

- - -

<a name="get-resource"></a>
### <a name="image-or-other-file-resource"></a><span data-ttu-id="5988f-176">Imagem ou outro recurso de arquivo</span><span class="sxs-lookup"><span data-stu-id="5988f-176">Image or other file resource</span></span>

<span data-ttu-id="5988f-177">Obtenha os dados binários de um recurso específico</span><span class="sxs-lookup"><span data-stu-id="5988f-177">Get the binary data of a specific resource by sending a GET request to the resource's  endpoint:</span></span> 

`../resources/{resource-id}/$value` 


<span data-ttu-id="5988f-178">Você pode encontrar a URI do recurso do arquivo na página de [HTML de saída](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="5988f-178">You can find the file's resource URI in the page's [output HTML](onenote_input_output_html.md).</span></span>

<span data-ttu-id="5988f-179">Por exemplo, um rótulo **img** inclui os pontos de extremidade para a imagem original no atributo **data-fullres-src** e a imagem otimizada no atributo **src**.</span><span class="sxs-lookup"><span data-stu-id="5988f-179">In the page HTML, an **** tag includes endpoints for the original image resource in the **** attribute and the optimized image in the **** attribute:</span></span> 

<span data-ttu-id="5988f-180">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="5988f-180">**Example**</span></span>

```
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="5988f-181">E um rótulo **object** inclui o ponto de extremidade para o recurso do arquivo no atributo **data**.</span><span class="sxs-lookup"><span data-stu-id="5988f-181">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

<span data-ttu-id="5988f-182">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="5988f-182">**Example**</span></span>

```
<object
    data="http://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

<span data-ttu-id="5988f-183">Para obter URLs públicas e pré-autenticadas para os recursos de imagem em uma página, inclua **preAuthenticated=true** na cadeia de caracteres de consulta ao [recuperar o conteúdo da página](#page-html-content) (**exemplo:**  `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="5988f-183">To get public URLs to the image resources on a page, include preAuthenticated=true in the query string when you retrieve the page content (example: ).</span></span> <span data-ttu-id="5988f-184">As URLs públicas que são retornadas no[HTML de saída](onenote_input_output_html.md#output-html-examples-for-images) são válidas por uma hora.</span><span class="sxs-lookup"><span data-stu-id="5988f-184">The public URLs that are returned are valid for one hour.</span></span> <span data-ttu-id="5988f-185">Sem este sinalizador, imagens recuperadas não serão renderizadas diretamente em um navegador, pois elas são privadas e é necessária autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="5988f-185">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> 

> <span data-ttu-id="5988f-186">**Observação:** não há suporte para obter uma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="5988f-186">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="5988f-187">Quando um recurso de arquivo é obtido, não é necessário incluir um tipo de conteúdo **Accept** na solicitação.</span><span class="sxs-lookup"><span data-stu-id="5988f-187">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="5988f-188">Para saber mais sobre solicitações GET, confira:</span><span class="sxs-lookup"><span data-stu-id="5988f-188">For more information about GET requests, see:</span></span> 
- [<span data-ttu-id="5988f-189">GET Pages</span><span class="sxs-lookup"><span data-stu-id="5988f-189">Get pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="5988f-190">GET Sections</span><span class="sxs-lookup"><span data-stu-id="5988f-190">GET Sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="5988f-191">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="5988f-191">GET SectionGroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="5988f-192">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="5988f-192">GET Notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 

<span data-ttu-id="5988f-193">na referência da API REST do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5988f-193">in the Microsoft Graph API REST reference.</span></span>


<a name="example"></a>
## <a name="example-get-requests"></a><span data-ttu-id="5988f-194">Exemplo de solicitações GET</span><span class="sxs-lookup"><span data-stu-id="5988f-194">Example GET requests</span></span>
<span data-ttu-id="5988f-195">Você pode consultar entidades do OneNote e o conteúdo de página de pesquisa para obter apenas as informações que você precisa.</span><span class="sxs-lookup"><span data-stu-id="5988f-195">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="5988f-196">Os exemplos a seguir mostram algumas maneiras de usar [opções de cadeia de caracteres de consulta com suporte](#supported-odata-query-string-options) em solicitações GET para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5988f-196">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="5988f-197">**Lembre-se:**</span><span class="sxs-lookup"><span data-stu-id="5988f-197">**Remember:**</span></span>

- <span data-ttu-id="5988f-198">Todas as solicitações GET começam com a [URL raiz de serviço raiz](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="5988f-198">All GET requests start with the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

  <span data-ttu-id="5988f-199">**Exemplos:**</span><span class="sxs-lookup"><span data-stu-id="5988f-199">**Examples**</span></span> 
  - `https://www.onenote.com/api/v1.0/me/notes`
  - `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`

- <span data-ttu-id="5988f-200">Os espaços na cadeia de caracteres de consulta da URL devem usar a codificação de %20.</span><span class="sxs-lookup"><span data-stu-id="5988f-200">Spaces in the URL query string must use %20 encoding.</span></span>

<span data-ttu-id="5988f-201">Exemplo: `filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="5988f-201">Example: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="5988f-202">Os nomes de propriedade e as comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5988f-202">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="5988f-203">É recomendável usar a função **tolower** do OData para comparações de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="5988f-203">We recommend using the OData **tolower** function for string comparisons.</span></span>

   <span data-ttu-id="5988f-204">Exemplo: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="5988f-204">Example: `filter=tolower(name) eq 'spring'`</span></span>
 

<span data-ttu-id="5988f-205">**search e filter**</span><span class="sxs-lookup"><span data-stu-id="5988f-205">**search & filter**</span></span>  

<span data-ttu-id="5988f-206">Obtenha todas as páginas que contêm o termo *recipe* que foram criados por um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="5988f-206">Get all pages that contain the term *recipe* that were created by a specific app.</span></span>  <span data-ttu-id="5988f-207">(`search` está disponível somente para blocos de anotações de consumidor)</span><span class="sxs-lookup"><span data-stu-id="5988f-207">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
<span data-ttu-id="5988f-208">**search e select**</span><span class="sxs-lookup"><span data-stu-id="5988f-208">**search & select**</span></span>  

<span data-ttu-id="5988f-209">Obtenha título, links de cliente do OneNote e o link **contentUrl** para todas as páginas que contêm o termo *golgi app*.</span><span class="sxs-lookup"><span data-stu-id="5988f-209">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app*.</span></span>  <span data-ttu-id="5988f-210">(`search` está disponível somente para blocos de anotações de consumidor)</span><span class="sxs-lookup"><span data-stu-id="5988f-210">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
<span data-ttu-id="5988f-211">**expand**</span><span class="sxs-lookup"><span data-stu-id="5988f-211">**expand**</span></span>  

<span data-ttu-id="5988f-212">Obtenha todos os blocos de anotações e expanda suas seções e grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="5988f-212">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```
 
<span data-ttu-id="5988f-213">Obtenha um grupo de seções específico e expanda suas seções e grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="5988f-213">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<span data-ttu-id="5988f-214">Obtenha uma página e expanda sua seção pai e o bloco de anotações pai.</span><span class="sxs-lookup"><span data-stu-id="5988f-214">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

<span data-ttu-id="5988f-215">**expand** (vários níveis)</span><span class="sxs-lookup"><span data-stu-id="5988f-215">**expand** (multiple levels)</span></span>  

<span data-ttu-id="5988f-216">Obtenha todos os blocos de anotações e expanda suas seções e grupos de seções, e expanda todas as seções em cada grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="5988f-216">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
><span data-ttu-id="5988f-217">Expanda pais de entidades filho ou expanda filhos de entidades pai cria uma referência circular e não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="5988f-217">Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
<span data-ttu-id="5988f-218">**expand e select ** (vários níveis)</span><span class="sxs-lookup"><span data-stu-id="5988f-218">**expand & select** (multiple levels)</span></span>  

<span data-ttu-id="5988f-219">Obtenha o nome e o **self** link para um grupo de seções específico, e obtenha o nome e os **self** links para todas as suas seções.</span><span class="sxs-lookup"><span data-stu-id="5988f-219">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```
 
<span data-ttu-id="5988f-220">Obtenha o nome e o **self** link para todas as seções e o nome e o tempo criados de cada bloco de anotações pai da seção.</span><span class="sxs-lookup"><span data-stu-id="5988f-220">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```
 
<span data-ttu-id="5988f-221">Obtenha o título e uma ID de todas as páginas, e o nome da seção pai e do bloco de anotações pai.</span><span class="sxs-lookup"><span data-stu-id="5988f-221">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

<span data-ttu-id="5988f-222">**expand e levels ** (vários níveis)</span><span class="sxs-lookup"><span data-stu-id="5988f-222">**expand & levels** (multiple levels)</span></span>  

<span data-ttu-id="5988f-223">Obtenha todos os blocos de anotações, seções e grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="5988f-223">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
<span data-ttu-id="5988f-224">**filter**</span><span class="sxs-lookup"><span data-stu-id="5988f-224">**filter**</span></span>  

<span data-ttu-id="5988f-225">Obtenha todas as seções que foram criadas em outubro de 2014.</span><span class="sxs-lookup"><span data-stu-id="5988f-225">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<span data-ttu-id="5988f-226">Obtenha as páginas que foram criadas por um aplicativo específico desde 1º de janeiro de 2015.</span><span class="sxs-lookup"><span data-stu-id="5988f-226">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

<span data-ttu-id="5988f-227">**filter e expand**</span><span class="sxs-lookup"><span data-stu-id="5988f-227">**filter & expand**</span></span>  

<span data-ttu-id="5988f-228">Obtenha todas as páginas em um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="5988f-228">Get all pages in a specific notebook.</span></span> <span data-ttu-id="5988f-229">A API retorna 20 entradas por padrão.</span><span class="sxs-lookup"><span data-stu-id="5988f-229">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<span data-ttu-id="5988f-230">Obtenha o nome e o link **pagesUrl** para todas as seções do bloco de anotações *School*.</span><span class="sxs-lookup"><span data-stu-id="5988f-230">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="5988f-231">Comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas, portanto, use a função **tolower** como uma prática recomendada.</span><span class="sxs-lookup"><span data-stu-id="5988f-231">OData string comparisons are case sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

<span data-ttu-id="5988f-232">**filter, select e orderby**</span><span class="sxs-lookup"><span data-stu-id="5988f-232">**filter & select & orderby**</span></span>   

<span data-ttu-id="5988f-233">Obtenha o nome e o link **pagesUrl** para todas as seções que contêm o termo *spring* no nome da seção.</span><span class="sxs-lookup"><span data-stu-id="5988f-233">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name.</span></span> <span data-ttu-id="5988f-234">Ordenar seções de pedidos por última data modificada.</span><span class="sxs-lookup"><span data-stu-id="5988f-234">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
<span data-ttu-id="5988f-235">**orderby**</span><span class="sxs-lookup"><span data-stu-id="5988f-235">**orderby**</span></span>  

<span data-ttu-id="5988f-236">Obtenha as primeiras 20 páginas pela propriedade **createdByAppId** e, depois, pela hora de criação mais recente.</span><span class="sxs-lookup"><span data-stu-id="5988f-236">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time.</span></span> <span data-ttu-id="5988f-237">A API retorna 20 entradas por padrão.</span><span class="sxs-lookup"><span data-stu-id="5988f-237">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

<span data-ttu-id="5988f-238">**search, filter e top**</span><span class="sxs-lookup"><span data-stu-id="5988f-238">**search & filter & top**</span></span>  

<span data-ttu-id="5988f-239">Obtenha as cinco páginas mais recentemente criadas desde 1º de janeiro de 2015 com a frase *cell division*.</span><span class="sxs-lookup"><span data-stu-id="5988f-239">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="5988f-240">A API retorna 20 entradas por padrão com um máximo de 100.</span><span class="sxs-lookup"><span data-stu-id="5988f-240">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="5988f-241">A ordem de classificação padrão é `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="5988f-241">The default sort order is `lastModifiedTime desc`.</span></span> <span data-ttu-id="5988f-242">(`search` está disponível somente para blocos de anotações de consumidor)</span><span class="sxs-lookup"><span data-stu-id="5988f-242">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

<span data-ttu-id="5988f-243">**search, filter, top e skip**</span><span class="sxs-lookup"><span data-stu-id="5988f-243">**search & filter & top & skip**</span></span>  

<span data-ttu-id="5988f-244">Obtenha as próximas cinco páginas do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="5988f-244">Get the next five pages in the result set.</span></span> <span data-ttu-id="5988f-245">(`search` está disponível somente para blocos de anotações de consumidor)</span><span class="sxs-lookup"><span data-stu-id="5988f-245">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<span data-ttu-id="5988f-246">E as cinco posteriores.</span><span class="sxs-lookup"><span data-stu-id="5988f-246">And the next five.</span></span> <span data-ttu-id="5988f-247">(`search` está disponível somente para blocos de anotações de consumidor)</span><span class="sxs-lookup"><span data-stu-id="5988f-247">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="5988f-248">**Observação:** se **search** e **filter** são aplicadas à mesma solicitação, os resultados incluem apenas as entidades que correspondem aos dois critérios.</span><span class="sxs-lookup"><span data-stu-id="5988f-248">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
<span data-ttu-id="5988f-249">**select**</span><span class="sxs-lookup"><span data-stu-id="5988f-249">**select**</span></span>  

<span data-ttu-id="5988f-250">Obtenha nome, hora de criação e **self** link de todas as seções nos blocos de anotações do usuário.</span><span class="sxs-lookup"><span data-stu-id="5988f-250">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<span data-ttu-id="5988f-251">Obtenha título, hora de criação e links do cliente do OneNote para uma página específica.</span><span class="sxs-lookup"><span data-stu-id="5988f-251">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

<span data-ttu-id="5988f-252">**select, expand e filter** (vários níveis)</span><span class="sxs-lookup"><span data-stu-id="5988f-252">**select & expand & filter** (multiple levels)</span></span>  

<span data-ttu-id="5988f-253">Obtenha nome e link **pagesUrl** para todas as seções do bloco de anotações do usuário.</span><span class="sxs-lookup"><span data-stu-id="5988f-253">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

<span data-ttu-id="5988f-254">**top, select e orderby**</span><span class="sxs-lookup"><span data-stu-id="5988f-254">**top & select & orderby**</span></span>  

<span data-ttu-id="5988f-255">Obtenha o título e o link **self** das 50 primeiras páginas, classificadas em ordem alfabética por título.</span><span class="sxs-lookup"><span data-stu-id="5988f-255">Get the title and **self** link for the first 50 pages, ordered alphabetically by title.</span></span> <span data-ttu-id="5988f-256">A API retorna 20 entradas por padrão com um máximo de 100.</span><span class="sxs-lookup"><span data-stu-id="5988f-256">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="5988f-257">A ordem de classificação padrão é `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="5988f-257">The default sort order is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

<span data-ttu-id="5988f-258">**skip, top, select e orderby**</span><span class="sxs-lookup"><span data-stu-id="5988f-258">**skip & top & select & orderby**</span></span>  

<span data-ttu-id="5988f-259">Obtenha páginas de 51 a 100.</span><span class="sxs-lookup"><span data-stu-id="5988f-259">Get pages 51 to 100.</span></span> <span data-ttu-id="5988f-260">A API retorna 20 entradas por padrão com um máximo de 100.</span><span class="sxs-lookup"><span data-stu-id="5988f-260">The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="5988f-261">**Observação:** solicitações GET para páginas que recuperam o número de entradas padrão (ou seja, não especificar uma expressão **top**) retornam um link **@odata.nextLink** na resposta que você pode usar para obter as próximas 20 entradas.</span><span class="sxs-lookup"><span data-stu-id="5988f-261">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="query-options"></a>
## <a name="supported-odata-query-string-options"></a><span data-ttu-id="5988f-262">Opções de cadeia de caracteres de consulta OData com suporte.</span><span class="sxs-lookup"><span data-stu-id="5988f-262">See Supported OData query string options.</span></span>

<span data-ttu-id="5988f-263">Quando enviar solicitações GET para Microsoft Graph, você pode usar as opções de cadeia de caracteres de consulta de OData para personalizar sua consulta e obter apenas as informações que você precisa.</span><span class="sxs-lookup"><span data-stu-id="5988f-263">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="5988f-264">Também podem melhorar o desempenho, reduzindo o número de chamadas para o serviço e o tamanho da carga de resposta.</span><span class="sxs-lookup"><span data-stu-id="5988f-264">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="5988f-265">**Observação:** para facilitar a leitura, os exemplos neste artigo não usam a codificação de %20 necessária para espaços na cadeia de caracteres de consulta da URL: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="5988f-265">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="5988f-266">Opção de consulta</span><span class="sxs-lookup"><span data-stu-id="5988f-266">Query option</span></span> | <span data-ttu-id="5988f-267">Exemplo e descrição</span><span class="sxs-lookup"><span data-stu-id="5988f-267">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="5988f-268">count</span><span class="sxs-lookup"><span data-stu-id="5988f-268">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="5988f-269">A contagem de entidades da coleção.</span><span class="sxs-lookup"><span data-stu-id="5988f-269">The count of entities in the collection.</span></span> <span data-ttu-id="5988f-270">O valor é retornado na propriedade **@odata.count** na resposta.</span><span class="sxs-lookup"><span data-stu-id="5988f-270">The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="5988f-271">expand</span><span class="sxs-lookup"><span data-stu-id="5988f-271">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="5988f-272">Propriedades de navegação para retornar embutidas na resposta.</span><span class="sxs-lookup"><span data-stu-id="5988f-272">The navigation properties to return inline in the response.</span></span> <span data-ttu-id="5988f-273">As propriedades a seguir têm suporte para expressões **expand**:</span><span class="sxs-lookup"><span data-stu-id="5988f-273">The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="5988f-274">– Páginas: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="5988f-274">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="5988f-275">– Seções: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="5988f-275">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="5988f-276">– Grupos de seções: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="5988f-276">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="5988f-277">– Blocos de anotações: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="5988f-277">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="5988f-278">Por padrão, as solicitações GET de páginas expandem **parentSection** e selecionam as propriedades **id**, **name** e **self**.</span><span class="sxs-lookup"><span data-stu-id="5988f-278">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties.</span></span> <span data-ttu-id="5988f-279">Solicitações GET padrão de seções e grupos de seções expandem **parentNotebook** e **parentSectionGroup** e selecionam as propriedades pai **id**, **name** e **self**.</span><span class="sxs-lookup"><span data-stu-id="5988f-279">Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties.</span></span> </p><p><span data-ttu-id="5988f-280">Pode ser usado para uma única entidade ou uma coleção.</span><span class="sxs-lookup"><span data-stu-id="5988f-280">Can be used for a single entity or a collection.</span></span> <span data-ttu-id="5988f-281">Separar com vírgulas várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="5988f-281">Separate multiple properties with commas.</span></span> <span data-ttu-id="5988f-282">Os nomes de propriedades diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5988f-282">Property names are case sensitive.</span></span></p> |   
| <span data-ttu-id="5988f-283">filter</span><span class="sxs-lookup"><span data-stu-id="5988f-283">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="5988f-284">Uma expressão booliana para se deseja incluir uma entrada no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="5988f-284">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="5988f-285">Compatível com os seguintes operadores e funções OData:</span><span class="sxs-lookup"><span data-stu-id="5988f-285">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="5988f-286">– Operadores de comparação: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span><span class="sxs-lookup"><span data-stu-id="5988f-286">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="5988f-287">– Operadores lógicos: **and**, **or**, **not**</span><span class="sxs-lookup"><span data-stu-id="5988f-287">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="5988f-288">– Funções de cadeia de caracteres: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span><span class="sxs-lookup"><span data-stu-id="5988f-288">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="5988f-289">Nomes de [propriedade](#onenote-entity-properties) e comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5988f-289">[Property](#onenote-entity-properties) names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="5988f-290">É recomendável usar a função **tolower** do OData para comparações de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="5988f-290">We recommend using the OData **tolower** function for string comparisons.</span></span> <span data-ttu-id="5988f-291">Exemplo: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="5988f-291">Example: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="5988f-292">orderby</span><span class="sxs-lookup"><span data-stu-id="5988f-292">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="5988f-293">As [propriedades](#onenote-entity-properties) para classificar por, com uma ordem de classificação opcional **asc** (padrão) ou **desc**.</span><span class="sxs-lookup"><span data-stu-id="5988f-293">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order.</span></span> <span data-ttu-id="5988f-294">Você pode classificar por qualquer propriedade da entidade na coleção solicitada.</span><span class="sxs-lookup"><span data-stu-id="5988f-294">You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="5988f-295">A ordem de classificação padrão para blocos de anotações, grupos de seções e seções é `name asc`, e para páginas é `lastModifiedTime desc` (última página modificada primeiro).</span><span class="sxs-lookup"><span data-stu-id="5988f-295">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="5988f-296">Separe as várias propriedades com vírgulas e liste-as na ordem de aplicação desejada.</span><span class="sxs-lookup"><span data-stu-id="5988f-296">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="5988f-297">Os nomes de propriedades diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5988f-297">Property names are case sensitive.</span></span></p> |  
| <span data-ttu-id="5988f-298">search</span><span class="sxs-lookup"><span data-stu-id="5988f-298">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="5988f-299">Disponível somente para blocos de anotações de consumidor.</span><span class="sxs-lookup"><span data-stu-id="5988f-299">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="5988f-300">O termo ou frase para pesquisar no título da página, corpo da página, texto alt da imagem e texto da imagem OCR.</span><span class="sxs-lookup"><span data-stu-id="5988f-300">The term or phrase to search for in the page title, page body, image alt text, and image OCR text.</span></span> <span data-ttu-id="5988f-301">Por padrão, consultas de pesquisa retornam resultados classificados por relevância.</span><span class="sxs-lookup"><span data-stu-id="5988f-301">By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="5988f-302">O OneNote usa a pesquisa de texto completo do Bing para dar suporte a pesquisa de frase, lematização, tolerância de ortografia, relevância e classificação, quebra de palavras, vários idiomas e outros recursos de pesquisa de texto completo.</span><span class="sxs-lookup"><span data-stu-id="5988f-302">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="5988f-303">As cadeias de caracteres de pesquisa diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5988f-303">Search strings are case insensitive.</span></span></p><p><span data-ttu-id="5988f-304">Aplica-se somente a páginas em blocos de anotações de propriedade do usuário (não compartilhados com o usuário).</span><span class="sxs-lookup"><span data-stu-id="5988f-304">Applies only to pages in notebooks owned by the user (not shared with the user).</span></span> <span data-ttu-id="5988f-305">O conteúdo indexado é privado e só pode ser acessado pelo proprietário.</span><span class="sxs-lookup"><span data-stu-id="5988f-305">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="5988f-306">As páginas protegidas por senha não são indexadas.</span><span class="sxs-lookup"><span data-stu-id="5988f-306">Password-protected pages are not indexed.</span></span> <span data-ttu-id="5988f-307">Aplicável somente ao ponto de extremidade `pages`.</span><span class="sxs-lookup"><span data-stu-id="5988f-307">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="5988f-308">select</span><span class="sxs-lookup"><span data-stu-id="5988f-308">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="5988f-309">As [propriedades](#onenote-entity-properties) a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="5988f-309">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="5988f-310">Pode ser usado para uma única entidade ou para uma coleção.</span><span class="sxs-lookup"><span data-stu-id="5988f-310">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="5988f-311">Separar com vírgulas várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="5988f-311">Separate multiple properties with commas.</span></span> <span data-ttu-id="5988f-312">Os nomes de propriedades diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5988f-312">Property names are case sensitive.</span></span></p> |  
| <span data-ttu-id="5988f-313">skip</span><span class="sxs-lookup"><span data-stu-id="5988f-313">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="5988f-314">O número de entradas para ignorar no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="5988f-314">The number of items to skip in a result set.</span></span> <span data-ttu-id="5988f-315">Costumam ser usadas para resultados de paginação.</span><span class="sxs-lookup"><span data-stu-id="5988f-315">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="5988f-316">top</span><span class="sxs-lookup"><span data-stu-id="5988f-316">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="5988f-317">O número de entradas para retornar do conjunto de resultados, até um máximo de 100.</span><span class="sxs-lookup"><span data-stu-id="5988f-317">The number of entries to return in the result set, up to a maximum of 100.</span></span> <span data-ttu-id="5988f-318">O valor padrão é 20.</span><span class="sxs-lookup"><span data-stu-id="5988f-318">The default value is 20.</span></span></p> |  

<span data-ttu-id="5988f-319">O Microsoft Graph também fornece a opção de cadeia de caracteres de consulta `pagelevel` que você pode usar para obter o nível e ordem das páginas dentro da seção pai.</span><span class="sxs-lookup"><span data-stu-id="5988f-319">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="5988f-320">Aplicam-se apenas às consultas de páginas em uma seção específica ou consultas para uma página específica.</span><span class="sxs-lookup"><span data-stu-id="5988f-320">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

<span data-ttu-id="5988f-321">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="5988f-321">**Example**</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="5988f-322">Funções e operadores de OData compatíveis</span><span class="sxs-lookup"><span data-stu-id="5988f-322">Supported OData operators and functions</span></span>

<span data-ttu-id="5988f-323">Microsoft Graph é compatível com os seguintes operadores e funções do OData nas expressões de **filter**.</span><span class="sxs-lookup"><span data-stu-id="5988f-323">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="5988f-324">Ao usar expressões de OData, lembre-se:</span><span class="sxs-lookup"><span data-stu-id="5988f-324">When using OData expressions, remember:</span></span>  
- <span data-ttu-id="5988f-325">Os espaços na cadeia de caracteres de consulta da URL devem ser substituídos pela codificação `%20`.</span><span class="sxs-lookup"><span data-stu-id="5988f-325">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span>

   <span data-ttu-id="5988f-326">**Exemplo:** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="5988f-326">Example</span></span>
- <span data-ttu-id="5988f-327">Os nomes de propriedade e as comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5988f-327">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="5988f-328">É recomendável usar a função **tolower** do OData para comparações de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="5988f-328">We recommend using the OData **tolower** function for string comparisons.</span></span>
   
   <span data-ttu-id="5988f-329">**Exemplo:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="5988f-329">Example</span></span>

| <span data-ttu-id="5988f-330">Operador de comparação</span><span class="sxs-lookup"><span data-stu-id="5988f-330">comparison operator</span></span> | <span data-ttu-id="5988f-331">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5988f-331">Example</span></span> |  
|------|------|  
| <span data-ttu-id="5988f-332">eq</span><span class="sxs-lookup"><span data-stu-id="5988f-332">EQ</span></span><br /><span data-ttu-id="5988f-333">(igual a)</span><span class="sxs-lookup"><span data-stu-id="5988f-333">Equal to</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="5988f-334">ne</span><span class="sxs-lookup"><span data-stu-id="5988f-334">ne</span></span><br /><span data-ttu-id="5988f-335">(é diferente de)</span><span class="sxs-lookup"><span data-stu-id="5988f-335">Not equal to</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="5988f-336">gt</span><span class="sxs-lookup"><span data-stu-id="5988f-336">gt;</span></span><br /><span data-ttu-id="5988f-337">(maior que)</span><span class="sxs-lookup"><span data-stu-id="5988f-337">Greater than</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="5988f-338">ge</span><span class="sxs-lookup"><span data-stu-id="5988f-338">ge</span></span><br /><span data-ttu-id="5988f-339">(maior que ou igual a)</span><span class="sxs-lookup"><span data-stu-id="5988f-339">Greater than or equal to.</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="5988f-340">lt</span><span class="sxs-lookup"><span data-stu-id="5988f-340">lt;</span></span><br /><span data-ttu-id="5988f-341">(menor que)</span><span class="sxs-lookup"><span data-stu-id="5988f-341">Less than</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="5988f-342">le</span><span class="sxs-lookup"><span data-stu-id="5988f-342">le</span></span><br /><span data-ttu-id="5988f-343">(menor que ou igual a)</span><span class="sxs-lookup"><span data-stu-id="5988f-343">Less than or equal to.</span></span> | `lastModifiedTime le 2014-02-23` |  
 
| <span data-ttu-id="5988f-344">Operador lógico</span><span class="sxs-lookup"><span data-stu-id="5988f-344">Logical operator</span></span> | <span data-ttu-id="5988f-345">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5988f-345">Example</span></span> |  
|------|------|  
| <span data-ttu-id="5988f-346">e</span><span class="sxs-lookup"><span data-stu-id="5988f-346">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="5988f-347">or</span><span class="sxs-lookup"><span data-stu-id="5988f-347">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="5988f-348">not</span><span class="sxs-lookup"><span data-stu-id="5988f-348">NOT</span></span> | `not contains(tolower(title),'school')` |  
 
| <span data-ttu-id="5988f-349">Função da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5988f-349">String Function</span></span> | <span data-ttu-id="5988f-350">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5988f-350">Example</span></span> |  
|------|------|   
| <span data-ttu-id="5988f-351">contains</span><span class="sxs-lookup"><span data-stu-id="5988f-351">"contains"</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="5988f-352">endswith</span><span class="sxs-lookup"><span data-stu-id="5988f-352">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="5988f-353">startswith</span><span class="sxs-lookup"><span data-stu-id="5988f-353">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="5988f-354">length</span><span class="sxs-lookup"><span data-stu-id="5988f-354">Length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="5988f-355">indexof</span><span class="sxs-lookup"><span data-stu-id="5988f-355">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="5988f-356">substring</span><span class="sxs-lookup"><span data-stu-id="5988f-356">Substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="5988f-357">tolower</span><span class="sxs-lookup"><span data-stu-id="5988f-357">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="5988f-358">toupper</span><span class="sxs-lookup"><span data-stu-id="5988f-358">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="5988f-359">trim</span><span class="sxs-lookup"><span data-stu-id="5988f-359">Trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="5988f-360">concat</span><span class="sxs-lookup"><span data-stu-id="5988f-360">CONCAT</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>
## <a name="onenote-entity-properties"></a><span data-ttu-id="5988f-361">Propriedades de entidade do OneNote</span><span class="sxs-lookup"><span data-stu-id="5988f-361">OneNote entity properties</span></span>

<span data-ttu-id="5988f-362">As expressões de consulta **filter**, **select**, **expand** e **orderby** podem incluir propriedades de entidades do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5988f-362">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

<span data-ttu-id="5988f-363">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="5988f-363">**Example**</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="5988f-364">Os nomes de propriedades diferenciam maiúsculas de minúsculas em expressões de consulta.</span><span class="sxs-lookup"><span data-stu-id="5988f-364">Property names are case sensitive in query expressions.</span></span>

<span data-ttu-id="5988f-365">Para uma lista de propriedades e tipos de propriedades, confira:</span><span class="sxs-lookup"><span data-stu-id="5988f-365">For the list of properties and property types, see:</span></span>

- [<span data-ttu-id="5988f-366">GET Pages</span><span class="sxs-lookup"><span data-stu-id="5988f-366">Get pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="5988f-367">GET Sections</span><span class="sxs-lookup"><span data-stu-id="5988f-367">GET Sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="5988f-368">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="5988f-368">GET SectionGroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="5988f-369">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="5988f-369">GET Notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 

<span data-ttu-id="5988f-370">na referência da API REST do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5988f-370">in the Microsoft Graph API REST reference.</span></span>

<span data-ttu-id="5988f-371">A opção de cadeia de caracteres de consulta **expand** pode ser usada com as seguintes propriedades de navegação:</span><span class="sxs-lookup"><span data-stu-id="5988f-371">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="5988f-372">Páginas: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="5988f-372">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="5988f-373">Seções: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="5988f-373">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="5988f-374">Grupos de seções: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="5988f-374">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="5988f-375">Blocos de anotações: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="5988f-375">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>
## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="5988f-376">Informações de solicitação e resposta para solicitações de *GET*</span><span class="sxs-lookup"><span data-stu-id="5988f-376">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="5988f-377">Dados da solicitação</span><span class="sxs-lookup"><span data-stu-id="5988f-377">Request data</span></span> | <span data-ttu-id="5988f-378">Descrição</span><span class="sxs-lookup"><span data-stu-id="5988f-378">Description</span></span> |  
|------|------|  
| <span data-ttu-id="5988f-379">Protocolo</span><span class="sxs-lookup"><span data-stu-id="5988f-379">Protocol</span></span> | <span data-ttu-id="5988f-380">Todas as solicitações usam o protocolo HTTPS de SSL/TLS.</span><span class="sxs-lookup"><span data-stu-id="5988f-380">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="5988f-381">Cabeçalho de autorização</span><span class="sxs-lookup"><span data-stu-id="5988f-381">Authorization header</span></span> | <p><span data-ttu-id="5988f-382">`Bearer {token}`, onde *{token}* é um token de acesso do OAuth 2.0 válido para o aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="5988f-382">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="5988f-383">Se ele estiver ausente ou for inválido, a solicitação falhará com um código de status 401.</span><span class="sxs-lookup"><span data-stu-id="5988f-383">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="5988f-384">Confira [Autenticação e permissões](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5988f-384">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="5988f-385">Cabeçalho Accept</span><span class="sxs-lookup"><span data-stu-id="5988f-385">accept header</span></span> | <p><span data-ttu-id="5988f-386">- `application/json` para entidades e conjunto de entidades do OneNote</span><span class="sxs-lookup"><span data-stu-id="5988f-386">- `application/json` for OneNote entities and entity sets</span></span></p><p><span data-ttu-id="5988f-387">- `text/html` para conteúdo de página</span><span class="sxs-lookup"><span data-stu-id="5988f-387">- `text/html` for page content</span></span></p> | 

| <span data-ttu-id="5988f-388">Dados de resposta</span><span class="sxs-lookup"><span data-stu-id="5988f-388">Response data</span></span> | <span data-ttu-id="5988f-389">Descrição</span><span class="sxs-lookup"><span data-stu-id="5988f-389">Description</span></span> |  
|------|------|  
| <span data-ttu-id="5988f-390">Código de êxito</span><span class="sxs-lookup"><span data-stu-id="5988f-390">Success code</span></span> | <span data-ttu-id="5988f-391">Um código de status de HTTP 200.</span><span class="sxs-lookup"><span data-stu-id="5988f-391">A 200 (OK) status code.</span></span> |  
| <span data-ttu-id="5988f-392">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="5988f-392">Response body</span></span> | <span data-ttu-id="5988f-393">Uma representação de OData da entidade ou conjunto de entidades no formato JSON, da página HTML ou dados binários do recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="5988f-393">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="5988f-394">Erros</span><span class="sxs-lookup"><span data-stu-id="5988f-394">Errors</span></span> | <span data-ttu-id="5988f-395">Se a solicitação falhar, a API retornará [erros](onenote_error_codes.md) no objeto **@api.diagnostics** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5988f-395">If the request fails, the API returns [errors](onenote_error_codes.md) in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="5988f-396">Cabeçalho X-CorrelationId</span><span class="sxs-lookup"><span data-stu-id="5988f-396">X-CorrelationId header</span></span> | <span data-ttu-id="5988f-397">Um GUID que identifica de forma exclusiva a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5988f-397">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="5988f-398">Você pode usar esse valor juntamente com o valor do cabeçalho Data ao trabalhar com o suporte da Microsoft para solucionar problemas.</span><span class="sxs-lookup"><span data-stu-id="5988f-398">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>
### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="5988f-399">Criar a URL raiz do serviço de anotações do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5988f-399">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="5988f-400">A URL raiz do serviço de anotações do Microsoft Graph usa o formato a seguir para todas as chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5988f-400">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes.</span></span> <span data-ttu-id="5988f-401">`https://graph.microsoft.com/{version}/me/onenote/`  O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="5988f-401">`https://graph.microsoft.com/{version}/me/onenote/`  The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="5988f-402">Use `v1.0` para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="5988f-402">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="5988f-403">Use `beta` para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="5988f-403">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="5988f-404">Os recursos e a funcionalidade na versão beta podem mudar, por isso, você não deve usá-la no código de produção.</span><span class="sxs-lookup"><span data-stu-id="5988f-404">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> <span data-ttu-id="5988f-405">Use `me` para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="5988f-405">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="5988f-406">Use `users/{id}` para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="5988f-406">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="5988f-407">Use o [Microsoft Graph](https://graph.microsoft.com/v1.0/users) para obter as IDs de usuário.</span><span class="sxs-lookup"><span data-stu-id="5988f-407">Use the [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>
## <a name="permissions-for-get-requests"></a><span data-ttu-id="5988f-408">Permissões para solicitações GET</span><span class="sxs-lookup"><span data-stu-id="5988f-408">Permissions for GET requests</span></span>

<span data-ttu-id="5988f-409">Para obter conteúdo ou estrutura do OneNote, você vai precisar solicitar as permissões adequadas.</span><span class="sxs-lookup"><span data-stu-id="5988f-409">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="5988f-410">Os seguintes escopos permitem solicitações GET para Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5988f-410">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="5988f-411">Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="5988f-411">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="5988f-412">Escolha entre:</span><span class="sxs-lookup"><span data-stu-id="5988f-412">Choose from:</span></span> 
- <span data-ttu-id="5988f-413">Notes.read</span><span class="sxs-lookup"><span data-stu-id="5988f-413">Notes.Read</span></span>
- <span data-ttu-id="5988f-414">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5988f-414">Notes.ReadWrite</span></span>
- <span data-ttu-id="5988f-415">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5988f-415">Notes.ReadWrite.All</span></span>


<span data-ttu-id="5988f-416">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Referência de permissões do Microsoft Graph](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5988f-416">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>

<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="5988f-417">Recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="5988f-417">Additional resources</span></span>

- [<span data-ttu-id="5988f-418">HTML de entrada e saída para páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="5988f-418">Input and output HTML in OneNote pages</span></span>](onenote_input_output_html.md)
- [<span data-ttu-id="5988f-419">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="5988f-419">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="5988f-420">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="5988f-420">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="5988f-421">Perguntas sobre desenvolvimento do OneNote no Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="5988f-421">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="5988f-422">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="5988f-422">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
