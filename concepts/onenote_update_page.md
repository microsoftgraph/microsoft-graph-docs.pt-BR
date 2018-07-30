# <a name="update-onenote-page-content"></a><span data-ttu-id="e159e-101">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="e159e-101">Update OneNote page content</span></span>

<span data-ttu-id="e159e-102">**Aplica-se a** Blocos de anotações de consumidor no OneDrive | Blocos de anotações empresariais no Office 365</span><span class="sxs-lookup"><span data-stu-id="e159e-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>


<span data-ttu-id="e159e-103">Para atualizar o conteúdo de uma página do OneNote, envie uma solicitação de PATCH para o ponto de extremidade do *conteúdo* da página:</span><span class="sxs-lookup"><span data-stu-id="e159e-103">To update the content of a OneNote page, you send a PATCH request to the page's *content* endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="e159e-104">Envie um objeto de alteração JSON no corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e159e-104">Send a JSON change object in the message body.</span></span> <span data-ttu-id="e159e-105">Se a solicitação for bem-sucedida, o Microsoft Graph retornará um código de status de HTTP 204.</span><span class="sxs-lookup"><span data-stu-id="e159e-105">If the request is successful, the Microsoft Graph returns a 204 HTTP status code.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="e159e-106">Construir a URI de solicitação</span><span class="sxs-lookup"><span data-stu-id="e159e-106">Construct the request URI</span></span>

<span data-ttu-id="e159e-107">Para construir a URI de solicitação, comece com a URL raiz do serviço:</span><span class="sxs-lookup"><span data-stu-id="e159e-107">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="e159e-108">Acrescente então o ponto de extremidade do *conteúdo* da página:</span><span class="sxs-lookup"><span data-stu-id="e159e-108">Then append the page's *content* endpoint:</span></span>

- <span data-ttu-id="e159e-109">**Obter o HTML da página e todos os valores de *data-id* definidos**</span><span class="sxs-lookup"><span data-stu-id="e159e-109">**Get the page HTML and all defined *data-id* values**</span></span><br/><br/>`../pages/{id}/content`   

- <span data-ttu-id="e159e-110">**Obter o HTML da página, todos os valores de *data-id* definidos e todos os valores de *id* gerados**</span><span class="sxs-lookup"><span data-stu-id="e159e-110">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span><br/><br/>`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="e159e-111">A **data-id** e os valores de **id** são usados como identificadores de **destino** para elementos que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="e159e-111">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="e159e-112">Sua solicitação de URI completa terá a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="e159e-112">Your full request URI will look like this:</span></span><br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="e159e-113">Saiba mais sobre a [URL raiz de serviço](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="e159e-113">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="e159e-114">Criar o corpo da mensagem</span><span class="sxs-lookup"><span data-stu-id="e159e-114">Construct the message body</span></span>

<span data-ttu-id="e159e-115">O HTML de uma página do OneNote contém texto, imagens e outros conteúdos organizados em estruturas como elementos **div**, **img** e **ol**.</span><span class="sxs-lookup"><span data-stu-id="e159e-115">The HTML of a OneNote page contains text, images, and other content organized into structures such as **div**, **img**, and **ol** elements.</span></span> <span data-ttu-id="e159e-116">Para atualizar o conteúdo da página do OneNote, adicione e substitua elementos HTML na página.</span><span class="sxs-lookup"><span data-stu-id="e159e-116">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="e159e-117">Suas alterações serão enviadas no corpo da mensagem como uma matriz de objetos de alteração JSON.</span><span class="sxs-lookup"><span data-stu-id="e159e-117">Your changes are sent in the message body as an array of JSON change objects.</span></span> <span data-ttu-id="e159e-118">Cada objeto especifica o elemento de destino, o novo conteúdo HTML e o que fazer com o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e159e-118">Each object specifies the target element, new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="e159e-119">A matriz a seguir define duas alterações.</span><span class="sxs-lookup"><span data-stu-id="e159e-119">The following array defines two changes.</span></span> <span data-ttu-id="e159e-120">A primeira insere uma imagem acima de um parágrafo como um irmão, e a segunda acrescenta um item em uma lista como um último filho.</span><span class="sxs-lookup"><span data-stu-id="e159e-120">The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

<span data-ttu-id="e159e-121">Veja [mais exemplos](#example-requests).</span><span class="sxs-lookup"><span data-stu-id="e159e-121">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="e159e-122">Atributos de objetos de alteração JSON</span><span class="sxs-lookup"><span data-stu-id="e159e-122">Attributes for JSON change objects</span></span>

<span data-ttu-id="e159e-123">Use atributos **target**, **action**, **position** e **content** para definir objetos JSON para solicitações de PATCH.</span><span class="sxs-lookup"><span data-stu-id="e159e-123">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

#### <a name="target"></a><span data-ttu-id="e159e-124">destino</span><span class="sxs-lookup"><span data-stu-id="e159e-124">target</span></span>

<span data-ttu-id="e159e-125">O elemento a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="e159e-125">The element to update.</span></span> <span data-ttu-id="e159e-126">O valor deve ser uma dos seguintes identificadores:</span><span class="sxs-lookup"><span data-stu-id="e159e-126">The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="e159e-127">Identificador</span><span class="sxs-lookup"><span data-stu-id="e159e-127">Identifier</span></span> | <span data-ttu-id="e159e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e159e-128">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e159e-129">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="e159e-129">#{data-id}</span></span> | <p><span data-ttu-id="e159e-130">Essa ID é opcionalmente definida em elementos na HTML de entrada ao [criar uma página](onenote-create-page.md) ou [atualizar uma página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="e159e-130">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote_update_page.md).</span></span> <span data-ttu-id="e159e-131">Coloque um # como prefixo do valor.</span><span class="sxs-lookup"><span data-stu-id="e159e-131">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="e159e-132">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="e159e-132">Example:</span></span><br/><span data-ttu-id="e159e-133">`'target':'#intro'` tem como destino o elemento `<div data-id="intro" ...>`</span><span class="sxs-lookup"><span data-stu-id="e159e-133">Example: `'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="e159e-134">id</span><span class="sxs-lookup"><span data-stu-id="e159e-134">id</span></span> | <p><span data-ttu-id="e159e-135">É a [ID gerada](#generated-ids) do Microsoft Graph e é necessário para a maioria das operações de substituição.</span><span class="sxs-lookup"><span data-stu-id="e159e-135">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="e159e-136">Não use # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="e159e-136">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="e159e-137">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="e159e-137">Example:</span></span><br/><span data-ttu-id="e159e-138">`'target':'div:{33f8a2...}{37}'` tem como destino o elemento `<div id="div:{33f8a2...}{37}" ...>`</span><span class="sxs-lookup"><span data-stu-id="e159e-138">Example: `'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="e159e-139">Não confunda esses identificadores com valores de **id** definidos no [HTML de entrada](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="e159e-139">Don't confuse these with any **id** values defined in the [input HTML](onenote_input_output_html.md).</span></span> <span data-ttu-id="e159e-140">Todos os valores de **id** enviados no HTML de entrada são descartados.</span><span class="sxs-lookup"><span data-stu-id="e159e-140">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="e159e-141">body</span><span class="sxs-lookup"><span data-stu-id="e159e-141">body</span></span> | <span data-ttu-id="e159e-142">A palavra-chave que tem como destino o primeiro div na página.</span><span class="sxs-lookup"><span data-stu-id="e159e-142">The keyword that targets the first div on the page.</span></span> <span data-ttu-id="e159e-143">Não use # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="e159e-143">Do not prefix with a #.</span></span> |  
| <span data-ttu-id="e159e-144">title</span><span class="sxs-lookup"><span data-stu-id="e159e-144">title</span></span> | <span data-ttu-id="e159e-145">A palavra-chave que tem como destino o título da página.</span><span class="sxs-lookup"><span data-stu-id="e159e-145">The keyword that targets the page title.</span></span> <span data-ttu-id="e159e-146">Não use # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="e159e-146">Do not prefix with a #.</span></span> |  
 
#### <a name="action"></a><span data-ttu-id="e159e-147">action</span><span class="sxs-lookup"><span data-stu-id="e159e-147">action</span></span>

<span data-ttu-id="e159e-148">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-148">The action to perform on the target element.</span></span> <span data-ttu-id="e159e-149">Veja as [ações com suporte para elementos](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="e159e-149">See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="e159e-150">Ação</span><span class="sxs-lookup"><span data-stu-id="e159e-150">Action</span></span> | <span data-ttu-id="e159e-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="e159e-151">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e159e-152">append</span><span class="sxs-lookup"><span data-stu-id="e159e-152">append</span></span> | <p><span data-ttu-id="e159e-153">Adiciona o conteúdo fornecido ao destino como primeiro ou último filho, conforme determinado pelo atributo **position**.</span><span class="sxs-lookup"><span data-stu-id="e159e-153">Adds the supplied content to the target as a first or last child, as determined by the **position** attribute.</span></span></p><p><span data-ttu-id="e159e-154">Aplicável somente a elementos **body**, **div**, **ol** e **ul**.</span><span class="sxs-lookup"><span data-stu-id="e159e-154">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="e159e-155">insert</span><span class="sxs-lookup"><span data-stu-id="e159e-155">insert</span></span> | <span data-ttu-id="e159e-156">Adiciona o conteúdo fornecido como irmão antes ou depois do destino, conforme determinado pelo atributo **position**.</span><span class="sxs-lookup"><span data-stu-id="e159e-156">Adds the supplied content as a sibling before or after the target, as determined by the **position** attribute.</span></span> |  
| <span data-ttu-id="e159e-157">prepend</span><span class="sxs-lookup"><span data-stu-id="e159e-157">prepend</span></span> | <p><span data-ttu-id="e159e-158">Adiciona o conteúdo fornecido ao destino como um primeiro filho.</span><span class="sxs-lookup"><span data-stu-id="e159e-158">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="e159e-159">Atalho para **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="e159e-159">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="e159e-160">Aplicável somente a elementos **body**, **div**, **ol** e **ul**.</span><span class="sxs-lookup"><span data-stu-id="e159e-160">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="e159e-161">replace</span><span class="sxs-lookup"><span data-stu-id="e159e-161">replace</span></span> | <p><span data-ttu-id="e159e-162">Substitui o destino pelo conteúdo fornecido.</span><span class="sxs-lookup"><span data-stu-id="e159e-162">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="e159e-163">A maioria das ações **replace** exige o uso de [ID gerada](#generated-ids) para o destino (exceto os elementos **img** e **object** em um div, que também é compatível com o uso de **data-id**).</span><span class="sxs-lookup"><span data-stu-id="e159e-163">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
#### <a name="position"></a><span data-ttu-id="e159e-164">position</span><span class="sxs-lookup"><span data-stu-id="e159e-164">position</span></span>

<span data-ttu-id="e159e-165">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-165">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="e159e-166">Usa o padrão **after** caso seja omitido.</span><span class="sxs-lookup"><span data-stu-id="e159e-166">Defaults to **after** if omitted.</span></span>

| <span data-ttu-id="e159e-167">Posição</span><span class="sxs-lookup"><span data-stu-id="e159e-167">Position</span></span> | <span data-ttu-id="e159e-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="e159e-168">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e159e-169">after (padrão)</span><span class="sxs-lookup"><span data-stu-id="e159e-169">after (default)</span></span> |<p><span data-ttu-id="e159e-170">Com **append**: último filho do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-170">- With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="e159e-171">Com **insert**: o irmão subsequente do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-171">- With **insert**: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="e159e-172">before</span><span class="sxs-lookup"><span data-stu-id="e159e-172">before</span></span> | <p><span data-ttu-id="e159e-173">Com **append**: primeiro filho do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-173">- With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="e159e-174">Com **insert**: o irmão precedente do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-174">- With **insert**: The preceding sibling of the target element.</span></span></p> |

#### <a name="content"></a><span data-ttu-id="e159e-175">content</span><span class="sxs-lookup"><span data-stu-id="e159e-175">content</span></span>

<span data-ttu-id="e159e-176">Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="e159e-176">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="e159e-177">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o tipo de conteúdo `multipart/form-data` com uma parte "Commands" (veja um [exemplo](#multipart-request-with-binary-content).)</span><span class="sxs-lookup"><span data-stu-id="e159e-177">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part (see an [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="e159e-178">IDs geradas</span><span class="sxs-lookup"><span data-stu-id="e159e-178">Generated IDs</span></span>
<span data-ttu-id="e159e-179">O Microsoft Graph gera valores de **id** para que os elementos na página possam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e159e-179">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="e159e-180">Para obter as IDs geradas, use a expressão de cadeia de caracteres de consulta `includeIDs=true` na sua solicitação GET:</span><span class="sxs-lookup"><span data-stu-id="e159e-180">To get generated IDs, use the `includeIDs=true` query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="e159e-181">**Observação:** a API descarta todos os valores de **id** na [HTML de entrada](onenote_input_output_html.md) das solicitações de criar página e atualizar página.</span><span class="sxs-lookup"><span data-stu-id="e159e-181">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote_input_output_html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="e159e-182">O exemplo a seguir mostra IDs geradas para um parágrafo e uma imagem no [HTML de saída](onenote_input_output_html.md) de uma página.</span><span class="sxs-lookup"><span data-stu-id="e159e-182">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote_input_output_html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="e159e-183">Os valores de **id** gerados podem ser alterados após uma atualização de página. Então você deve obter valores atuais antes de criar uma solicitação de PATCH que usa esses valores.</span><span class="sxs-lookup"><span data-stu-id="e159e-183">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="e159e-184">Você pode especificar elementos de destino usando os valores **data-id** ou **id** seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="e159e-184">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="e159e-185">Para as ações **append** e **insert**, você pode usar o ID como o valor de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-185">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="e159e-186">Para as ações **replace**, use o ID gerado para todos os elementos, exceto o título da página e imagens e objetos que estejam dentro de um div.</span><span class="sxs-lookup"><span data-stu-id="e159e-186">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div.</span></span> 
    - <span data-ttu-id="e159e-187">Para substituir um título, use a palavra-chave **título**.</span><span class="sxs-lookup"><span data-stu-id="e159e-187">To replace a title, use the **title** keyword.</span></span> 
    - <span data-ttu-id="e159e-188">Para substituir imagens e objetos que estejam dentro de um div, use **data-id** ou **id**.</span><span class="sxs-lookup"><span data-stu-id="e159e-188">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="e159e-189">O exemplo a seguir usa o valor **id** para o destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-189">The following example uses the **id** value for the target.</span></span> <span data-ttu-id="e159e-190">Não use o prefixo # com um ID gerado.</span><span class="sxs-lookup"><span data-stu-id="e159e-190">Don't use the # prefix with a generated ID.</span></span>

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a><span data-ttu-id="e159e-191">Elementos e ações compatíveis</span><span class="sxs-lookup"><span data-stu-id="e159e-191">Supported elements and actions</span></span>

<span data-ttu-id="e159e-192">Muitos elementos na página podem ser atualizados, mas cada tipo de elemento é compatível com ações específicas.</span><span class="sxs-lookup"><span data-stu-id="e159e-192">Many elements on the page can be updated, but each element type supports specific actions.</span></span> <span data-ttu-id="e159e-193">A tabela a seguir mostra os elementos de destino compatíveis com as ações de atualização a que eles dão suporte.</span><span class="sxs-lookup"><span data-stu-id="e159e-193">The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="e159e-194">Elemento</span><span class="sxs-lookup"><span data-stu-id="e159e-194">Element</span></span> | <span data-ttu-id="e159e-195">Substituir</span><span class="sxs-lookup"><span data-stu-id="e159e-195">Replace</span></span> | <span data-ttu-id="e159e-196">Anexar filho</span><span class="sxs-lookup"><span data-stu-id="e159e-196">Append child</span></span> | <span data-ttu-id="e159e-197">Inserir irmão</span><span class="sxs-lookup"><span data-stu-id="e159e-197">Insert sibling</span></span> |  
|------|:------:|:------:|:------:|  
| <span data-ttu-id="e159e-198">body</span><span class="sxs-lookup"><span data-stu-id="e159e-198">body</span></span><br /> <span data-ttu-id="e159e-199">(tem como destino o primeiro div na página)</span><span class="sxs-lookup"><span data-stu-id="e159e-199">(targets first div on the page)</span></span> | <span data-ttu-id="e159e-200">não</span><span class="sxs-lookup"><span data-stu-id="e159e-200">no</span></span> | <span data-ttu-id="e159e-201">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-201">**yes**</span></span> | <span data-ttu-id="e159e-202">não</span><span class="sxs-lookup"><span data-stu-id="e159e-202">no</span></span> |  
| <span data-ttu-id="e159e-203">div</span><span class="sxs-lookup"><span data-stu-id="e159e-203">div</span></span><br /> <span data-ttu-id="e159e-204">([absoluto posicionado](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="e159e-204">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="e159e-205">não</span><span class="sxs-lookup"><span data-stu-id="e159e-205">no</span></span> | <span data-ttu-id="e159e-206">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-206">**yes**</span></span> | <span data-ttu-id="e159e-207">não</span><span class="sxs-lookup"><span data-stu-id="e159e-207">no</span></span> |  
| <span data-ttu-id="e159e-208">div</span><span class="sxs-lookup"><span data-stu-id="e159e-208">div</span></span><br /> <span data-ttu-id="e159e-209">(em um div)</span><span class="sxs-lookup"><span data-stu-id="e159e-209">(within a div)</span></span> | <span data-ttu-id="e159e-210">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-210">**yes**</span></span><br/><span data-ttu-id="e159e-211">(somente id)</span><span class="sxs-lookup"><span data-stu-id="e159e-211">yes (id only)</span></span> | <span data-ttu-id="e159e-212">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-212">**yes**</span></span> | <span data-ttu-id="e159e-213">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-213">**yes**</span></span> |   
| <span data-ttu-id="e159e-214">img, object</span><span class="sxs-lookup"><span data-stu-id="e159e-214">img, object</span></span><br /> <span data-ttu-id="e159e-215">(em um div)</span><span class="sxs-lookup"><span data-stu-id="e159e-215">(within a div)</span></span> | <span data-ttu-id="e159e-216">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-216">**yes**</span></span> | <span data-ttu-id="e159e-217">não</span><span class="sxs-lookup"><span data-stu-id="e159e-217">no</span></span> | <span data-ttu-id="e159e-218">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-218">**yes**</span></span> |   
| <span data-ttu-id="e159e-219">ol, ul</span><span class="sxs-lookup"><span data-stu-id="e159e-219">ol, ul</span></span> | <span data-ttu-id="e159e-220">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-220">**yes**</span></span><br/><span data-ttu-id="e159e-221">(somente id)</span><span class="sxs-lookup"><span data-stu-id="e159e-221">yes (id only)</span></span> | <span data-ttu-id="e159e-222">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-222">**yes**</span></span> | <span data-ttu-id="e159e-223">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-223">**yes**</span></span> |   
| <span data-ttu-id="e159e-224">table</span><span class="sxs-lookup"><span data-stu-id="e159e-224">table</span></span> | <span data-ttu-id="e159e-225">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-225">**yes**</span></span><br/><span data-ttu-id="e159e-226">(somente id)</span><span class="sxs-lookup"><span data-stu-id="e159e-226">yes (id only)</span></span> | <span data-ttu-id="e159e-227">não</span><span class="sxs-lookup"><span data-stu-id="e159e-227">no</span></span> | <span data-ttu-id="e159e-228">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-228">**yes**</span></span> |   
| <span data-ttu-id="e159e-229">p, li, h1-h6</span><span class="sxs-lookup"><span data-stu-id="e159e-229">p, li, h1-h6</span></span> | <span data-ttu-id="e159e-230">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-230">**yes**</span></span><br/><span data-ttu-id="e159e-231">(somente id)</span><span class="sxs-lookup"><span data-stu-id="e159e-231">yes (id only)</span></span> | <span data-ttu-id="e159e-232">não</span><span class="sxs-lookup"><span data-stu-id="e159e-232">no</span></span> | <span data-ttu-id="e159e-233">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-233">**yes**</span></span> |   
| <span data-ttu-id="e159e-234">title</span><span class="sxs-lookup"><span data-stu-id="e159e-234">title</span></span> | <span data-ttu-id="e159e-235">**sim**</span><span class="sxs-lookup"><span data-stu-id="e159e-235">**yes**</span></span> | <span data-ttu-id="e159e-236">não</span><span class="sxs-lookup"><span data-stu-id="e159e-236">no</span></span> | <span data-ttu-id="e159e-237">não</span><span class="sxs-lookup"><span data-stu-id="e159e-237">no</span></span> |  
 
<br/>

<span data-ttu-id="e159e-238">Os seguintes elementos não dão suporte a nenhuma ação de atualização.</span><span class="sxs-lookup"><span data-stu-id="e159e-238">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="e159e-239">img ([absoluto posicionado](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="e159e-239">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="e159e-240">object ([absoluto posicionado](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="e159e-240">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="e159e-241">tr, td</span><span class="sxs-lookup"><span data-stu-id="e159e-241">tr, td</span></span>
- <span data-ttu-id="e159e-242">meta</span><span class="sxs-lookup"><span data-stu-id="e159e-242">meta</span></span>
- <span data-ttu-id="e159e-243">head</span><span class="sxs-lookup"><span data-stu-id="e159e-243">head</span></span>
- <span data-ttu-id="e159e-244">span</span><span class="sxs-lookup"><span data-stu-id="e159e-244">span</span></span>
- <span data-ttu-id="e159e-245">a</span><span class="sxs-lookup"><span data-stu-id="e159e-245">a</span></span>
- <span data-ttu-id="e159e-246">style tags</span><span class="sxs-lookup"><span data-stu-id="e159e-246">style tags</span></span>


<a name="examples"></a>

## <a name="example-requests"></a><span data-ttu-id="e159e-247">Solicitações de exemplo</span><span class="sxs-lookup"><span data-stu-id="e159e-247">Example requests</span></span>

<span data-ttu-id="e159e-248">Uma solicitação de atualização contém um ou mais alterações representadas como objetos de alteração JSON.</span><span class="sxs-lookup"><span data-stu-id="e159e-248">An update request contains one or more changes represented as JSON change objects.</span></span> <span data-ttu-id="e159e-249">Esses objetos podem definir destinos diferentes na página e outras ações e conteúdos diferentes para os destinos.</span><span class="sxs-lookup"><span data-stu-id="e159e-249">These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="e159e-250">Os exemplos a seguir contêm objetos JSON usados em solicitações de PATCH e solicitações de PATCH completo:</span><span class="sxs-lookup"><span data-stu-id="e159e-250">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

- [<span data-ttu-id="e159e-251">Acrescentar elementos filho</span><span class="sxs-lookup"><span data-stu-id="e159e-251">Append child elements</span></span>](#append-child-elements)
- [<span data-ttu-id="e159e-252">Inserir elementos irmãos</span><span class="sxs-lookup"><span data-stu-id="e159e-252">Insert sibling elements</span></span>](#insert-sibling-elements)
- [<span data-ttu-id="e159e-253">Substituir elementos</span><span class="sxs-lookup"><span data-stu-id="e159e-253">Replace elements</span></span>](#replace-elements)
- [<span data-ttu-id="e159e-254">Solicitações de PATCH completo</span><span class="sxs-lookup"><span data-stu-id="e159e-254">Complete PATCH requests</span></span>](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="e159e-255">Acrescentar elementos filho</span><span class="sxs-lookup"><span data-stu-id="e159e-255">Append child elements</span></span>

<span data-ttu-id="e159e-256">A ação **append** adiciona um filho a um elemento **body**, **div** (dentro de um div), **ol** ou **ul**.</span><span class="sxs-lookup"><span data-stu-id="e159e-256">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element.</span></span> <span data-ttu-id="e159e-257">O atributo **position** determina se deve acrescentar o filho antes ou depois do destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-257">The **position** attribute determines whether to append the child before or after the target.</span></span> <span data-ttu-id="e159e-258">A posição padrão é **after**.</span><span class="sxs-lookup"><span data-stu-id="e159e-258">The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="e159e-259">Acrescentar a um div</span><span class="sxs-lookup"><span data-stu-id="e159e-259">Append to a div</span></span>

<span data-ttu-id="e159e-260">O exemplo a seguir adiciona dois nós filho ao elemento **div1**.</span><span class="sxs-lookup"><span data-stu-id="e159e-260">The following example adds two child nodes to the **div1** element.</span></span> <span data-ttu-id="e159e-261">Ele adiciona uma imagem como primeiro filho e um parágrafo como último filho.</span><span class="sxs-lookup"><span data-stu-id="e159e-261">It adds an image as the first child and a paragraph as the last child.</span></span> 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="e159e-262">Acrescentar ao elemento *body*</span><span class="sxs-lookup"><span data-stu-id="e159e-262">Append to the *body* element</span></span>

<span data-ttu-id="e159e-263">Você pode usar o atalho **body** para acrescentar um elemento filho dentro o primeiro div em qualquer página.</span><span class="sxs-lookup"><span data-stu-id="e159e-263">You can use the **body** shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="e159e-264">O exemplo a seguir adiciona dois parágrafos como primeiro filho e último filho ao primeiro div na página.</span><span class="sxs-lookup"><span data-stu-id="e159e-264">The following example adds two paragraphs as the first child and the last child to the first div on the page.</span></span> <span data-ttu-id="e159e-265">Não use # com o destino **body**.</span><span class="sxs-lookup"><span data-stu-id="e159e-265">Don't use a # with the **body** target.</span></span> <span data-ttu-id="e159e-266">Este exemplo usa a ação **prepend** como um atalho para **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="e159e-266">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a><span data-ttu-id="e159e-267">Acrescentar a uma lista</span><span class="sxs-lookup"><span data-stu-id="e159e-267">Append to a list</span></span>

<span data-ttu-id="e159e-268">O exemplo a seguir adiciona um item de lista como um último filho à lista de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-268">The following example adds a list item as a last child to the target list.</span></span> <span data-ttu-id="e159e-269">A propriedade **list-style-type** é definida porque o item usa um estilo de lista não padrão.</span><span class="sxs-lookup"><span data-stu-id="e159e-269">The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a><span data-ttu-id="e159e-270">Inserir elementos irmãos</span><span class="sxs-lookup"><span data-stu-id="e159e-270">Insert sibling elements</span></span>

<span data-ttu-id="e159e-271">A ação **insert** adiciona irmão a um elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-271">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="e159e-272">O atributo **position** determina se deve inserir o irmão antes ou depois do destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-272">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="e159e-273">A posição padrão é **after**.</span><span class="sxs-lookup"><span data-stu-id="e159e-273">The default position is **after**.</span></span> <span data-ttu-id="e159e-274">Ver [elementos compatíveis com **insert**](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="e159e-274">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

#### <a name="insert-siblings"></a><span data-ttu-id="e159e-275">Inserir irmãos</span><span class="sxs-lookup"><span data-stu-id="e159e-275">Insert siblings</span></span>

<span data-ttu-id="e159e-276">O exemplo a seguir adiciona dois nós irmãos à página.</span><span class="sxs-lookup"><span data-stu-id="e159e-276">The following example adds two sibling nodes to the page.</span></span> <span data-ttu-id="e159e-277">Adiciona uma imagem acima do elemento **para1** elemento e um parágrafo abaixo do elemento **para2**.</span><span class="sxs-lookup"><span data-stu-id="e159e-277">It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a><span data-ttu-id="e159e-278">Substituir elementos</span><span class="sxs-lookup"><span data-stu-id="e159e-278">Replace elements</span></span>

<span data-ttu-id="e159e-279">Você pode usar **data-id** ou **id** gerado como o valor de destino para substituir os elementos **img** e **object** que estão em um div.</span><span class="sxs-lookup"><span data-stu-id="e159e-279">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div.</span></span> <span data-ttu-id="e159e-280">Para substituir um título de página, use a palavra-chave **title**.</span><span class="sxs-lookup"><span data-stu-id="e159e-280">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="e159e-281">Para todos os outros [elementos compatíveis com **replace**](#supported-elements-and-actions), você deve usar o ID gerado.</span><span class="sxs-lookup"><span data-stu-id="e159e-281">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="e159e-282">Substituir uma imagem</span><span class="sxs-lookup"><span data-stu-id="e159e-282">Replace an image</span></span>

<span data-ttu-id="e159e-283">O exemplo a seguir substitui uma imagem por um div usando a **data-id** da imagem como destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-283">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="e159e-284">Atualizar um tabela</span><span class="sxs-lookup"><span data-stu-id="e159e-284">Update a table</span></span> 

<span data-ttu-id="e159e-285">Este exemplo mostra como atualizar uma tabela usando seu ID gerado.</span><span class="sxs-lookup"><span data-stu-id="e159e-285">This example shows how to update a table by using its generated ID.</span></span> <span data-ttu-id="e159e-286">A substituição dos elementos **tr** e **td** não tem suporte, mas você pode substituir a tabela inteira.</span><span class="sxs-lookup"><span data-stu-id="e159e-286">Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a><span data-ttu-id="e159e-287">Alterar o título</span><span class="sxs-lookup"><span data-stu-id="e159e-287">Change the title</span></span> 

<span data-ttu-id="e159e-288">Este exemplo mostra como alterar o título da página.</span><span class="sxs-lookup"><span data-stu-id="e159e-288">This example shows how to change the title of a page.</span></span> <span data-ttu-id="e159e-289">Para alterar o título, use a palavra-chave **title** como o valor de destino.</span><span class="sxs-lookup"><span data-stu-id="e159e-289">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="e159e-290">Não use # com o destino de título.</span><span class="sxs-lookup"><span data-stu-id="e159e-290">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="e159e-291">Atualizar um item pendente</span><span class="sxs-lookup"><span data-stu-id="e159e-291">Update a to-do item</span></span>

<span data-ttu-id="e159e-292">O exemplo a seguir usa a ação de substituir para alterar um item de caixa de seleção pendente para um estado concluído.</span><span class="sxs-lookup"><span data-stu-id="e159e-292">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="e159e-293">Veja [Usar marcas de anotação](onenote-note-tags.md) para saber mais sobre como usar o atributo **data-tag**.</span><span class="sxs-lookup"><span data-stu-id="e159e-293">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="e159e-294">Exemplos de solicitação de PATCH completo</span><span class="sxs-lookup"><span data-stu-id="e159e-294">Complete PATCH request examples</span></span>

<span data-ttu-id="e159e-295">Os exemplos a seguir mostram solicitações de PATCH completo.</span><span class="sxs-lookup"><span data-stu-id="e159e-295">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="e159e-296">Solicitar apenas com conteúdo de texto</span><span class="sxs-lookup"><span data-stu-id="e159e-296">Request with text content only</span></span>

<span data-ttu-id="e159e-297">O exemplo a seguir mostra uma solicitação de PATCH que usa o tipo de conteúdo **application/json**.</span><span class="sxs-lookup"><span data-stu-id="e159e-297">The following example shows a PATCH request that uses the **application/json** content type.</span></span> <span data-ttu-id="e159e-298">Você pode usar esse formato quando seu conteúdo não contém dados binários.</span><span class="sxs-lookup"><span data-stu-id="e159e-298">You can use this format when your content doesn't contain binary data.</span></span>

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="e159e-299">Solicitação de partes múltiplas com conteúdo binário</span><span class="sxs-lookup"><span data-stu-id="e159e-299">Multipart request with binary content</span></span> 

<span data-ttu-id="e159e-300">O exemplo a seguir mostra uma solicitação de PATCH de diversas partes que inclui dados binários.</span><span class="sxs-lookup"><span data-stu-id="e159e-300">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="e159e-301">As solicitações de diversas partes exigem uma parte de "Comandos" que especifica o tipo de conteúdo **application/json** e contém a matriz de objetos de alteração JSON.</span><span class="sxs-lookup"><span data-stu-id="e159e-301">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="e159e-302">Outras partes de dados podem conter dados binários.</span><span class="sxs-lookup"><span data-stu-id="e159e-302">Other data parts can contain binary data.</span></span> <span data-ttu-id="e159e-303">Os nomes de partes são geralmente cadeias de caracteres acrescentadas com a hora atual em milissegundos ou um GUID aleatório.</span><span class="sxs-lookup"><span data-stu-id="e159e-303">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="e159e-304">Informações de solicitação e resposta para solicitações de PATCH</span><span class="sxs-lookup"><span data-stu-id="e159e-304">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="e159e-305">Dados da solicitação</span><span class="sxs-lookup"><span data-stu-id="e159e-305">Request data</span></span> | <span data-ttu-id="e159e-306">Descrição</span><span class="sxs-lookup"><span data-stu-id="e159e-306">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e159e-307">Protocolo</span><span class="sxs-lookup"><span data-stu-id="e159e-307">Protocol</span></span> | <span data-ttu-id="e159e-308">Todas as solicitações usam o protocolo HTTPS de SSL/TLS.</span><span class="sxs-lookup"><span data-stu-id="e159e-308">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="e159e-309">Cabeçalho de autorização</span><span class="sxs-lookup"><span data-stu-id="e159e-309">Authorization header</span></span> | <p><span data-ttu-id="e159e-310">`Bearer {token}`, onde `{token}` é um token de acesso do OAuth 2.0 válido para o aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="e159e-310">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="e159e-311">Se ele estiver ausente ou for inválido, a solicitação falhará com um código de status 401.</span><span class="sxs-lookup"><span data-stu-id="e159e-311">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="e159e-312">Confira [Autenticação e permissões](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e159e-312">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="e159e-313">Cabeçalho content-type</span><span class="sxs-lookup"><span data-stu-id="e159e-313">Content-Type header</span></span> | <p><span data-ttu-id="e159e-314">`application/json` para a matriz de objetos de alteração JSON, seja enviado diretamente no corpo da mensagem, seja na parte "Comandos" obrigatória de [solicitações de diversas partes](#multipart-request-with-binary-content).</span><span class="sxs-lookup"><span data-stu-id="e159e-314">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="e159e-315">As solicitações de diversas partes são necessárias quando se enviam dados binários e usam o tipo de conteúdo `multipart/form-data; boundary=part-boundary`, onde `{part-boundary}` é uma cadeia de caracteres que sinaliza o início e o término de cada parte de dados.</span><span class="sxs-lookup"><span data-stu-id="e159e-315">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  

<br/> 

| <span data-ttu-id="e159e-316">Dados de resposta</span><span class="sxs-lookup"><span data-stu-id="e159e-316">Response data</span></span> | <span data-ttu-id="e159e-317">Descrição</span><span class="sxs-lookup"><span data-stu-id="e159e-317">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e159e-318">Código de êxito</span><span class="sxs-lookup"><span data-stu-id="e159e-318">Success code</span></span> | <span data-ttu-id="e159e-319">Um código de status de HTTP 204.</span><span class="sxs-lookup"><span data-stu-id="e159e-319">A 204 HTTP status code.</span></span> <span data-ttu-id="e159e-320">Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="e159e-320">No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="e159e-321">Erros</span><span class="sxs-lookup"><span data-stu-id="e159e-321">Errors</span></span> | <span data-ttu-id="e159e-322">Leia [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote_error_codes.md) para saber mais sobre erros do OneNote que poderão ser retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e159e-322">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="e159e-323">Criar a URL raiz do serviço do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e159e-323">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="e159e-324">A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para o OneNote:</span><span class="sxs-lookup"><span data-stu-id="e159e-324">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="e159e-325">O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="e159e-325">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="e159e-326">`v1.0` serve para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="e159e-326">`v1.0` is for stable production code.</span></span> <span data-ttu-id="e159e-327">`beta` serve para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="e159e-327">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="e159e-328">Os recursos e a funcionalidade na versão beta podem mudar, por isso, você não deve usá-la no código de produção.</span><span class="sxs-lookup"><span data-stu-id="e159e-328">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>

<span data-ttu-id="e159e-329">`me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="e159e-329">`me` is for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="e159e-330">`users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="e159e-330">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="e159e-331">Use a [API do Microsoft Azure AD Graph](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="e159e-331">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span></span>


> <span data-ttu-id="e159e-332">**Observação:** para obter as ids de usuário, faça uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="e159e-332">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="e159e-333">Permissões</span><span class="sxs-lookup"><span data-stu-id="e159e-333">Permissions</span></span>

<span data-ttu-id="e159e-334">Para atualizar páginas do OneNote, solicite as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="e159e-334">To update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="e159e-335">Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="e159e-335">Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="e159e-336">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e159e-336">Notes.ReadWrite</span></span>
- <span data-ttu-id="e159e-337">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e159e-337">Notes.ReadWrite.All</span></span>

<span data-ttu-id="e159e-338">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e159e-338">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="e159e-339">Confira também</span><span class="sxs-lookup"><span data-stu-id="e159e-339">See also</span></span>

- [<span data-ttu-id="e159e-340">Adicionar imagens e arquivos</span><span class="sxs-lookup"><span data-stu-id="e159e-340">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="e159e-341">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="e159e-341">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="e159e-342">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="e159e-342">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="e159e-343">Perguntas sobre desenvolvimento do OneNote no Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="e159e-343">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="e159e-344">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="e159e-344">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
