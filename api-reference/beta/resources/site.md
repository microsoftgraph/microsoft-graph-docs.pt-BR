---
author: JeremyKelley
description: O recurso site fornece metadados e relações para um site do SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 691f91b63fdff583476c5308f4b8370a563120a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008352"
---
# <a name="site-resource-type"></a><span data-ttu-id="ca6b3-103">tipo de recurso do site</span><span class="sxs-lookup"><span data-stu-id="ca6b3-103">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca6b3-104">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-104">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="ca6b3-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ca6b3-105">Methods</span></span>

| <span data-ttu-id="ca6b3-106">Método</span><span class="sxs-lookup"><span data-stu-id="ca6b3-106">Method</span></span>                         | <span data-ttu-id="ca6b3-107">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="ca6b3-107">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="ca6b3-108">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-108">[Get root site][]</span></span>              | <span data-ttu-id="ca6b3-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="ca6b3-109">GET /sites/root</span></span>
| <span data-ttu-id="ca6b3-110">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-110">[Get site][]</span></span>                   | <span data-ttu-id="ca6b3-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="ca6b3-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="ca6b3-112">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-112">[Get site by path][]</span></span>           | <span data-ttu-id="ca6b3-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="ca6b3-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="ca6b3-114">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-114">[Get site for a group][]</span></span>       | <span data-ttu-id="ca6b3-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="ca6b3-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="ca6b3-116">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-116">[Get analytics][]</span></span>              | <span data-ttu-id="ca6b3-117">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="ca6b3-117">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="ca6b3-118">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-118">[Get activities by interval][]</span></span> | <span data-ttu-id="ca6b3-119">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="ca6b3-119">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="ca6b3-120">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-120">[List pages][]</span></span>                 | <span data-ttu-id="ca6b3-121">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="ca6b3-121">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="ca6b3-122">[Lista sites raiz][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-122">[List root sites][]</span></span>            | <span data-ttu-id="ca6b3-123">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="ca6b3-123">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="ca6b3-124">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-124">[Search for sites][]</span></span>           | <span data-ttu-id="ca6b3-125">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="ca6b3-125">GET /sites?search={query}</span></span>
| <span data-ttu-id="ca6b3-126">[Seguir Site][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-126">[Follow Site][]</span></span>                | <span data-ttu-id="ca6b3-127">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="ca6b3-127">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="ca6b3-128">[Deixar de Seguir Site][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-128">[Unfollow Site][]</span></span>              | <span data-ttu-id="ca6b3-129">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="ca6b3-129">POST /users/{user-id}/followedSites/remove</span></span>

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


## <a name="properties"></a><span data-ttu-id="ca6b3-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca6b3-141">Properties</span></span>

| <span data-ttu-id="ca6b3-142">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ca6b3-142">Property name</span></span>            | <span data-ttu-id="ca6b3-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca6b3-143">Type</span></span>               | <span data-ttu-id="ca6b3-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca6b3-144">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="ca6b3-145">**id**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-145">**id**</span></span>                   | <span data-ttu-id="ca6b3-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca6b3-146">string</span></span>             | <span data-ttu-id="ca6b3-147">O [identificador exclusivo](#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-147">The unique identifier of the item.</span></span> <span data-ttu-id="ca6b3-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-148">Read-only.</span></span>
| <span data-ttu-id="ca6b3-149">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-149">**createdDateTime**</span></span>      | <span data-ttu-id="ca6b3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca6b3-150">DateTimeOffset</span></span>     | <span data-ttu-id="ca6b3-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ca6b3-153">**description**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-153">**description**</span></span>          | <span data-ttu-id="ca6b3-154">string</span><span class="sxs-lookup"><span data-stu-id="ca6b3-154">string</span></span>             | <span data-ttu-id="ca6b3-155">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-155">The descriptive text for the site.</span></span>
| <span data-ttu-id="ca6b3-156">**eTag**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-156">**eTag**</span></span>                 | <span data-ttu-id="ca6b3-157">string</span><span class="sxs-lookup"><span data-stu-id="ca6b3-157">string</span></span>             | <span data-ttu-id="ca6b3-p103">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="ca6b3-160">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-160">**displayName**</span></span>          | <span data-ttu-id="ca6b3-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca6b3-161">string</span></span>             | <span data-ttu-id="ca6b3-p104">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="ca6b3-164">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-164">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ca6b3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca6b3-165">DateTimeOffset</span></span>     | <span data-ttu-id="ca6b3-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ca6b3-168">**name**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-168">**name**</span></span>                 | <span data-ttu-id="ca6b3-169">string</span><span class="sxs-lookup"><span data-stu-id="ca6b3-169">string</span></span>             | <span data-ttu-id="ca6b3-170">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-170">The name / title of the item.</span></span>
| <span data-ttu-id="ca6b3-171">**root**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-171">**root**</span></span>                 | <span data-ttu-id="ca6b3-172">[root][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-172">[root][]</span></span>           | <span data-ttu-id="ca6b3-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="ca6b3-175">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-175">**sharepointIds**</span></span>        | <span data-ttu-id="ca6b3-176">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-176">[sharepointIds][]</span></span>  | <span data-ttu-id="ca6b3-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ca6b3-179">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-179">**siteCollection**</span></span>       | <span data-ttu-id="ca6b3-180">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-180">[siteCollection][]</span></span> | <span data-ttu-id="ca6b3-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="ca6b3-184">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-184">**webUrl**</span></span>               | <span data-ttu-id="ca6b3-185">string (url)</span><span class="sxs-lookup"><span data-stu-id="ca6b3-185">string (url)</span></span>       | <span data-ttu-id="ca6b3-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="ca6b3-188">propriedade do id</span><span class="sxs-lookup"><span data-stu-id="ca6b3-188">Id property</span></span>
<span data-ttu-id="ca6b3-189">Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="ca6b3-189">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>
* <span data-ttu-id="ca6b3-190">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="ca6b3-190">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="ca6b3-191">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="ca6b3-191">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="ca6b3-192">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="ca6b3-192">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="ca6b3-193">O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:</span><span class="sxs-lookup"><span data-stu-id="ca6b3-193">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="ca6b3-194">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-194">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="ca6b3-195">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-195">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="ca6b3-196">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ca6b3-196">Relationships</span></span>

| <span data-ttu-id="ca6b3-197">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="ca6b3-197">Relationship name</span></span> | <span data-ttu-id="ca6b3-198">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca6b3-198">Type</span></span>                             | <span data-ttu-id="ca6b3-199">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca6b3-199">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="ca6b3-200">**analytics**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-200">**analytics**</span></span>     | <span data-ttu-id="ca6b3-201">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="ca6b3-201">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="ca6b3-202">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-202">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="ca6b3-203">**columns**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-203">**columns**</span></span>       | <span data-ttu-id="ca6b3-204">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ca6b3-204">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ca6b3-205">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-205">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="ca6b3-206">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-206">**contentTypes**</span></span>  | <span data-ttu-id="ca6b3-207">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ca6b3-207">Collection([contentType][])</span></span>      | <span data-ttu-id="ca6b3-208">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-208">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="ca6b3-209">**drive**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-209">**drive**</span></span>         | <span data-ttu-id="ca6b3-210">[drive][]</span><span class="sxs-lookup"><span data-stu-id="ca6b3-210">[drive][]</span></span>                        | <span data-ttu-id="ca6b3-211">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-211">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="ca6b3-212">**drives**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-212">**drives**</span></span>        | <span data-ttu-id="ca6b3-213">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="ca6b3-213">Collection([drive][])</span></span>            | <span data-ttu-id="ca6b3-214">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-214">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="ca6b3-215">**items**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-215">**items**</span></span>         | <span data-ttu-id="ca6b3-216">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="ca6b3-216">Collection([baseItem][])</span></span>         | <span data-ttu-id="ca6b3-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="ca6b3-219">**lists**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-219">**lists**</span></span>         | <span data-ttu-id="ca6b3-220">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="ca6b3-220">Collection([list][])</span></span>             | <span data-ttu-id="ca6b3-221">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-221">The collection of lists under this site.</span></span>
| <span data-ttu-id="ca6b3-222">**pages**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-222">**pages**</span></span>         | <span data-ttu-id="ca6b3-223">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="ca6b3-223">Collection([sitePage][])</span></span>         | <span data-ttu-id="ca6b3-224">O conjunto de páginas na lista SitePages no site.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-224">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="ca6b3-225">**sites**</span><span class="sxs-lookup"><span data-stu-id="ca6b3-225">**sites**</span></span>         | <span data-ttu-id="ca6b3-226">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="ca6b3-226">Collection([site][])</span></span>             | <span data-ttu-id="ca6b3-227">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-227">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="ca6b3-239">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca6b3-239">JSON representation</span></span>

<span data-ttu-id="ca6b3-240">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-240">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="ca6b3-241">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="ca6b3-241">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
