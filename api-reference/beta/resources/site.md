---
author: JeremyKelley
description: O recurso site fornece metadados e relações para um site do SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: fc6a7472da2676d0266d964b7bdddee976d5ac8c
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864221"
---
# <a name="site-resource-type"></a><span data-ttu-id="b377f-103">tipo de recurso do site</span><span class="sxs-lookup"><span data-stu-id="b377f-103">site resource type</span></span>

<span data-ttu-id="b377f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b377f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b377f-105">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b377f-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="b377f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b377f-106">Methods</span></span>

| <span data-ttu-id="b377f-107">Método</span><span class="sxs-lookup"><span data-stu-id="b377f-107">Method</span></span>                         | <span data-ttu-id="b377f-108">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="b377f-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="b377f-109">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="b377f-109">[Get root site][]</span></span>              | <span data-ttu-id="b377f-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="b377f-110">GET /sites/root</span></span>
| <span data-ttu-id="b377f-111">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="b377f-111">[Get site][]</span></span>                   | <span data-ttu-id="b377f-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="b377f-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="b377f-113">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="b377f-113">[Get site by path][]</span></span>           | <span data-ttu-id="b377f-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="b377f-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="b377f-115">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="b377f-115">[Get site for a group][]</span></span>       | <span data-ttu-id="b377f-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="b377f-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="b377f-117">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="b377f-117">[Get analytics][]</span></span>              | <span data-ttu-id="b377f-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="b377f-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="b377f-119">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="b377f-119">[Get activities by interval][]</span></span> | <span data-ttu-id="b377f-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="b377f-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="b377f-121">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="b377f-121">[List pages][]</span></span>                 | <span data-ttu-id="b377f-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="b377f-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="b377f-123">[Lista sites raiz][]</span><span class="sxs-lookup"><span data-stu-id="b377f-123">[List root sites][]</span></span>            | <span data-ttu-id="b377f-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="b377f-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="b377f-125">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="b377f-125">[Search for sites][]</span></span>           | <span data-ttu-id="b377f-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="b377f-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="b377f-127">[Seguir site][]</span><span class="sxs-lookup"><span data-stu-id="b377f-127">[Follow site][]</span></span>                | <span data-ttu-id="b377f-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="b377f-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="b377f-129">[Deixar de seguir site][]</span><span class="sxs-lookup"><span data-stu-id="b377f-129">[Unfollow site][]</span></span>              | <span data-ttu-id="b377f-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="b377f-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="b377f-131">[Listar sites seguidos][]</span><span class="sxs-lookup"><span data-stu-id="b377f-131">[List followed sites][]</span></span>        | <span data-ttu-id="b377f-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="b377f-132">GET /me/followedSites</span></span>

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
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Listar páginas]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Lista sites raiz]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[Procurar sites]: ../api/site-search.md
[Search for sites]: ../api/site-search.md
[Seguir site]: ../api/site-follow.md
[Follow site]: ../api/site-follow.md
[Deixar de seguir site]: ../api/site-unfollow.md
[Unfollow site]: ../api/site-unfollow.md
[Listar sites seguidos]: ../api/sites-list-followed.md
[List followed sites]: ../api/sites-list-followed.md


## <a name="properties"></a><span data-ttu-id="b377f-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b377f-145">Properties</span></span>

| <span data-ttu-id="b377f-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b377f-146">Property name</span></span>            | <span data-ttu-id="b377f-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="b377f-147">Type</span></span>               | <span data-ttu-id="b377f-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="b377f-148">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="b377f-149">**id**</span><span class="sxs-lookup"><span data-stu-id="b377f-149">**id**</span></span>                   | <span data-ttu-id="b377f-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b377f-150">string</span></span>             | <span data-ttu-id="b377f-151">O [identificador exclusivo](#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="b377f-151">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="b377f-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b377f-152">Read-only.</span></span>
| <span data-ttu-id="b377f-153">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="b377f-153">**createdDateTime**</span></span>      | <span data-ttu-id="b377f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b377f-154">DateTimeOffset</span></span>     | <span data-ttu-id="b377f-155">The date and time the item was created.</span><span class="sxs-lookup"><span data-stu-id="b377f-155">The date and time the item was created.</span></span> <span data-ttu-id="b377f-156">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b377f-156">Read-only.</span></span>
| <span data-ttu-id="b377f-157">**description**</span><span class="sxs-lookup"><span data-stu-id="b377f-157">**description**</span></span>          | <span data-ttu-id="b377f-158">string</span><span class="sxs-lookup"><span data-stu-id="b377f-158">string</span></span>             | <span data-ttu-id="b377f-159">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="b377f-159">The descriptive text for the site.</span></span>
| <span data-ttu-id="b377f-160">**eTag**</span><span class="sxs-lookup"><span data-stu-id="b377f-160">**eTag**</span></span>                 | <span data-ttu-id="b377f-161">string</span><span class="sxs-lookup"><span data-stu-id="b377f-161">string</span></span>             | <span data-ttu-id="b377f-162">ETag for the item.</span><span class="sxs-lookup"><span data-stu-id="b377f-162">ETag for the item.</span></span> <span data-ttu-id="b377f-163">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b377f-163">Read-only.</span></span>                                                                  |
| <span data-ttu-id="b377f-164">**displayName**</span><span class="sxs-lookup"><span data-stu-id="b377f-164">**displayName**</span></span>          | <span data-ttu-id="b377f-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b377f-165">string</span></span>             | <span data-ttu-id="b377f-166">The full title for the site.</span><span class="sxs-lookup"><span data-stu-id="b377f-166">The full title for the site.</span></span> <span data-ttu-id="b377f-167">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b377f-167">Read-only.</span></span>
| <span data-ttu-id="b377f-168">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b377f-168">**lastModifiedDateTime**</span></span> | <span data-ttu-id="b377f-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b377f-169">DateTimeOffset</span></span>     | <span data-ttu-id="b377f-170">The date and time the item was last modified.</span><span class="sxs-lookup"><span data-stu-id="b377f-170">The date and time the item was last modified.</span></span> <span data-ttu-id="b377f-171">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b377f-171">Read-only.</span></span>
| <span data-ttu-id="b377f-172">**name**</span><span class="sxs-lookup"><span data-stu-id="b377f-172">**name**</span></span>                 | <span data-ttu-id="b377f-173">string</span><span class="sxs-lookup"><span data-stu-id="b377f-173">string</span></span>             | <span data-ttu-id="b377f-174">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="b377f-174">The name / title of the item.</span></span>
| <span data-ttu-id="b377f-175">**root**</span><span class="sxs-lookup"><span data-stu-id="b377f-175">**root**</span></span>                 | <span data-ttu-id="b377f-176">[root][]</span><span class="sxs-lookup"><span data-stu-id="b377f-176">[root][]</span></span>           | <span data-ttu-id="b377f-177">If present, indicates that this is the root site in the site collection.</span><span class="sxs-lookup"><span data-stu-id="b377f-177">If present, indicates that this is the root site in the site collection.</span></span> <span data-ttu-id="b377f-178">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b377f-178">Read-only.</span></span>
| <span data-ttu-id="b377f-179">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="b377f-179">**sharepointIds**</span></span>        | <span data-ttu-id="b377f-180">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b377f-180">[sharepointIds][]</span></span>  | <span data-ttu-id="b377f-181">Returns identifiers useful for SharePoint REST compatibility.</span><span class="sxs-lookup"><span data-stu-id="b377f-181">Returns identifiers useful for SharePoint REST compatibility.</span></span> <span data-ttu-id="b377f-182">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b377f-182">Read-only.</span></span>
| <span data-ttu-id="b377f-183">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="b377f-183">**siteCollection**</span></span>       | <span data-ttu-id="b377f-184">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="b377f-184">[siteCollection][]</span></span> | <span data-ttu-id="b377f-185">Provides details about the site's site collection.</span><span class="sxs-lookup"><span data-stu-id="b377f-185">Provides details about the site's site collection.</span></span> <span data-ttu-id="b377f-186">Available only on the root site.</span><span class="sxs-lookup"><span data-stu-id="b377f-186">Available only on the root site.</span></span> <span data-ttu-id="b377f-187">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b377f-187">Read-only.</span></span>
| <span data-ttu-id="b377f-188">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="b377f-188">**webUrl**</span></span>               | <span data-ttu-id="b377f-189">string (url)</span><span class="sxs-lookup"><span data-stu-id="b377f-189">string (url)</span></span>       | <span data-ttu-id="b377f-190">URL that displays the item in the browser.</span><span class="sxs-lookup"><span data-stu-id="b377f-190">URL that displays the item in the browser.</span></span> <span data-ttu-id="b377f-191">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b377f-191">Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="b377f-192">propriedade do id</span><span class="sxs-lookup"><span data-stu-id="b377f-192">id property</span></span>
<span data-ttu-id="b377f-193">Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="b377f-193">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="b377f-194">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="b377f-194">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="b377f-195">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="b377f-195">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="b377f-196">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="b377f-196">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="b377f-197">O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:</span><span class="sxs-lookup"><span data-stu-id="b377f-197">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="b377f-198">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="b377f-198">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="b377f-199">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="b377f-199">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="b377f-200">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="b377f-200">Relationships</span></span>

| <span data-ttu-id="b377f-201">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="b377f-201">Relationship name</span></span> | <span data-ttu-id="b377f-202">Tipo</span><span class="sxs-lookup"><span data-stu-id="b377f-202">Type</span></span>                             | <span data-ttu-id="b377f-203">Descrição</span><span class="sxs-lookup"><span data-stu-id="b377f-203">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="b377f-204">**analytics**</span><span class="sxs-lookup"><span data-stu-id="b377f-204">**analytics**</span></span>     | <span data-ttu-id="b377f-205">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="b377f-205">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="b377f-206">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="b377f-206">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="b377f-207">**columns**</span><span class="sxs-lookup"><span data-stu-id="b377f-207">**columns**</span></span>       | <span data-ttu-id="b377f-208">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="b377f-208">Collection([columnDefinition][])</span></span> | <span data-ttu-id="b377f-209">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="b377f-209">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="b377f-210">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="b377f-210">**contentTypes**</span></span>  | <span data-ttu-id="b377f-211">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="b377f-211">Collection([contentType][])</span></span>      | <span data-ttu-id="b377f-212">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="b377f-212">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="b377f-213">**drive**</span><span class="sxs-lookup"><span data-stu-id="b377f-213">**drive**</span></span>         | <span data-ttu-id="b377f-214">[drive][]</span><span class="sxs-lookup"><span data-stu-id="b377f-214">[drive][]</span></span>                        | <span data-ttu-id="b377f-215">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="b377f-215">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="b377f-216">**drives**</span><span class="sxs-lookup"><span data-stu-id="b377f-216">**drives**</span></span>        | <span data-ttu-id="b377f-217">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="b377f-217">Collection([drive][])</span></span>            | <span data-ttu-id="b377f-218">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="b377f-218">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="b377f-219">**items**</span><span class="sxs-lookup"><span data-stu-id="b377f-219">**items**</span></span>         | <span data-ttu-id="b377f-220">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="b377f-220">Collection([baseItem][])</span></span>         | <span data-ttu-id="b377f-221">Used to address any item contained in this site.</span><span class="sxs-lookup"><span data-stu-id="b377f-221">Used to address any item contained in this site.</span></span> <span data-ttu-id="b377f-222">This collection cannot be enumerated.</span><span class="sxs-lookup"><span data-stu-id="b377f-222">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="b377f-223">**lists**</span><span class="sxs-lookup"><span data-stu-id="b377f-223">**lists**</span></span>         | <span data-ttu-id="b377f-224">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="b377f-224">Collection([list][])</span></span>             | <span data-ttu-id="b377f-225">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="b377f-225">The collection of lists under this site.</span></span>
| <span data-ttu-id="b377f-226">**pages**</span><span class="sxs-lookup"><span data-stu-id="b377f-226">**pages**</span></span>         | <span data-ttu-id="b377f-227">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="b377f-227">Collection([sitePage][])</span></span>         | <span data-ttu-id="b377f-228">O conjunto de páginas na lista SitePages no site.</span><span class="sxs-lookup"><span data-stu-id="b377f-228">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="b377f-229">**sites**</span><span class="sxs-lookup"><span data-stu-id="b377f-229">**sites**</span></span>         | <span data-ttu-id="b377f-230">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="b377f-230">Collection([site][])</span></span>             | <span data-ttu-id="b377f-231">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="b377f-231">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="b377f-243">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b377f-243">JSON representation</span></span>

<span data-ttu-id="b377f-244">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="b377f-244">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="b377f-245">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="b377f-245">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": {
    "Resources/Site": "#"
  },
  "suppressions": []
}
-->
