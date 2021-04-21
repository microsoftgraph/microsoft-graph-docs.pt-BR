---
title: Atualizar o conteúdo da página do OneNote
description: " Blocos de anotações empresariais no Microsoft 365"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8786bcf8a0aa3aafaca8406f11e6243b8dd7b49c
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920100"
---
# <a name="update-onenote-page-content"></a><span data-ttu-id="a2fd8-103">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="a2fd8-103">Update OneNote page content</span></span>

<span data-ttu-id="a2fd8-104">**Aplica-se a** Notebooks de consumidores no OneDrive | Notebooks corporativos no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a2fd8-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>


<span data-ttu-id="a2fd8-105">Para atualizar o conteúdo de uma página do OneNote, envie uma solicitação de PATCH para o ponto de extremidade do *conteúdo* da página:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-105">To update the content of a OneNote page, you send a PATCH request to the page's *content* endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="a2fd8-p101">Envie um objeto de alteração JSON no corpo da mensagem. Se a solicitação for bem-sucedida, o Microsoft Graph retornará um código de status de HTTP 204.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-p101">Send a JSON change object in the message body. If the request is successful, Microsoft Graph returns a 204 HTTP status code.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="a2fd8-108">Construir a URI de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2fd8-108">Construct the request URI</span></span>

<span data-ttu-id="a2fd8-109">Para construir a URI de solicitação, comece com a URL raiz do serviço:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="a2fd8-110">Acrescente então o ponto de extremidade do *conteúdo* da página:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-110">Then append the page's *content* endpoint:</span></span>

- <span data-ttu-id="a2fd8-111">**Obter o HTML da página e todos os valores de *data-id* definidos**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-111">**Get the page HTML and all defined *data-id* values**</span></span><br/><br/>`../pages/{id}/content`   

- <span data-ttu-id="a2fd8-112">**Obter o HTML da página, todos os valores de *data-id* definidos e todos os valores de *id* gerados**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-112">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span><br/><br/>`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="a2fd8-113">A **data-id** e os valores de **id** são usados como identificadores de **destino** para elementos que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-113">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="a2fd8-114">Sua solicitação de URI completa terá a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-114">Your full request URI will look like this:</span></span><br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="a2fd8-115">Saiba mais sobre a [URL raiz de serviço](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-115">Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="a2fd8-116">Criar o corpo da mensagem</span><span class="sxs-lookup"><span data-stu-id="a2fd8-116">Construct the message body</span></span>

<span data-ttu-id="a2fd8-117">O HTML de uma página do OneNote contém texto, imagens e outros conteúdos organizados em estruturas como elementos **div**, **img** e **ol**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-117">The HTML of a OneNote page contains text, images, and other content organized into structures such as **div**, **img**, and **ol** elements.</span></span> <span data-ttu-id="a2fd8-118">Para atualizar o conteúdo da página do OneNote, adicione e substitua elementos HTML na página.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-118">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="a2fd8-119">Suas alterações serão enviadas no corpo da mensagem como uma matriz de objetos de alteração JSON.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-119">Your changes are sent in the message body as an array of JSON change objects.</span></span> <span data-ttu-id="a2fd8-120">Cada objeto especifica o elemento de destino, o novo conteúdo HTML e o que fazer com o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-120">Each object specifies the target element, new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="a2fd8-121">A matriz a seguir define duas alterações.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-121">The following array defines two changes.</span></span> <span data-ttu-id="a2fd8-122">A primeira insere uma imagem acima de um parágrafo como um irmão, e a segunda acrescenta um item em uma lista como um último filho.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-122">The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

> [!NOTE]
> <span data-ttu-id="a2fd8-123">Ao atualizar uma imagem em uma página do OneNote, não é possível usar links de www.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-123">When updating an image on a OneNote page, you can't use www links.</span></span> <span data-ttu-id="a2fd8-124">O serviço não tentará baixar recursos aleatórios.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-124">The service won't try to download random resources.</span></span> <span data-ttu-id="a2fd8-125">Em vez disso, a imagem deve fazer parte da solicitação, seja por uma imagem-data-url ou um nome de parte de uma solicitação de várias partes.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-125">Instead, the image must be part of the request, either by an image-data-url or a part-name of a multipart request.</span></span>

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

<span data-ttu-id="a2fd8-126">Veja [mais exemplos](#example-requests).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-126">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="a2fd8-127">Atributos de objetos de alteração JSON</span><span class="sxs-lookup"><span data-stu-id="a2fd8-127">Attributes for JSON change objects</span></span>

<span data-ttu-id="a2fd8-128">Use atributos **target**, **action**, **position** e **content** para definir objetos JSON para solicitações de PATCH.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-128">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

#### <a name="target"></a><span data-ttu-id="a2fd8-129">destino</span><span class="sxs-lookup"><span data-stu-id="a2fd8-129">target</span></span>

<span data-ttu-id="a2fd8-130">O elemento a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-130">The element to update.</span></span> <span data-ttu-id="a2fd8-131">O valor deve ser uma dos seguintes identificadores:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-131">The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="a2fd8-132">Identificador</span><span class="sxs-lookup"><span data-stu-id="a2fd8-132">Identifier</span></span> | <span data-ttu-id="a2fd8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2fd8-133">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2fd8-134">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="a2fd8-134">#{data-id}</span></span> | <p><span data-ttu-id="a2fd8-135">Essa ID é opcionalmente definida em elementos na HTML de entrada ao [criar uma página](onenote-create-page.md) ou [atualizar uma página](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-135">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote-update-page.md).</span></span> <span data-ttu-id="a2fd8-136">Coloque um # como prefixo do valor.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-136">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="a2fd8-137">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-137">Example:</span></span><br/><span data-ttu-id="a2fd8-138">`'target':'#intro'` tem como destino o elemento `<div data-id="intro" ...>`</span><span class="sxs-lookup"><span data-stu-id="a2fd8-138">`'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="a2fd8-139">id</span><span class="sxs-lookup"><span data-stu-id="a2fd8-139">id</span></span> | <p><span data-ttu-id="a2fd8-140">É a [ID gerada](#generated-ids) do Microsoft Graph e é necessário para a maioria das operações de substituição.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-140">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="a2fd8-141">Não use # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-141">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="a2fd8-142">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-142">Example:</span></span><br/><span data-ttu-id="a2fd8-143">`'target':'div:{33f8a2...}{37}'` tem como destino o elemento `<div id="div:{33f8a2...}{37}" ...>`</span><span class="sxs-lookup"><span data-stu-id="a2fd8-143">`'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="a2fd8-144">Não confunda esses identificadores com valores de **id** definidos no [HTML de entrada](onenote-input-output-html.md).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-144">Don't confuse these with any **id** values defined in the [input HTML](onenote-input-output-html.md).</span></span> <span data-ttu-id="a2fd8-145">Todos os valores de **id** enviados no HTML de entrada são descartados.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-145">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="a2fd8-146">body</span><span class="sxs-lookup"><span data-stu-id="a2fd8-146">body</span></span> | <span data-ttu-id="a2fd8-147">A palavra-chave que tem como destino o primeiro div na página.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-147">The keyword that targets the first div on the page.</span></span> <span data-ttu-id="a2fd8-148">Não use # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-148">Do not prefix with a #.</span></span> |  
| <span data-ttu-id="a2fd8-149">title</span><span class="sxs-lookup"><span data-stu-id="a2fd8-149">title</span></span> | <span data-ttu-id="a2fd8-150">A palavra-chave que tem como destino o título da página.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-150">The keyword that targets the page title.</span></span> <span data-ttu-id="a2fd8-151">Não use # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-151">Do not prefix with a #.</span></span> |  
 
#### <a name="action"></a><span data-ttu-id="a2fd8-152">action</span><span class="sxs-lookup"><span data-stu-id="a2fd8-152">action</span></span>

<span data-ttu-id="a2fd8-153">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-153">The action to perform on the target element.</span></span> <span data-ttu-id="a2fd8-154">Veja as [ações com suporte para elementos](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-154">See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="a2fd8-155">Ação</span><span class="sxs-lookup"><span data-stu-id="a2fd8-155">Action</span></span> | <span data-ttu-id="a2fd8-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2fd8-156">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2fd8-157">append</span><span class="sxs-lookup"><span data-stu-id="a2fd8-157">append</span></span> | <p><span data-ttu-id="a2fd8-158">Adiciona o conteúdo fornecido ao destino como primeiro ou último filho, conforme determinado pelo atributo **position**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-158">Adds the supplied content to the target as a first or last child, as determined by the **position** attribute.</span></span></p><p><span data-ttu-id="a2fd8-159">Aplicável somente a elementos **body**, **div**, **ol** e **ul**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-159">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="a2fd8-160">insert</span><span class="sxs-lookup"><span data-stu-id="a2fd8-160">insert</span></span> | <span data-ttu-id="a2fd8-161">Adiciona o conteúdo fornecido como irmão antes ou depois do destino, conforme determinado pelo atributo **position**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-161">Adds the supplied content as a sibling before or after the target, as determined by the **position** attribute.</span></span> |  
| <span data-ttu-id="a2fd8-162">prepend</span><span class="sxs-lookup"><span data-stu-id="a2fd8-162">prepend</span></span> | <p><span data-ttu-id="a2fd8-163">Adiciona o conteúdo fornecido ao destino como um primeiro filho.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-163">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="a2fd8-164">Atalho para **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-164">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="a2fd8-165">Aplicável somente a elementos **body**, **div**, **ol** e **ul**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-165">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="a2fd8-166">replace</span><span class="sxs-lookup"><span data-stu-id="a2fd8-166">replace</span></span> | <p><span data-ttu-id="a2fd8-167">Substitui o destino pelo conteúdo fornecido.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-167">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="a2fd8-168">A maioria das ações **replace** exige o uso de [ID gerada](#generated-ids) para o destino (exceto os elementos **img** e **object** em um div, que também é compatível com o uso de **data-id**).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-168">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
#### <a name="position"></a><span data-ttu-id="a2fd8-169">position</span><span class="sxs-lookup"><span data-stu-id="a2fd8-169">position</span></span>

<span data-ttu-id="a2fd8-170">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-170">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="a2fd8-171">Usa o padrão **after** caso seja omitido.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-171">Defaults to **after** if omitted.</span></span>

| <span data-ttu-id="a2fd8-172">Posição</span><span class="sxs-lookup"><span data-stu-id="a2fd8-172">Position</span></span> | <span data-ttu-id="a2fd8-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2fd8-173">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2fd8-174">after (padrão)</span><span class="sxs-lookup"><span data-stu-id="a2fd8-174">after (default)</span></span> |<p><span data-ttu-id="a2fd8-175">Com **append**: último filho do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-175">With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="a2fd8-176">Com **insert**: o irmão subsequente do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-176">With **insert**: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="a2fd8-177">before</span><span class="sxs-lookup"><span data-stu-id="a2fd8-177">before</span></span> | <p><span data-ttu-id="a2fd8-178">Com **append**: primeiro filho do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-178">With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="a2fd8-179">Com **insert**: o irmão precedente do elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-179">With **insert**: The preceding sibling of the target element.</span></span></p> |

#### <a name="content"></a><span data-ttu-id="a2fd8-180">content</span><span class="sxs-lookup"><span data-stu-id="a2fd8-180">content</span></span>

<span data-ttu-id="a2fd8-181">Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-181">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="a2fd8-182">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o tipo de conteúdo `multipart/form-data` com uma parte "Commands" (veja um [exemplo](#multipart-request-with-binary-content).)</span><span class="sxs-lookup"><span data-stu-id="a2fd8-182">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part (see an [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="a2fd8-183">IDs geradas</span><span class="sxs-lookup"><span data-stu-id="a2fd8-183">Generated IDs</span></span>
<span data-ttu-id="a2fd8-184">O Microsoft Graph gera valores de **id** para que os elementos na página possam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-184">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="a2fd8-185">Para obter as IDs geradas, use a expressão de cadeia de caracteres de consulta `includeIDs=true` na sua solicitação GET:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-185">To get generated IDs, use the `includeIDs=true` query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="a2fd8-186">**Observação:** a API descarta todos os valores de **id** na [HTML de entrada](onenote-input-output-html.md) das solicitações de criar página e atualizar página.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-186">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote-input-output-html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="a2fd8-187">O exemplo a seguir mostra IDs geradas para um parágrafo e uma imagem no [HTML de saída](onenote-input-output-html.md) de uma página.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-187">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote-input-output-html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="a2fd8-188">Os valores de **id** gerados podem ser alterados após uma atualização de página. Então você deve obter valores atuais antes de criar uma solicitação de PATCH que usa esses valores.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-188">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="a2fd8-189">Você pode especificar elementos de destino usando os valores **data-id** ou **id** seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-189">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="a2fd8-190">Para as ações **append** e **insert**, você pode usar o ID como o valor de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-190">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="a2fd8-191">Para as ações **replace**, use o ID gerado para todos os elementos, exceto o título da página e imagens e objetos que estejam dentro de um div.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-191">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div.</span></span> 
  - <span data-ttu-id="a2fd8-192">Para substituir um título, use a palavra-chave **título**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-192">To replace a title, use the **title** keyword.</span></span> 
  - <span data-ttu-id="a2fd8-193">Para substituir imagens e objetos que estejam dentro de um div, use **data-id** ou **id**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-193">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="a2fd8-194">O exemplo a seguir usa o valor **id** para o destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-194">The following example uses the **id** value for the target.</span></span> <span data-ttu-id="a2fd8-195">Não use o prefixo # com um ID gerado.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-195">Don't use the # prefix with a generated ID.</span></span>

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

## <a name="supported-elements-and-actions"></a><span data-ttu-id="a2fd8-196">Elementos e ações compatíveis</span><span class="sxs-lookup"><span data-stu-id="a2fd8-196">Supported elements and actions</span></span>

<span data-ttu-id="a2fd8-197">Muitos elementos na página podem ser atualizados, mas cada tipo de elemento é compatível com ações específicas.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-197">Many elements on the page can be updated, but each element type supports specific actions.</span></span> <span data-ttu-id="a2fd8-198">A tabela a seguir mostra os elementos de destino compatíveis com as ações de atualização a que eles dão suporte.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-198">The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="a2fd8-199">Elemento</span><span class="sxs-lookup"><span data-stu-id="a2fd8-199">Element</span></span> | <span data-ttu-id="a2fd8-200">Substituir</span><span class="sxs-lookup"><span data-stu-id="a2fd8-200">Replace</span></span> | <span data-ttu-id="a2fd8-201">Anexar filho</span><span class="sxs-lookup"><span data-stu-id="a2fd8-201">Append child</span></span> | <span data-ttu-id="a2fd8-202">Inserir irmão</span><span class="sxs-lookup"><span data-stu-id="a2fd8-202">Insert sibling</span></span> |  
|------|:------:|:------:|:------:|  
| <span data-ttu-id="a2fd8-203">body</span><span class="sxs-lookup"><span data-stu-id="a2fd8-203">body</span></span><br /> <span data-ttu-id="a2fd8-204">(tem como destino o primeiro div na página)</span><span class="sxs-lookup"><span data-stu-id="a2fd8-204">(targets first div on the page)</span></span> | <span data-ttu-id="a2fd8-205">não</span><span class="sxs-lookup"><span data-stu-id="a2fd8-205">no</span></span> | <span data-ttu-id="a2fd8-206">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-206">**yes**</span></span> | <span data-ttu-id="a2fd8-207">não</span><span class="sxs-lookup"><span data-stu-id="a2fd8-207">no</span></span> |  
| <span data-ttu-id="a2fd8-208">div</span><span class="sxs-lookup"><span data-stu-id="a2fd8-208">div</span></span><br /> <span data-ttu-id="a2fd8-209">([absoluto posicionado](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="a2fd8-209">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="a2fd8-210">não</span><span class="sxs-lookup"><span data-stu-id="a2fd8-210">no</span></span> | <span data-ttu-id="a2fd8-211">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-211">**yes**</span></span> | <span data-ttu-id="a2fd8-212">não</span><span class="sxs-lookup"><span data-stu-id="a2fd8-212">no</span></span> |  
| <span data-ttu-id="a2fd8-213">div</span><span class="sxs-lookup"><span data-stu-id="a2fd8-213">div</span></span><br /> <span data-ttu-id="a2fd8-214">(em um div)</span><span class="sxs-lookup"><span data-stu-id="a2fd8-214">(within a div)</span></span> | <span data-ttu-id="a2fd8-215">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-215">**yes**</span></span><br/><span data-ttu-id="a2fd8-216">(somente id)</span><span class="sxs-lookup"><span data-stu-id="a2fd8-216">(id only)</span></span> | <span data-ttu-id="a2fd8-217">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-217">**yes**</span></span> | <span data-ttu-id="a2fd8-218">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-218">**yes**</span></span> |   
| <span data-ttu-id="a2fd8-219">img, object</span><span class="sxs-lookup"><span data-stu-id="a2fd8-219">img, object</span></span><br /> <span data-ttu-id="a2fd8-220">(em um div)</span><span class="sxs-lookup"><span data-stu-id="a2fd8-220">(within a div)</span></span> | <span data-ttu-id="a2fd8-221">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-221">**yes**</span></span> | <span data-ttu-id="a2fd8-222">não</span><span class="sxs-lookup"><span data-stu-id="a2fd8-222">no</span></span> | <span data-ttu-id="a2fd8-223">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-223">**yes**</span></span> |   
| <span data-ttu-id="a2fd8-224">ol, ul</span><span class="sxs-lookup"><span data-stu-id="a2fd8-224">ol, ul</span></span> | <span data-ttu-id="a2fd8-225">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-225">**yes**</span></span><br/><span data-ttu-id="a2fd8-226">(somente id)</span><span class="sxs-lookup"><span data-stu-id="a2fd8-226">(id only)</span></span> | <span data-ttu-id="a2fd8-227">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-227">**yes**</span></span> | <span data-ttu-id="a2fd8-228">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-228">**yes**</span></span> |   
| <span data-ttu-id="a2fd8-229">table</span><span class="sxs-lookup"><span data-stu-id="a2fd8-229">table</span></span> | <span data-ttu-id="a2fd8-230">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-230">**yes**</span></span><br/><span data-ttu-id="a2fd8-231">(somente id)</span><span class="sxs-lookup"><span data-stu-id="a2fd8-231">(id only)</span></span> | <span data-ttu-id="a2fd8-232">não</span><span class="sxs-lookup"><span data-stu-id="a2fd8-232">no</span></span> | <span data-ttu-id="a2fd8-233">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-233">**yes**</span></span> |   
| <span data-ttu-id="a2fd8-234">p, li, h1-h6</span><span class="sxs-lookup"><span data-stu-id="a2fd8-234">p, li, h1-h6</span></span> | <span data-ttu-id="a2fd8-235">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-235">**yes**</span></span><br/><span data-ttu-id="a2fd8-236">(somente id)</span><span class="sxs-lookup"><span data-stu-id="a2fd8-236">(id only)</span></span> | <span data-ttu-id="a2fd8-237">não</span><span class="sxs-lookup"><span data-stu-id="a2fd8-237">no</span></span> | <span data-ttu-id="a2fd8-238">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-238">**yes**</span></span> |   
| <span data-ttu-id="a2fd8-239">title</span><span class="sxs-lookup"><span data-stu-id="a2fd8-239">title</span></span> | <span data-ttu-id="a2fd8-240">**sim**</span><span class="sxs-lookup"><span data-stu-id="a2fd8-240">**yes**</span></span> | <span data-ttu-id="a2fd8-241">não</span><span class="sxs-lookup"><span data-stu-id="a2fd8-241">no</span></span> | <span data-ttu-id="a2fd8-242">não</span><span class="sxs-lookup"><span data-stu-id="a2fd8-242">no</span></span> |  
 
<br/>

<span data-ttu-id="a2fd8-243">Os seguintes elementos não dão suporte a nenhuma ação de atualização.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-243">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="a2fd8-244">img ([absoluto posicionado](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="a2fd8-244">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="a2fd8-245">object ([absoluto posicionado](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="a2fd8-245">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="a2fd8-246">tr, td</span><span class="sxs-lookup"><span data-stu-id="a2fd8-246">tr, td</span></span>
- <span data-ttu-id="a2fd8-247">meta</span><span class="sxs-lookup"><span data-stu-id="a2fd8-247">meta</span></span>
- <span data-ttu-id="a2fd8-248">head</span><span class="sxs-lookup"><span data-stu-id="a2fd8-248">head</span></span>
- <span data-ttu-id="a2fd8-249">span</span><span class="sxs-lookup"><span data-stu-id="a2fd8-249">span</span></span>
- <span data-ttu-id="a2fd8-250">a</span><span class="sxs-lookup"><span data-stu-id="a2fd8-250">a</span></span>
- <span data-ttu-id="a2fd8-251">style tags</span><span class="sxs-lookup"><span data-stu-id="a2fd8-251">style tags</span></span>


<a name="examples"></a>

## <a name="example-requests"></a><span data-ttu-id="a2fd8-252">Solicitações de exemplo</span><span class="sxs-lookup"><span data-stu-id="a2fd8-252">Example requests</span></span>

<span data-ttu-id="a2fd8-253">Uma solicitação de atualização contém um ou mais alterações representadas como objetos de alteração JSON.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-253">An update request contains one or more changes represented as JSON change objects.</span></span> <span data-ttu-id="a2fd8-254">Esses objetos podem definir destinos diferentes na página e outras ações e conteúdos diferentes para os destinos.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-254">These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="a2fd8-255">Os exemplos a seguir contêm objetos JSON usados em solicitações de PATCH e solicitações de PATCH completo:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-255">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

- [<span data-ttu-id="a2fd8-256">Acrescentar elementos filho</span><span class="sxs-lookup"><span data-stu-id="a2fd8-256">Append child elements</span></span>](#append-child-elements)
- [<span data-ttu-id="a2fd8-257">Inserir elementos irmãos</span><span class="sxs-lookup"><span data-stu-id="a2fd8-257">Insert sibling elements</span></span>](#insert-sibling-elements)
- [<span data-ttu-id="a2fd8-258">Substituir elementos</span><span class="sxs-lookup"><span data-stu-id="a2fd8-258">Replace elements</span></span>](#replace-elements)
- [<span data-ttu-id="a2fd8-259">Solicitações de PATCH completo</span><span class="sxs-lookup"><span data-stu-id="a2fd8-259">Complete PATCH requests</span></span>](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="a2fd8-260">Acrescentar elementos filho</span><span class="sxs-lookup"><span data-stu-id="a2fd8-260">Append child elements</span></span>

<span data-ttu-id="a2fd8-261">A ação **append** adiciona um filho a um elemento **body**, **div** (dentro de um div), **ol** ou **ul**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-261">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element.</span></span> <span data-ttu-id="a2fd8-262">O atributo **position** determina se deve acrescentar o filho antes ou depois do destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-262">The **position** attribute determines whether to append the child before or after the target.</span></span> <span data-ttu-id="a2fd8-263">A posição padrão é **after**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-263">The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="a2fd8-264">Acrescentar a um div</span><span class="sxs-lookup"><span data-stu-id="a2fd8-264">Append to a div</span></span>

<span data-ttu-id="a2fd8-265">O exemplo a seguir adiciona dois nós filho ao elemento **div1**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-265">The following example adds two child nodes to the **div1** element.</span></span> <span data-ttu-id="a2fd8-266">Ele adiciona uma imagem como primeiro filho e um parágrafo como último filho.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-266">It adds an image as the first child and a paragraph as the last child.</span></span> 

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
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="a2fd8-267">Acrescentar ao elemento *body*</span><span class="sxs-lookup"><span data-stu-id="a2fd8-267">Append to the *body* element</span></span>

<span data-ttu-id="a2fd8-268">Você pode usar o atalho **body** para acrescentar um elemento filho dentro o primeiro div em qualquer página.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-268">You can use the **body** shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="a2fd8-269">O exemplo a seguir adiciona dois parágrafos como primeiro filho e último filho ao primeiro div na página.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-269">The following example adds two paragraphs as the first child and the last child to the first div on the page.</span></span> <span data-ttu-id="a2fd8-270">Não use # com o destino **body**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-270">Don't use a # with the **body** target.</span></span> <span data-ttu-id="a2fd8-271">Este exemplo usa a ação **prepend** como um atalho para **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-271">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

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
 

#### <a name="append-to-a-list"></a><span data-ttu-id="a2fd8-272">Acrescentar a uma lista</span><span class="sxs-lookup"><span data-stu-id="a2fd8-272">Append to a list</span></span>

<span data-ttu-id="a2fd8-273">O exemplo a seguir adiciona um item de lista como um último filho à lista de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-273">The following example adds a list item as a last child to the target list.</span></span> <span data-ttu-id="a2fd8-274">A propriedade **list-style-type** é definida porque o item usa um estilo de lista não padrão.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-274">The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

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

### <a name="insert-sibling-elements"></a><span data-ttu-id="a2fd8-275">Inserir elementos irmãos</span><span class="sxs-lookup"><span data-stu-id="a2fd8-275">Insert sibling elements</span></span>

<span data-ttu-id="a2fd8-276">A ação **insert** adiciona irmão a um elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-276">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="a2fd8-277">O atributo **position** determina se deve inserir o irmão antes ou depois do destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-277">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="a2fd8-278">A posição padrão é **after**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-278">The default position is **after**.</span></span> <span data-ttu-id="a2fd8-279">Ver [elementos compatíveis com **insert**](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-279">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

#### <a name="insert-siblings"></a><span data-ttu-id="a2fd8-280">Inserir irmãos</span><span class="sxs-lookup"><span data-stu-id="a2fd8-280">Insert siblings</span></span>

<span data-ttu-id="a2fd8-281">O exemplo a seguir adiciona dois nós irmãos à página.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-281">The following example adds two sibling nodes to the page.</span></span> <span data-ttu-id="a2fd8-282">Adiciona uma imagem acima do elemento **para1** elemento e um parágrafo abaixo do elemento **para2**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-282">It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-data-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a><span data-ttu-id="a2fd8-283">Substituir elementos</span><span class="sxs-lookup"><span data-stu-id="a2fd8-283">Replace elements</span></span>

<span data-ttu-id="a2fd8-284">Você pode usar **data-id** ou **id** gerado como o valor de destino para substituir os elementos **img** e **object** que estão em um div.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-284">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div.</span></span> <span data-ttu-id="a2fd8-285">Para substituir um título de página, use a palavra-chave **title**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-285">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="a2fd8-286">Para todos os outros [elementos compatíveis com **replace**](#supported-elements-and-actions), você deve usar o ID gerado.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-286">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="a2fd8-287">Substituir uma imagem</span><span class="sxs-lookup"><span data-stu-id="a2fd8-287">Replace an image</span></span>

<span data-ttu-id="a2fd8-288">O exemplo a seguir substitui uma imagem por um div usando a **data-id** da imagem como destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-288">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="a2fd8-289">Atualizar um tabela</span><span class="sxs-lookup"><span data-stu-id="a2fd8-289">Update a table</span></span> 

<span data-ttu-id="a2fd8-290">Este exemplo mostra como atualizar uma tabela usando seu ID gerado.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-290">This example shows how to update a table by using its generated ID.</span></span> <span data-ttu-id="a2fd8-291">A substituição dos elementos **tr** e **td** não tem suporte, mas você pode substituir a tabela inteira.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-291">Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

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
 

#### <a name="change-the-title"></a><span data-ttu-id="a2fd8-292">Alterar o título</span><span class="sxs-lookup"><span data-stu-id="a2fd8-292">Change the title</span></span> 

<span data-ttu-id="a2fd8-293">Este exemplo mostra como alterar o título da página.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-293">This example shows how to change the title of a page.</span></span> <span data-ttu-id="a2fd8-294">Para alterar o título, use a palavra-chave **title** como o valor de destino.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-294">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="a2fd8-295">Não use # com o destino de título.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-295">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="a2fd8-296">Atualizar um item pendente</span><span class="sxs-lookup"><span data-stu-id="a2fd8-296">Update a to-do item</span></span>

<span data-ttu-id="a2fd8-297">O exemplo a seguir usa a ação de substituir para alterar um item de caixa de seleção pendente para um estado concluído.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-297">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="a2fd8-298">Veja [Usar marcas de anotação](onenote-note-tags.md) para saber mais sobre como usar o atributo **data-tag**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-298">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="a2fd8-299">Exemplos de solicitação de PATCH completo</span><span class="sxs-lookup"><span data-stu-id="a2fd8-299">Complete PATCH request examples</span></span>

<span data-ttu-id="a2fd8-300">Os exemplos a seguir mostram solicitações de PATCH completo.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-300">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="a2fd8-301">Solicitar apenas com conteúdo de texto</span><span class="sxs-lookup"><span data-stu-id="a2fd8-301">Request with text content only</span></span>

<span data-ttu-id="a2fd8-302">O exemplo a seguir mostra uma solicitação de PATCH que usa o tipo de conteúdo **application/json**.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-302">The following example shows a PATCH request that uses the **application/json** content type.</span></span> <span data-ttu-id="a2fd8-303">Você pode usar esse formato quando seu conteúdo não contém dados binários.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-303">You can use this format when your content doesn't contain binary data.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="a2fd8-304">Solicitação de partes múltiplas com conteúdo binário</span><span class="sxs-lookup"><span data-stu-id="a2fd8-304">Multipart request with binary content</span></span> 

<span data-ttu-id="a2fd8-305">O exemplo a seguir mostra uma solicitação de PATCH de diversas partes que inclui dados binários.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-305">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="a2fd8-306">As solicitações de diversas partes exigem uma parte de "Comandos" que especifica o tipo de conteúdo **application/json** e contém a matriz de objetos de alteração JSON.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-306">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="a2fd8-307">Outras partes de dados podem conter dados binários.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-307">Other data parts can contain binary data.</span></span> <span data-ttu-id="a2fd8-308">Os nomes de partes são geralmente cadeias de caracteres acrescentadas com a hora atual em milissegundos ou um GUID aleatório.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-308">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```http
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

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="a2fd8-309">Informações de solicitação e resposta para solicitações de PATCH</span><span class="sxs-lookup"><span data-stu-id="a2fd8-309">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="a2fd8-310">Dados da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2fd8-310">Request data</span></span> | <span data-ttu-id="a2fd8-311">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2fd8-311">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2fd8-312">Protocolo</span><span class="sxs-lookup"><span data-stu-id="a2fd8-312">Protocol</span></span> | <span data-ttu-id="a2fd8-313">Todas as solicitações usam o protocolo HTTPS de SSL/TLS.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-313">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="a2fd8-314">Cabeçalho de autorização</span><span class="sxs-lookup"><span data-stu-id="a2fd8-314">Authorization header</span></span> | <p><span data-ttu-id="a2fd8-315">`Bearer {token}`, onde `{token}` é um token de acesso do OAuth 2.0 válido para o aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-315">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="a2fd8-316">Se ele estiver ausente ou for inválido, a solicitação falhará com um código de status 401.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-316">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="a2fd8-317">Confira [Autenticação e permissões](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-317">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="a2fd8-318">Cabeçalho content-type</span><span class="sxs-lookup"><span data-stu-id="a2fd8-318">Content-Type header</span></span> | <p><span data-ttu-id="a2fd8-319">`application/json` para a matriz de objetos de alteração JSON, seja enviado diretamente no corpo da mensagem, seja na parte "Comandos" obrigatória de [solicitações de diversas partes](#multipart-request-with-binary-content).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-319">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="a2fd8-320">As solicitações de diversas partes são necessárias quando se enviam dados binários e usam o tipo de conteúdo `multipart/form-data; boundary=part-boundary`, onde `{part-boundary}` é uma cadeia de caracteres que sinaliza o início e o término de cada parte de dados.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-320">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  

<br/> 

| <span data-ttu-id="a2fd8-321">Dados de resposta</span><span class="sxs-lookup"><span data-stu-id="a2fd8-321">Response data</span></span> | <span data-ttu-id="a2fd8-322">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2fd8-322">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2fd8-323">Código de êxito</span><span class="sxs-lookup"><span data-stu-id="a2fd8-323">Success code</span></span> | <span data-ttu-id="a2fd8-324">Um código de status de HTTP 204.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-324">A 204 HTTP status code.</span></span> <span data-ttu-id="a2fd8-325">Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-325">No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="a2fd8-326">Erros</span><span class="sxs-lookup"><span data-stu-id="a2fd8-326">Errors</span></span> | <span data-ttu-id="a2fd8-327">Leia [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote-error-codes.md) para saber mais sobre erros do OneNote que poderão ser retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-327">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="a2fd8-328">Criar a URL raiz do serviço do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a2fd8-328">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="a2fd8-329">A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para o OneNote:</span><span class="sxs-lookup"><span data-stu-id="a2fd8-329">The OneNote service root URL uses the following format for all calls to the OneNote API:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="a2fd8-330">O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-330">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="a2fd8-331">`v1.0` serve para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-331">`v1.0` is for stable production code.</span></span> <span data-ttu-id="a2fd8-332">`beta` serve para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-332">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="a2fd8-333">Os recursos e a funcionalidade na versão beta podem mudar, por isso, você não deve usá-la no código de produção.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-333">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>

<span data-ttu-id="a2fd8-334">`me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-334">`me` is for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="a2fd8-335">`users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-335">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="a2fd8-336">Use a [API do Microsoft Azure AD Graph](/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-336">Use the [Azure AD Graph API](/previous-versions/azure/ad/graph/api/api-catalog).</span></span>


> <span data-ttu-id="a2fd8-337">**Observação:** para obter as ids de usuário, faça uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-337">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="a2fd8-338">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2fd8-338">Permissions</span></span>

<span data-ttu-id="a2fd8-339">Para atualizar páginas do OneNote, solicite as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-339">To update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="a2fd8-340">Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2fd8-340">Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="a2fd8-341">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2fd8-341">Notes.ReadWrite</span></span>
- <span data-ttu-id="a2fd8-342">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2fd8-342">Notes.ReadWrite.All</span></span>

<span data-ttu-id="a2fd8-343">Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2fd8-343">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="a2fd8-344">Confira também</span><span class="sxs-lookup"><span data-stu-id="a2fd8-344">See also</span></span>

- [<span data-ttu-id="a2fd8-345">Adicionar imagens e arquivos</span><span class="sxs-lookup"><span data-stu-id="a2fd8-345">Add images and files</span></span>](onenote-images-files.md)
- [<span data-ttu-id="a2fd8-346">Integrar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="a2fd8-346">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="a2fd8-347">Blog de desenvolvedor do OneNote</span><span class="sxs-lookup"><span data-stu-id="a2fd8-347">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="a2fd8-348">Perguntas de desenvolvimento do OneNote no Microsoft Q&A</span><span class="sxs-lookup"><span data-stu-id="a2fd8-348">OneNote development questions on Microsoft Q&A</span></span>](/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="a2fd8-349">Repositórios do OneNote no GitHub</span><span class="sxs-lookup"><span data-stu-id="a2fd8-349">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)