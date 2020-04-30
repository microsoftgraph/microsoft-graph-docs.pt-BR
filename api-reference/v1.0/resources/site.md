---
author: JeremyKelley
ms.author: JeremyKelley
title: Recurso do site
description: O recurso do site fornece metadados e relações para um site do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a4e67deb63850bdc938f72f5e517bc28a5a8df03
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934854"
---
# <a name="site-resource"></a><span data-ttu-id="e4f2f-103">Recurso do site</span><span class="sxs-lookup"><span data-stu-id="e4f2f-103">site resource</span></span>

<span data-ttu-id="e4f2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4f2f-105">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="e4f2f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e4f2f-106">Methods</span></span>

| <span data-ttu-id="e4f2f-107">Método</span><span class="sxs-lookup"><span data-stu-id="e4f2f-107">Method</span></span>                | <span data-ttu-id="e4f2f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e4f2f-108">Return type</span></span> | <span data-ttu-id="e4f2f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4f2f-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="e4f2f-110">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-110">[Get root site][]</span></span>        | <span data-ttu-id="e4f2f-111">site</span><span class="sxs-lookup"><span data-stu-id="e4f2f-111">site</span></span> | <span data-ttu-id="e4f2f-112">Acessar o site raiz do SharePoint dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="e4f2f-113">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-113">[Get site][]</span></span>             | <span data-ttu-id="e4f2f-114">site</span><span class="sxs-lookup"><span data-stu-id="e4f2f-114">site</span></span> | <span data-ttu-id="e4f2f-115">Acessar um site do sharePoint usando o siteId.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="e4f2f-116">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-116">[Get site by path][]</span></span>     | <span data-ttu-id="e4f2f-117">site</span><span class="sxs-lookup"><span data-stu-id="e4f2f-117">site</span></span> | <span data-ttu-id="e4f2f-118">Acessar o site raiz do SharePoint com um caminho relativo.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="e4f2f-119">[Obter site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-119">[Get site for a group][]</span></span> | <span data-ttu-id="e4f2f-120">site</span><span class="sxs-lookup"><span data-stu-id="e4f2f-120">site</span></span> | <span data-ttu-id="e4f2f-121">Acessar o site de equipe de um grupo.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-121">Access the team site for a group.</span></span>
| <span data-ttu-id="e4f2f-122">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-122">[Get analytics][]</span></span>              | <span data-ttu-id="e4f2f-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-123">[itemAnalytics][]</span></span> | <span data-ttu-id="e4f2f-124">Obter análises para este recurso.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="e4f2f-125">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-125">[Get activities by interval][]</span></span> | <span data-ttu-id="e4f2f-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-126">[itemActivityStat][]</span></span> | <span data-ttu-id="e4f2f-127">Obter uma coleção de **itemActivityStats** dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="e4f2f-128">[Pesquisar sites][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-128">[Search for sites][]</span></span>     | <span data-ttu-id="e4f2f-129">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="e4f2f-129">collection of site</span></span> | <span data-ttu-id="e4f2f-130">Pesquise num locatário do SharePoint por sites que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>
| <span data-ttu-id="e4f2f-131">[Seguir site][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-131">[Follow site][]</span></span>          | <span data-ttu-id="e4f2f-132">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="e4f2f-132">collection of site</span></span> | <span data-ttu-id="e4f2f-133">Seguir um ou vários sites de usuário.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-133">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="e4f2f-134">[Deixar de seguir site][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-134">[Unfollow site][]</span></span>        | <span data-ttu-id="e4f2f-135">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="e4f2f-135">collection of site</span></span> | <span data-ttu-id="e4f2f-136">Seguir um ou vários sites de usuário.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-136">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="e4f2f-137">[Listar sites seguidos][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-137">[List followed sites][]</span></span>  | <span data-ttu-id="e4f2f-138">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="e4f2f-138">collection of site</span></span> | <span data-ttu-id="e4f2f-139">Liste os sites que foram seguidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-139">List the sites that have been followed by the signed in user.</span></span>

[Obter site]: ../api/site-get.md
[Get site]: ../api/site-get.md
[Obter site raiz]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[Obter site por caminho]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[Obter o site para um grupo]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[Pesquisar sites]: ../api/site-search.md
[Search for sites]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md
[Seguir site]: ../api/site-follow.md
[Follow site]: ../api/site-follow.md
[Deixar de seguir site]: ../api/site-unfollow.md
[Unfollow site]: ../api/site-unfollow.md
[Listar sites seguidos]: ../api/sites-list-followed.md
[List followed sites]: ../api/sites-list-followed.md

## <a name="properties"></a><span data-ttu-id="e4f2f-151">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4f2f-151">Properties</span></span>

| <span data-ttu-id="e4f2f-152">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4f2f-152">Property</span></span>            | <span data-ttu-id="e4f2f-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4f2f-153">Type</span></span>                                | <span data-ttu-id="e4f2f-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4f2f-154">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e4f2f-155">**id**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-155">**id**</span></span>                   | <span data-ttu-id="e4f2f-156">string</span><span class="sxs-lookup"><span data-stu-id="e4f2f-156">string</span></span>                              | <span data-ttu-id="e4f2f-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="e4f2f-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-159">**createdDateTime**</span></span>      | <span data-ttu-id="e4f2f-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f2f-160">DateTimeOffset</span></span>                      | <span data-ttu-id="e4f2f-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="e4f2f-163">**description**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-163">**description**</span></span>          | <span data-ttu-id="e4f2f-164">string</span><span class="sxs-lookup"><span data-stu-id="e4f2f-164">string</span></span>                              | <span data-ttu-id="e4f2f-165">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-165">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="e4f2f-166">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-166">**displayName**</span></span>          | <span data-ttu-id="e4f2f-167">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4f2f-167">string</span></span>                              | <span data-ttu-id="e4f2f-p103">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="e4f2f-170">**eTag**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-170">**eTag**</span></span>                 | <span data-ttu-id="e4f2f-171">string</span><span class="sxs-lookup"><span data-stu-id="e4f2f-171">string</span></span>                              | <span data-ttu-id="e4f2f-p104">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="e4f2f-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="e4f2f-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f2f-175">DateTimeOffset</span></span>                      | <span data-ttu-id="e4f2f-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="e4f2f-178">**name**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-178">**name**</span></span>                 | <span data-ttu-id="e4f2f-179">string</span><span class="sxs-lookup"><span data-stu-id="e4f2f-179">string</span></span>                              | <span data-ttu-id="e4f2f-180">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-180">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="e4f2f-181">**root**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-181">**root**</span></span>                 | [<span data-ttu-id="e4f2f-182">root</span><span class="sxs-lookup"><span data-stu-id="e4f2f-182">root</span></span>](root.md)                     | <span data-ttu-id="e4f2f-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="e4f2f-185">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-185">**sharepointIds**</span></span>        | [<span data-ttu-id="e4f2f-186">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="e4f2f-186">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="e4f2f-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="e4f2f-189">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-189">**siteCollection**</span></span>       | [<span data-ttu-id="e4f2f-190">siteCollection</span><span class="sxs-lookup"><span data-stu-id="e4f2f-190">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="e4f2f-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="e4f2f-194">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-194">**webUrl**</span></span>               | <span data-ttu-id="e4f2f-195">string (url)</span><span class="sxs-lookup"><span data-stu-id="e4f2f-195">string (url)</span></span>                        | <span data-ttu-id="e4f2f-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

### <a name="id-property"></a><span data-ttu-id="e4f2f-198">propriedade do id</span><span class="sxs-lookup"><span data-stu-id="e4f2f-198">id property</span></span>
<span data-ttu-id="e4f2f-199">Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="e4f2f-199">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="e4f2f-200">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="e4f2f-200">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="e4f2f-201">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="e4f2f-201">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="e4f2f-202">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="e4f2f-202">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="e4f2f-203">O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:</span><span class="sxs-lookup"><span data-stu-id="e4f2f-203">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="e4f2f-204">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-204">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="e4f2f-205">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-205">`/groups/{group-id}/sites/root`: The group's team site.</span></span>
  
## <a name="relationships"></a><span data-ttu-id="e4f2f-206">Relações</span><span class="sxs-lookup"><span data-stu-id="e4f2f-206">Relationships</span></span>

| <span data-ttu-id="e4f2f-207">Relação</span><span class="sxs-lookup"><span data-stu-id="e4f2f-207">Relationship</span></span>      | <span data-ttu-id="e4f2f-208">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4f2f-208">Type</span></span>                             | <span data-ttu-id="e4f2f-209">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4f2f-209">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="e4f2f-210">**analytics**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-210">**analytics**</span></span>     | <span data-ttu-id="e4f2f-211">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="e4f2f-211">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="e4f2f-212">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-212">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="e4f2f-213">**columns**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-213">**columns**</span></span>       | <span data-ttu-id="e4f2f-214">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="e4f2f-214">Collection([columnDefinition][])</span></span> | <span data-ttu-id="e4f2f-215">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-215">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="e4f2f-216">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-216">**contentTypes**</span></span>  | <span data-ttu-id="e4f2f-217">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="e4f2f-217">Collection([contentType][])</span></span>      | <span data-ttu-id="e4f2f-218">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-218">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="e4f2f-219">**drive**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-219">**drive**</span></span>         | <span data-ttu-id="e4f2f-220">[drive][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-220">[drive][]</span></span>                        | <span data-ttu-id="e4f2f-221">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-221">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="e4f2f-222">**drives**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-222">**drives**</span></span>        | <span data-ttu-id="e4f2f-223">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="e4f2f-223">Collection([drive][])</span></span>            | <span data-ttu-id="e4f2f-224">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-224">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="e4f2f-225">**items**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-225">**items**</span></span>         | <span data-ttu-id="e4f2f-226">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="e4f2f-226">Collection([baseItem][])</span></span>         | <span data-ttu-id="e4f2f-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="e4f2f-229">**lists**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-229">**lists**</span></span>         | <span data-ttu-id="e4f2f-230">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="e4f2f-230">Collection([list][])</span></span>             | <span data-ttu-id="e4f2f-231">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-231">The collection of lists under this site.</span></span>
| <span data-ttu-id="e4f2f-232">**sites**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-232">**sites**</span></span>         | <span data-ttu-id="e4f2f-233">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="e4f2f-233">Collection([site][])</span></span>             | <span data-ttu-id="e4f2f-234">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-234">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="e4f2f-235">**onenote**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-235">**onenote**</span></span>       | <span data-ttu-id="e4f2f-236">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="e4f2f-236">[onenote][]</span></span>                      | <span data-ttu-id="e4f2f-237">Chama o serviço OneNote para operações relacionadas ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-237">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="e4f2f-246">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4f2f-246">JSON representation</span></span>

<span data-ttu-id="e4f2f-247">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-247">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="e4f2f-248">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="e4f2f-248">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
