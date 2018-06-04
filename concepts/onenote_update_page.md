# <a name="update-onenote-page-content"></a><span data-ttu-id="4ef95-101">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="4ef95-101">Update OneNote page content</span></span>

<span data-ttu-id="4ef95-102">*__Aplica-se a:__ Bloco de anotações dos consumidores no OneDrive | Bloco de anotações empresariais no Office 365*</span><span class="sxs-lookup"><span data-stu-id="4ef95-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>


<span data-ttu-id="4ef95-103">Para atualizar o conteúdo de uma página do OneNote, envie uma solicitação de PATCH para o ponto de extremidade do *conteúdo* da página:</span><span class="sxs-lookup"><span data-stu-id="4ef95-103">To update the content of a OneNote page, you send a PATCH request to the page's *content* endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="4ef95-104">Envie um objeto de alteração JSON no corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="4ef95-104">Send a JSON change object in the message body.</span></span> <span data-ttu-id="4ef95-105">Se a solicitação for bem-sucedida, o Microsoft Graph retorna um código de status de HTTP 204.</span><span class="sxs-lookup"><span data-stu-id="4ef95-105">If the request is successful, the Microsoft Graph returns a 204 HTTP status code.</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="4ef95-106">Construir a URI de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ef95-106">Construct the request</span></span>

<span data-ttu-id="4ef95-107">Para construir a URI de solicitação, comece com a URL raiz do serviço:</span><span class="sxs-lookup"><span data-stu-id="4ef95-107">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="4ef95-108">Acrescente então o ponto de extremidade do *conteúdo* da página:</span><span class="sxs-lookup"><span data-stu-id="4ef95-108">Then append the page's *content* endpoint:</span></span>

<span data-ttu-id="4ef95-109">**Obter o HTML da página e todos os valores de *data-id* definidos**</span><span class="sxs-lookup"><span data-stu-id="4ef95-109">**Get the page HTML and all defined *data-id* values**</span></span></p>
`../pages/{id}/content`   

<span data-ttu-id="4ef95-110">**Obter o HTML da página, todos os valores de *data-id* definidos e todos os valores de *id* gerados**</span><span class="sxs-lookup"><span data-stu-id="4ef95-110">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span>  
`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="4ef95-111">A **data-id** e os valores de **id** são usados como identificadores de **destino** para elementos que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="4ef95-111">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="4ef95-112">Sua solicitação de URI completa terá a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="4ef95-112">Your full request URI will look like this:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="4ef95-113">Saiba mais sobre a [URL raiz de serviço](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="4ef95-113">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>


<a name="message-body"></a>
## <a name="construct-the-message-body"></a><span data-ttu-id="4ef95-114">Criar o corpo da mensagem</span><span class="sxs-lookup"><span data-stu-id="4ef95-114">Construct the message body</span></span>

<span data-ttu-id="4ef95-115">O HTML de uma página do OneNote contém texto, imagens e outros conteúdos organizados em estruturas como elementos **div**, **img** e **ol**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-115">The HTML of a OneNote page contains text, images, and other content organized into structures such as **div**, **img**, and **ol** elements.</span></span> <span data-ttu-id="4ef95-116">Para atualizar o conteúdo da página do OneNote, adicione e substitua elementos HTML na página.</span><span class="sxs-lookup"><span data-stu-id="4ef95-116">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="4ef95-117">Suas alterações serão enviadas no corpo da mensagem como uma matriz de objetos de alteração JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef95-117">Your changes are sent in the message body as an array of JSON change objects.</span></span> <span data-ttu-id="4ef95-118">Cada objeto especifica o elemento de destino, o novo conteúdo HTML e o que fazer com o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4ef95-118">Each object specifies the target element, new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="4ef95-119">A matriz a seguir define duas alterações.</span><span class="sxs-lookup"><span data-stu-id="4ef95-119">The following array defines two changes.</span></span> <span data-ttu-id="4ef95-120">A primeira insere uma imagem acima de um parágrafo como um irmão, e a segunda acrescenta um item em uma lista como um último filho.</span><span class="sxs-lookup"><span data-stu-id="4ef95-120">The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

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

<span data-ttu-id="4ef95-121">Veja [mais exemplos](#example-requests).</span><span class="sxs-lookup"><span data-stu-id="4ef95-121">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="4ef95-122">Atributos de objetos de alteração JSON</span><span class="sxs-lookup"><span data-stu-id="4ef95-122">Attributes for JSON change objects</span></span>

<span data-ttu-id="4ef95-123">Use atributos **target**, **action**, **position** e **content** para definir objetos JSON para solicitações de PATCH.</span><span class="sxs-lookup"><span data-stu-id="4ef95-123">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

<span data-ttu-id="4ef95-124">**target**</span><span class="sxs-lookup"><span data-stu-id="4ef95-124">**target**</span></span>  
<span data-ttu-id="4ef95-125">O elemento a atualizar.</span><span class="sxs-lookup"><span data-stu-id="4ef95-125">The element to update.</span></span> <span data-ttu-id="4ef95-126">O valor deve ser uma dos seguintes identificadores:</span><span class="sxs-lookup"><span data-stu-id="4ef95-126">The value must be one of the following:</span></span>

| <span data-ttu-id="4ef95-127">Identificador</span><span class="sxs-lookup"><span data-stu-id="4ef95-127">identifier</span></span> | <span data-ttu-id="4ef95-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ef95-128">Description</span></span> |  
|------|------|  
| <span data-ttu-id="4ef95-129">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="4ef95-129">data-id</span></span> | <p><span data-ttu-id="4ef95-130">Essa ID é opcionalmente definida em elementos na HTML de entrada ao [criar uma página](onenote-create-page.md) ou [atualizar uma página](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="4ef95-130">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote_update_page.md).</span></span> <span data-ttu-id="4ef95-131">Coloque um # como prefixo do valor.</span><span class="sxs-lookup"><span data-stu-id="4ef95-131">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="4ef95-132">Exemplo: `'target':'#intro'` tem como destino o elemento `<div data-id="intro" ...>`</span><span class="sxs-lookup"><span data-stu-id="4ef95-132">Example: `'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="4ef95-133">id</span><span class="sxs-lookup"><span data-stu-id="4ef95-133">id</span></span> | <p><span data-ttu-id="4ef95-134">É a [ID gerada](#generated-ids) do Microsoft Graph e é necessário para a maioria das operações de substituição.</span><span class="sxs-lookup"><span data-stu-id="4ef95-134">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="4ef95-135">Não use # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="4ef95-135">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="4ef95-136">Exemplo: `'target':'div:{33f8a2...}{37}'` tem como destino o elemento `<div id="div:{33f8a2...}{37}" ...>`</span><span class="sxs-lookup"><span data-stu-id="4ef95-136">Example: `'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="4ef95-137">Não confunda esses identificadores com valores de **id** definidos no [HTML de entrada](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="4ef95-137">Don't confuse these with any **id** values defined in the [input HTML](onenote_input_output_html.md).</span></span> <span data-ttu-id="4ef95-138">Todos os valores de **id** enviados no HTML de entrada são descartados.</span><span class="sxs-lookup"><span data-stu-id="4ef95-138">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="4ef95-139">body</span><span class="sxs-lookup"><span data-stu-id="4ef95-139">body</span></span> | <span data-ttu-id="4ef95-140">A palavra-chave que tem como destino o primeiro div na página.</span><span class="sxs-lookup"><span data-stu-id="4ef95-140">The keyword that targets the first div on the page.</span></span> <span data-ttu-id="4ef95-141">Não use # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="4ef95-141">Do not prefix with a #.</span></span> |  
| <span data-ttu-id="4ef95-142">title</span><span class="sxs-lookup"><span data-stu-id="4ef95-142">title</span></span> | <span data-ttu-id="4ef95-143">A palavra-chave que tem como destino o título da página.</span><span class="sxs-lookup"><span data-stu-id="4ef95-143">The keyword that targets the page title.</span></span> <span data-ttu-id="4ef95-144">Não use # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="4ef95-144">Do not prefix with a #.</span></span> |  
 
<span data-ttu-id="4ef95-145">**action**</span><span class="sxs-lookup"><span data-stu-id="4ef95-145">**action**</span></span>  
<span data-ttu-id="4ef95-146">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-146">The action to perform on the target element. Possible values are: , , , , or .</span></span> <span data-ttu-id="4ef95-147">Veja as [ações com suporte para elementos](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="4ef95-147">See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="4ef95-148">Ação</span><span class="sxs-lookup"><span data-stu-id="4ef95-148">Action</span></span> | <span data-ttu-id="4ef95-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ef95-149">Description</span></span> |  
|------|------|  
| <span data-ttu-id="4ef95-150">append</span><span class="sxs-lookup"><span data-stu-id="4ef95-150">Append</span></span> | <p><span data-ttu-id="4ef95-151">Adiciona o conteúdo fornecido ao destino como primeiro ou último filho, conforme determinado pelo atributo **position**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-151">Adds the supplied content to the target as a first or last child, as determined by the **position** attribute.</span></span></p><p><span data-ttu-id="4ef95-152">Aplicável somente a elementos **body**, **div**, **ol** e **ul**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-152">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="4ef95-153">insert</span><span class="sxs-lookup"><span data-stu-id="4ef95-153">Insert</span></span> | <span data-ttu-id="4ef95-154">Adiciona o conteúdo fornecido como irmão antes ou depois do destino, conforme determinado pelo atributo **position**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-154">Adds the supplied content as a sibling before or after the target, as determined by the **position** attribute.</span></span> |  
| <span data-ttu-id="4ef95-155">prepend</span><span class="sxs-lookup"><span data-stu-id="4ef95-155">prepend</span></span> | <p><span data-ttu-id="4ef95-156">Adiciona o conteúdo fornecido ao destino como um primeiro filho.</span><span class="sxs-lookup"><span data-stu-id="4ef95-156">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="4ef95-157">Atalho para **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-157">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="4ef95-158">Aplicável somente a elementos **body**, **div**, **ol** e **ul**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-158">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="4ef95-159">replace</span><span class="sxs-lookup"><span data-stu-id="4ef95-159">Replace</span></span> | <p><span data-ttu-id="4ef95-160">Substitui o destino pelo conteúdo fornecido.</span><span class="sxs-lookup"><span data-stu-id="4ef95-160">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="4ef95-161">A maioria das ações **replace** exige o uso de [ID gerada](#generated-ids) para o destino (exceto os elementos **img** e **object** em um div, que também é compatível com o uso de **data-id**).</span><span class="sxs-lookup"><span data-stu-id="4ef95-161">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
<span data-ttu-id="4ef95-162">**position**</span><span class="sxs-lookup"><span data-stu-id="4ef95-162">**position**</span></span>  
<span data-ttu-id="4ef95-163">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-163">The location to add the supplied content, relative to the target element. Possible values are:  (default) or .</span></span> <span data-ttu-id="4ef95-164">Usa o padrão **after** caso seja omitido.</span><span class="sxs-lookup"><span data-stu-id="4ef95-164">Defaults to **after** if omitted.</span></span>

| <span data-ttu-id="4ef95-165">Posição</span><span class="sxs-lookup"><span data-stu-id="4ef95-165">Position</span></span> | <span data-ttu-id="4ef95-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ef95-166">Description</span></span> |  
|------|------|  
| <span data-ttu-id="4ef95-167">after (padrão)</span><span class="sxs-lookup"><span data-stu-id="4ef95-167">after (default)</span></span> | <p><span data-ttu-id="4ef95-168">– Com **append**: último filho do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-168">- With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="4ef95-169">– Com **insert**: o irmão subsequente do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-169">- With **insert**: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="4ef95-170">before</span><span class="sxs-lookup"><span data-stu-id="4ef95-170">Before</span></span> | <p><span data-ttu-id="4ef95-171">– Com **append**: primeiro filho do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-171">- With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="4ef95-172">– Com **insert**: o irmão precedente do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-172">- With **insert**: The preceding sibling of the target element.</span></span></p> |

<span data-ttu-id="4ef95-173">**content**</span><span class="sxs-lookup"><span data-stu-id="4ef95-173">**content**</span></span>  
<span data-ttu-id="4ef95-174">Uma cadeia de caracteres de HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="4ef95-174">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the  content type with a "Commands" part.</span></span> <span data-ttu-id="4ef95-175">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o tipo de conteúdo `multipart/form-data` com uma parte "Commands" (veja um [exemplo](#multipart-request-with-binary-content).)</span><span class="sxs-lookup"><span data-stu-id="4ef95-175">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="4ef95-176">IDs geradas</span><span class="sxs-lookup"><span data-stu-id="4ef95-176">Generated IDs</span></span>
<span data-ttu-id="4ef95-177">O Microsoft Graph gera valores de **id** para que os elementos na página possam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4ef95-177">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="4ef95-178">Para obter as IDs geradas, use a expressão de cadeia de caracteres de consulta `includeIDs=true` na sua solicitação GET:</span><span class="sxs-lookup"><span data-stu-id="4ef95-178">To get generated IDs, use the `includeIDs=true` query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="4ef95-179">**Observação:** a API descarta todos os valores de **id** na [HTML de entrada](onenote_input_output_html.md) das solicitações de criar página e atualizar página.</span><span class="sxs-lookup"><span data-stu-id="4ef95-179">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote_input_output_html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="4ef95-180">O exemplo a seguir mostra IDs geradas para um parágrafo e uma imagem no [HTML de saída](onenote_input_output_html.md) de uma página.</span><span class="sxs-lookup"><span data-stu-id="4ef95-180">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote_input_output_html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="4ef95-181">Os valores de **id** gerados podem ser alterados após uma atualização de página. Então você deve obter valores atuais antes de criar uma solicitação de PATCH que usa esses valores.</span><span class="sxs-lookup"><span data-stu-id="4ef95-181">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="4ef95-182">Você pode especificar elementos de destino usando os valores **data-id** ou **id** seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="4ef95-182">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="4ef95-183">Para as ações **append** e **insert**, você pode usar o ID como o valor de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-183">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="4ef95-184">Para as ações **replace**, use o ID gerado para todos os elementos, exceto o título da página e imagens e objetos que estejam dentro de um div.</span><span class="sxs-lookup"><span data-stu-id="4ef95-184">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div.</span></span> 
    - <span data-ttu-id="4ef95-185">Para substituir um título, use a palavra-chave **título**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-185">To replace a title, use the **title** keyword.</span></span> 
    - <span data-ttu-id="4ef95-186">Para substituir imagens e objetos que estejam dentro de um div, use **data-id** ou **id**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-186">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="4ef95-187">O exemplo a seguir usa o valor **id** para o destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-187">The following example uses the **id** value for the target.</span></span> <span data-ttu-id="4ef95-188">Não use o prefixo # com um ID gerado.</span><span class="sxs-lookup"><span data-stu-id="4ef95-188">Don't use the # prefix with a generated ID.</span></span>

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

## <a name="supported-elements-and-actions"></a><span data-ttu-id="4ef95-189">Elementos e ações compatíveis</span><span class="sxs-lookup"><span data-stu-id="4ef95-189">Supported elements and actions</span></span>
<span data-ttu-id="4ef95-190">Muitos elementos na página podem ser atualizados, mas cada tipo de elemento é compatível com ações específicas.</span><span class="sxs-lookup"><span data-stu-id="4ef95-190">Many elements on the page can be updated, but each element type supports specific actions.</span></span> <span data-ttu-id="4ef95-191">A tabela a seguir mostra os elementos de destino compatíveis com as ações de atualização a que eles dão suporte.</span><span class="sxs-lookup"><span data-stu-id="4ef95-191">The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="4ef95-192">Elemento</span><span class="sxs-lookup"><span data-stu-id="4ef95-192">Element</span></span> | <span data-ttu-id="4ef95-193">Substituir</span><span class="sxs-lookup"><span data-stu-id="4ef95-193">Replace</span></span> | <span data-ttu-id="4ef95-194">Anexar filho</span><span class="sxs-lookup"><span data-stu-id="4ef95-194">Append child</span></span> | <span data-ttu-id="4ef95-195">Inserir irmão</span><span class="sxs-lookup"><span data-stu-id="4ef95-195">Insert sibling</span></span> |  
|------|------|------|------|  
| <span data-ttu-id="4ef95-196">body</span><span class="sxs-lookup"><span data-stu-id="4ef95-196">body</span></span><br /> <span data-ttu-id="4ef95-197">(tem como destino o primeiro div na página)</span><span class="sxs-lookup"><span data-stu-id="4ef95-197">(targets first div on the page)</span></span> | <span data-ttu-id="4ef95-198">não</span><span class="sxs-lookup"><span data-stu-id="4ef95-198">no</span></span> | <span data-ttu-id="4ef95-199">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-199">**yes**</span></span> | <span data-ttu-id="4ef95-200">não</span><span class="sxs-lookup"><span data-stu-id="4ef95-200">no</span></span> |  
| <span data-ttu-id="4ef95-201">div</span><span class="sxs-lookup"><span data-stu-id="4ef95-201">div</span></span><br /> <span data-ttu-id="4ef95-202">([absoluto posicionado](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="4ef95-202">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="4ef95-203">não</span><span class="sxs-lookup"><span data-stu-id="4ef95-203">no</span></span> | <span data-ttu-id="4ef95-204">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-204">**yes**</span></span> | <span data-ttu-id="4ef95-205">não</span><span class="sxs-lookup"><span data-stu-id="4ef95-205">no</span></span> |  
| <span data-ttu-id="4ef95-206">div</span><span class="sxs-lookup"><span data-stu-id="4ef95-206">div</span></span><br /> <span data-ttu-id="4ef95-207">(em um div)</span><span class="sxs-lookup"><span data-stu-id="4ef95-207">(within a div)</span></span> | <span data-ttu-id="4ef95-208">**sim** (somente id)</span><span class="sxs-lookup"><span data-stu-id="4ef95-208">**yes** (id only)</span></span> | <span data-ttu-id="4ef95-209">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-209">**Yes**</span></span> | <span data-ttu-id="4ef95-210">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-210">**Yes**</span></span> |   
| <span data-ttu-id="4ef95-211">img, object</span><span class="sxs-lookup"><span data-stu-id="4ef95-211">img, object</span></span><br /> <span data-ttu-id="4ef95-212">(em um div)</span><span class="sxs-lookup"><span data-stu-id="4ef95-212">(within a div)</span></span> | <span data-ttu-id="4ef95-213">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-213">**yes**</span></span> | <span data-ttu-id="4ef95-214">não</span><span class="sxs-lookup"><span data-stu-id="4ef95-214">no</span></span> | <span data-ttu-id="4ef95-215">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-215">**yes**</span></span> |   
| <span data-ttu-id="4ef95-216">ol, ul</span><span class="sxs-lookup"><span data-stu-id="4ef95-216">ol, ul</span></span> | <span data-ttu-id="4ef95-217">**sim** (somente id)</span><span class="sxs-lookup"><span data-stu-id="4ef95-217">**yes** (id only)</span></span> | <span data-ttu-id="4ef95-218">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-218">**Yes**</span></span> | <span data-ttu-id="4ef95-219">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-219">**Yes**</span></span> |   
| <span data-ttu-id="4ef95-220">table</span><span class="sxs-lookup"><span data-stu-id="4ef95-220">table</span></span> | <span data-ttu-id="4ef95-221">**sim** (somente id)</span><span class="sxs-lookup"><span data-stu-id="4ef95-221">**yes** (id only)</span></span> | <span data-ttu-id="4ef95-222">não</span><span class="sxs-lookup"><span data-stu-id="4ef95-222">no</span></span> | <span data-ttu-id="4ef95-223">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-223">**yes**</span></span> |   
| <span data-ttu-id="4ef95-224">p, li, h1-h6</span><span class="sxs-lookup"><span data-stu-id="4ef95-224">p, li, h1-h6</span></span> | <span data-ttu-id="4ef95-225">**sim** (somente id)</span><span class="sxs-lookup"><span data-stu-id="4ef95-225">**yes** (id only)</span></span> | <span data-ttu-id="4ef95-226">não</span><span class="sxs-lookup"><span data-stu-id="4ef95-226">no</span></span> | <span data-ttu-id="4ef95-227">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-227">**yes**</span></span> |   
| <span data-ttu-id="4ef95-228">title</span><span class="sxs-lookup"><span data-stu-id="4ef95-228">title</span></span> | <span data-ttu-id="4ef95-229">**sim**</span><span class="sxs-lookup"><span data-stu-id="4ef95-229">**yes**</span></span> | <span data-ttu-id="4ef95-230">não</span><span class="sxs-lookup"><span data-stu-id="4ef95-230">no</span></span> | <span data-ttu-id="4ef95-231">não</span><span class="sxs-lookup"><span data-stu-id="4ef95-231">no</span></span> |  
 

<span data-ttu-id="4ef95-232">Os seguintes elementos não dão suporte a nenhuma ação de atualização.</span><span class="sxs-lookup"><span data-stu-id="4ef95-232">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="4ef95-233">img ([absoluto posicionado](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="4ef95-233">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="4ef95-234">object ([absoluto posicionado](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="4ef95-234">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="4ef95-235">tr, td</span><span class="sxs-lookup"><span data-stu-id="4ef95-235">tr, td</span></span>
- <span data-ttu-id="4ef95-236">meta</span><span class="sxs-lookup"><span data-stu-id="4ef95-236">meta</span></span>
- <span data-ttu-id="4ef95-237">head</span><span class="sxs-lookup"><span data-stu-id="4ef95-237">head</span></span>
- <span data-ttu-id="4ef95-238">span</span><span class="sxs-lookup"><span data-stu-id="4ef95-238">span</span></span>
- <span data-ttu-id="4ef95-239">a</span><span class="sxs-lookup"><span data-stu-id="4ef95-239">a</span></span>
- <span data-ttu-id="4ef95-240">style tags</span><span class="sxs-lookup"><span data-stu-id="4ef95-240">style tags</span></span>


<a name="examples"></a>
## <a name="example-requests"></a><span data-ttu-id="4ef95-241">Solicitações de exemplo</span><span class="sxs-lookup"><span data-stu-id="4ef95-241">Example requests and responses</span></span>
<span data-ttu-id="4ef95-242">Uma solicitação de atualização contém um ou mais alterações representadas como objetos de alteração JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef95-242">An update request contains one or more changes represented as JSON change objects.</span></span> <span data-ttu-id="4ef95-243">Esses objetos podem definir destinos diferentes na página e outras ações e conteúdos diferentes para os destinos.</span><span class="sxs-lookup"><span data-stu-id="4ef95-243">These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="4ef95-244">Os exemplos a seguir contêm objetos JSON usados em solicitações de PATCH e solicitações de PATCH completo:</span><span class="sxs-lookup"><span data-stu-id="4ef95-244">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

<span data-ttu-id="4ef95-245">[Acrescentar elementos filho](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Inserir elementos irmãos](#insert-sibling-elements)&nbsp; &nbsp;| &nbsp; &nbsp; [Substituir elementos](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Solicitações de PATCH completo](#complete-patch-request-examples)</span><span class="sxs-lookup"><span data-stu-id="4ef95-245">[Append child elements](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Insert sibling elements](#insert-sibling-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Replace elements](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Complete PATCH requests](#complete-patch-request-examples)</span></span>


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="4ef95-246">Acrescentar elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ef95-246">Append child elements</span></span>
<span data-ttu-id="4ef95-247">A ação **append** adiciona um filho a um elemento **body**, **div** (dentro de um div), **ol** ou **ul**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-247">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element.</span></span> <span data-ttu-id="4ef95-248">O atributo **position** determina se deve acrescentar o filho antes ou depois do destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-248">The **position** attribute determines whether to append the child before or after the target.</span></span> <span data-ttu-id="4ef95-249">A posição padrão é **after**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-249">The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="4ef95-250">Acrescentar a um div</span><span class="sxs-lookup"><span data-stu-id="4ef95-250">Append to a div</span></span>

<span data-ttu-id="4ef95-251">O exemplo a seguir adiciona dois nós filho ao elemento **div1**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-251">The following example adds two child nodes to the **div1** element.</span></span> <span data-ttu-id="4ef95-252">Ele adiciona uma imagem como primeiro filho e um parágrafo como último filho.</span><span class="sxs-lookup"><span data-stu-id="4ef95-252">It adds an image as the first child and a paragraph as the last child.</span></span> 

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
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="4ef95-253">Acrescentar ao elemento *body*</span><span class="sxs-lookup"><span data-stu-id="4ef95-253">Append to the *body* element</span></span>

<span data-ttu-id="4ef95-254">Você pode usar o atalho **body** para acrescentar um elemento filho dentro o primeiro div em qualquer página.</span><span class="sxs-lookup"><span data-stu-id="4ef95-254">You can use the **body** shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="4ef95-255">O exemplo a seguir adiciona dois parágrafos como primeiro filho e último filho ao primeiro div na página.</span><span class="sxs-lookup"><span data-stu-id="4ef95-255">The following example adds two paragraphs as the first child and the last child to the first div on the page.</span></span> <span data-ttu-id="4ef95-256">Não use # com o destino **body**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-256">Don't use a # with the **body** target.</span></span> <span data-ttu-id="4ef95-257">Este exemplo usa a ação **prepend** como um atalho para **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-257">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

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
 

#### <a name="append-to-a-list"></a><span data-ttu-id="4ef95-258">Acrescentar a uma lista</span><span class="sxs-lookup"><span data-stu-id="4ef95-258">Append to a list</span></span>

<span data-ttu-id="4ef95-259">O exemplo a seguir adiciona um item de lista como um último filho à lista de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-259">The following example adds a list item as a last child to the target list.</span></span> <span data-ttu-id="4ef95-260">A propriedade **list-style-type** é definida porque o item usa um estilo de lista não padrão.</span><span class="sxs-lookup"><span data-stu-id="4ef95-260">The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

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

### <a name="insert-sibling-elements"></a><span data-ttu-id="4ef95-261">Inserir elementos irmãos</span><span class="sxs-lookup"><span data-stu-id="4ef95-261">Insert sibling elements</span></span>
<span data-ttu-id="4ef95-262">A ação **insert** adiciona irmão a um elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-262">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="4ef95-263">O atributo **position** determina se deve inserir o irmão antes ou depois do destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-263">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="4ef95-264">A posição padrão é **after**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-264">The default position is **after**.</span></span> <span data-ttu-id="4ef95-265">Ver [elementos compatíveis com **insert**](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="4ef95-265">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

<span data-ttu-id="4ef95-266">**Inserir irmão**</span><span class="sxs-lookup"><span data-stu-id="4ef95-266">**Insert siblings**</span></span>

<span data-ttu-id="4ef95-267">O exemplo a seguir adiciona dois nós irmão à página.</span><span class="sxs-lookup"><span data-stu-id="4ef95-267">The following example adds two sibling nodes to the page.</span></span> <span data-ttu-id="4ef95-268">Adiciona uma imagem acima do elemento **para1** elemento e um parágrafo abaixo do elemento **para2**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-268">It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

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

### <a name="replace-elements"></a><span data-ttu-id="4ef95-269">Substituir elementos</span><span class="sxs-lookup"><span data-stu-id="4ef95-269">Replace elements</span></span>

<span data-ttu-id="4ef95-270">Você pode usar **data-id** ou **id** gerado como o valor de destino para substituir os elementos **img** e **object** que estão em um div.</span><span class="sxs-lookup"><span data-stu-id="4ef95-270">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div.</span></span> <span data-ttu-id="4ef95-271">Para substituir um título de página, use a palavra-chave **title**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-271">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="4ef95-272">Para todos os outros [elementos compatíveis com **replace**](#supported-elements-and-actions), você deve usar o ID gerado.</span><span class="sxs-lookup"><span data-stu-id="4ef95-272">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="4ef95-273">Substituir uma imagem</span><span class="sxs-lookup"><span data-stu-id="4ef95-273">Replace an image</span></span>

<span data-ttu-id="4ef95-274">O exemplo a seguir substitui uma imagem por um div usando a **data-id** da imagem como destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-274">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="4ef95-275">Atualizar um tabela</span><span class="sxs-lookup"><span data-stu-id="4ef95-275">Update a table</span></span> 

<span data-ttu-id="4ef95-276">Este exemplo mostra como atualizar uma tabela usando seu ID gerado.</span><span class="sxs-lookup"><span data-stu-id="4ef95-276">This example shows how to update a table by using its generated ID.</span></span> <span data-ttu-id="4ef95-277">A substituição dos elementos **tr** e **td** não tem suporte, mas você pode substituir a tabela inteira.</span><span class="sxs-lookup"><span data-stu-id="4ef95-277">Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

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
 

#### <a name="change-the-title"></a><span data-ttu-id="4ef95-278">Alterar o título</span><span class="sxs-lookup"><span data-stu-id="4ef95-278">Change the title</span></span> 

<span data-ttu-id="4ef95-279">Este exemplo mostra como alterar o título da página.</span><span class="sxs-lookup"><span data-stu-id="4ef95-279">This example shows how to change the title of a page.</span></span> <span data-ttu-id="4ef95-280">Para alterar o título, use a palavra-chave **title** como o valor de destino.</span><span class="sxs-lookup"><span data-stu-id="4ef95-280">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="4ef95-281">Não use # com o destino de título.</span><span class="sxs-lookup"><span data-stu-id="4ef95-281">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="4ef95-282">Atualizar um item pendente</span><span class="sxs-lookup"><span data-stu-id="4ef95-282">Assign a to-do item</span></span>

<span data-ttu-id="4ef95-283">O exemplo a seguir usa a ação de substituir para alterar um item de caixa de seleção pendente para um estado concluído.</span><span class="sxs-lookup"><span data-stu-id="4ef95-283">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="4ef95-284">Veja [Usar marcas de anotação](onenote-note-tags.md) para saber mais sobre como usar o atributo **data-tag**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-284">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="4ef95-285">Exemplos de solicitação de PATCH completo</span><span class="sxs-lookup"><span data-stu-id="4ef95-285">Complete PATCH request examples</span></span>

<span data-ttu-id="4ef95-286">Os exemplos a seguir mostram solicitações de PATCH completo.</span><span class="sxs-lookup"><span data-stu-id="4ef95-286">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="4ef95-287">Solicitar apenas com conteúdo de texto</span><span class="sxs-lookup"><span data-stu-id="4ef95-287">Request with text content only</span></span>  
<span data-ttu-id="4ef95-288">O exemplo a seguir mostra uma solicitação de PATCH que usa o tipo de conteúdo **application/json**.</span><span class="sxs-lookup"><span data-stu-id="4ef95-288">The following example shows a PATCH request that uses the **application/json** content type.</span></span> <span data-ttu-id="4ef95-289">Você pode usar esse formato quando seu conteúdo não contém dados binários.</span><span class="sxs-lookup"><span data-stu-id="4ef95-289">You can use this format when your content doesn't contain binary data.</span></span>

```
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

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="4ef95-290">Solicitação de partes múltiplas com conteúdo binário</span><span class="sxs-lookup"><span data-stu-id="4ef95-290">Multipart request with binary content</span></span> 

<span data-ttu-id="4ef95-291">O exemplo a seguir mostra uma solicitação de PATCH de diversas partes que inclui dados binários.</span><span class="sxs-lookup"><span data-stu-id="4ef95-291">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="4ef95-292">As solicitações de diversas partes exigem uma parte de "Comandos" que especifica o tipo de conteúdo **application/json** e contém a matriz de objetos de alteração JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef95-292">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="4ef95-293">Outras partes de dados podem conter dados binários.</span><span class="sxs-lookup"><span data-stu-id="4ef95-293">Other data parts can contain binary data.</span></span> <span data-ttu-id="4ef95-294">Os nomes de partes são geralmente cadeias de caracteres acrescentadas com a hora atual em milissegundos ou um GUID aleatório.</span><span class="sxs-lookup"><span data-stu-id="4ef95-294">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```
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

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="4ef95-295">Informações de solicitação e resposta para solicitações de PATCH</span><span class="sxs-lookup"><span data-stu-id="4ef95-295">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="4ef95-296">Dados da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ef95-296">Request data</span></span> | <span data-ttu-id="4ef95-297">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ef95-297">Description</span></span> |  
|------|------|  
| <span data-ttu-id="4ef95-298">Protocolo</span><span class="sxs-lookup"><span data-stu-id="4ef95-298">Protocol</span></span> | <span data-ttu-id="4ef95-299">Todas as solicitações usam o protocolo HTTPS de SSL/TLS.</span><span class="sxs-lookup"><span data-stu-id="4ef95-299">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="4ef95-300">Cabeçalho de autorização</span><span class="sxs-lookup"><span data-stu-id="4ef95-300">Authorization header</span></span> | <p><span data-ttu-id="4ef95-301">`Bearer {token}`, onde *{token}* é um token de acesso do OAuth 2.0 válido para o aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="4ef95-301">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="4ef95-302">Se ele estiver ausente ou for inválido, a solicitação falhará com um código de status 401.</span><span class="sxs-lookup"><span data-stu-id="4ef95-302">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="4ef95-303">Confira [Autenticação e permissões](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ef95-303">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="4ef95-304">Cabeçalho content-type</span><span class="sxs-lookup"><span data-stu-id="4ef95-304">content-type header</span></span> | <p><span data-ttu-id="4ef95-305">`application/json` para a matriz de objetos de alteração JSON, seja enviado diretamente no corpo da mensagem, seja na parte "Comandos" obrigatória de [solicitações de diversas partes](#multipart-request-with-binary-content).</span><span class="sxs-lookup"><span data-stu-id="4ef95-305">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="4ef95-306">As solicitações de diversas partes são necessárias quando se enviam dados binários e usam o tipo de conteúdo `multipart/form-data; boundary=part-boundary`, onde *{part-boundary}* é uma cadeia de caracteres que sinaliza o início e o término de cada parte de dados.</span><span class="sxs-lookup"><span data-stu-id="4ef95-306">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where *{part-boundary}* is a string that signals the start and end of each data part.</span></span></p> |  
 

| <span data-ttu-id="4ef95-307">Dados de resposta</span><span class="sxs-lookup"><span data-stu-id="4ef95-307">Response data</span></span> | <span data-ttu-id="4ef95-308">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ef95-308">Description</span></span> |  
|------|------|  
| <span data-ttu-id="4ef95-309">Código de êxito</span><span class="sxs-lookup"><span data-stu-id="4ef95-309">Success code</span></span> | <span data-ttu-id="4ef95-310">Um código de status de HTTP 204.</span><span class="sxs-lookup"><span data-stu-id="4ef95-310">A 204 HTTP status code.</span></span> <span data-ttu-id="4ef95-311">Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="4ef95-311">If successful, this method returns a  response code.  No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="4ef95-312">Erros</span><span class="sxs-lookup"><span data-stu-id="4ef95-312">Errors</span></span> | <span data-ttu-id="4ef95-313">Leia [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote_error_codes.md) para saber mais sobre erros do OneNote que poderão ser retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4ef95-313">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="4ef95-314">Criar a URL raiz do serviço do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4ef95-314">Constructing the Microsoft Graph service root URL</span></span>

<a name="root-url"></a>

## <a name="root-url"></a><span data-ttu-id="4ef95-315">URL raiz</span><span class="sxs-lookup"><span data-stu-id="4ef95-315">URL Root</span></span>
<span data-ttu-id="4ef95-316">A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para o OneNote.</span><span class="sxs-lookup"><span data-stu-id="4ef95-316">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="4ef95-317">O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="4ef95-317">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>
- <span data-ttu-id="4ef95-318">`v1.0` serve para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="4ef95-318">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="4ef95-319">`beta` serve para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="4ef95-319">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="4ef95-320">Os recursos e a funcionalidade na versão beta podem mudar, por isso, você não deve usá-la no código de produção.</span><span class="sxs-lookup"><span data-stu-id="4ef95-320">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>
- <span data-ttu-id="4ef95-321">`me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="4ef95-321">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="4ef95-322">`users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="4ef95-322">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="4ef95-323">Use a [API do Microsoft Azure AD Graph](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="4ef95-323">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span></span>


> <span data-ttu-id="4ef95-324">**Observação:** para obter as ids de usuário, fazer uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="4ef95-324">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="4ef95-325">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ef95-325">Permissions</span></span>

<span data-ttu-id="4ef95-326">Para atualizar páginas do OneNote, solicite as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="4ef95-326">To update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="4ef95-327">Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="4ef95-327">Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="4ef95-328">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ef95-328">Notes.ReadWrite</span></span>
- <span data-ttu-id="4ef95-329">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ef95-329">Notes.ReadWrite.All</span></span>

<span data-ttu-id="4ef95-330">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ef95-330">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="additional-resources"></a><span data-ttu-id="4ef95-331">Recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="4ef95-331">Additional resources</span></span>

- [<span data-ttu-id="4ef95-332">Adicionar imagens e arquivos</span><span class="sxs-lookup"><span data-stu-id="4ef95-332">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="4ef95-333">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="4ef95-333">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="4ef95-334">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="4ef95-334">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="4ef95-335">Perguntas sobre desenvolvimento do OneNote no Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="4ef95-335">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="4ef95-336">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="4ef95-336">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
