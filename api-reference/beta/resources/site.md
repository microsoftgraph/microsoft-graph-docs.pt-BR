---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f2386228c3758cc15d9c270f0da32608e4f2b901
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683500"
---
# <a name="site-resource-type"></a><span data-ttu-id="6842b-102">tipo de recurso do site</span><span class="sxs-lookup"><span data-stu-id="6842b-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6842b-103">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6842b-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="6842b-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="6842b-104">Methods</span></span>

| <span data-ttu-id="6842b-105">Método</span><span class="sxs-lookup"><span data-stu-id="6842b-105">Method</span></span>                         | <span data-ttu-id="6842b-106">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="6842b-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="6842b-107">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="6842b-107">[Get root site][]</span></span>              | <span data-ttu-id="6842b-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="6842b-108">GET /sites/root</span></span>
| <span data-ttu-id="6842b-109">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="6842b-109">[Get site][]</span></span>                   | <span data-ttu-id="6842b-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="6842b-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="6842b-111">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="6842b-111">[Get site by path][]</span></span>           | <span data-ttu-id="6842b-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="6842b-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="6842b-113">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="6842b-113">[Get site for a group][]</span></span>       | <span data-ttu-id="6842b-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="6842b-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="6842b-115">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="6842b-115">[Get analytics][]</span></span>              | <span data-ttu-id="6842b-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="6842b-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="6842b-117">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="6842b-117">[Get activities by interval][]</span></span> | <span data-ttu-id="6842b-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="6842b-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="6842b-119">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="6842b-119">[List pages][]</span></span>                 | <span data-ttu-id="6842b-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="6842b-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="6842b-121">[Lista sites raiz][]</span><span class="sxs-lookup"><span data-stu-id="6842b-121">[List root sites][]</span></span>            | <span data-ttu-id="6842b-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="6842b-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="6842b-123">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="6842b-123">[Search for sites][]</span></span>           | <span data-ttu-id="6842b-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="6842b-124">GET /sites?search={query}</span></span>
| <span data-ttu-id="6842b-125">[Seguir Site][]</span><span class="sxs-lookup"><span data-stu-id="6842b-125">[Follow Site][]</span></span>                | <span data-ttu-id="6842b-126">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="6842b-126">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="6842b-127">[Deixar de Seguir Site][]</span><span class="sxs-lookup"><span data-stu-id="6842b-127">[Unfollow Site][]</span></span>              | <span data-ttu-id="6842b-128">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="6842b-128">POST /users/{user-id}/followedSites/remove</span></span>

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


## <a name="properties"></a><span data-ttu-id="6842b-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6842b-140">Properties</span></span>

| <span data-ttu-id="6842b-141">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6842b-141">Property name</span></span>            | <span data-ttu-id="6842b-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="6842b-142">Type</span></span>               | <span data-ttu-id="6842b-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="6842b-143">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="6842b-144">**id**</span><span class="sxs-lookup"><span data-stu-id="6842b-144">**id**</span></span>                   | <span data-ttu-id="6842b-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6842b-145">string</span></span>             | <span data-ttu-id="6842b-146">O [identificador exclusivo](#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="6842b-146">The unique identifier of the item.</span></span> <span data-ttu-id="6842b-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6842b-147">Read-only.</span></span>
| <span data-ttu-id="6842b-148">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="6842b-148">**createdDateTime**</span></span>      | <span data-ttu-id="6842b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6842b-149">DateTimeOffset</span></span>     | <span data-ttu-id="6842b-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6842b-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="6842b-152">**description**</span><span class="sxs-lookup"><span data-stu-id="6842b-152">**description**</span></span>          | <span data-ttu-id="6842b-153">string</span><span class="sxs-lookup"><span data-stu-id="6842b-153">string</span></span>             | <span data-ttu-id="6842b-154">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="6842b-154">The descriptive text for the site.</span></span>
| <span data-ttu-id="6842b-155">**eTag**</span><span class="sxs-lookup"><span data-stu-id="6842b-155">**eTag**</span></span>                 | <span data-ttu-id="6842b-156">string</span><span class="sxs-lookup"><span data-stu-id="6842b-156">string</span></span>             | <span data-ttu-id="6842b-p103">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6842b-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="6842b-159">**displayName**</span><span class="sxs-lookup"><span data-stu-id="6842b-159">**displayName**</span></span>          | <span data-ttu-id="6842b-160">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6842b-160">string</span></span>             | <span data-ttu-id="6842b-p104">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6842b-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="6842b-163">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="6842b-163">**lastModifiedDateTime**</span></span> | <span data-ttu-id="6842b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6842b-164">DateTimeOffset</span></span>     | <span data-ttu-id="6842b-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6842b-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6842b-167">**name**</span><span class="sxs-lookup"><span data-stu-id="6842b-167">**name**</span></span>                 | <span data-ttu-id="6842b-168">string</span><span class="sxs-lookup"><span data-stu-id="6842b-168">string</span></span>             | <span data-ttu-id="6842b-169">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="6842b-169">The name / title of the item.</span></span>
| <span data-ttu-id="6842b-170">**root**</span><span class="sxs-lookup"><span data-stu-id="6842b-170">**root**</span></span>                 | <span data-ttu-id="6842b-171">[root][]</span><span class="sxs-lookup"><span data-stu-id="6842b-171">[root][]</span></span>           | <span data-ttu-id="6842b-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6842b-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="6842b-174">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="6842b-174">**sharepointIds**</span></span>        | <span data-ttu-id="6842b-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="6842b-175">[sharepointIds][]</span></span>  | <span data-ttu-id="6842b-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6842b-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="6842b-178">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="6842b-178">**siteCollection**</span></span>       | <span data-ttu-id="6842b-179">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="6842b-179">[siteCollection][]</span></span> | <span data-ttu-id="6842b-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6842b-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="6842b-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="6842b-183">**webUrl**</span></span>               | <span data-ttu-id="6842b-184">string (url)</span><span class="sxs-lookup"><span data-stu-id="6842b-184">string (url)</span></span>       | <span data-ttu-id="6842b-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6842b-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="6842b-187">propriedade do id</span><span class="sxs-lookup"><span data-stu-id="6842b-187">Id property</span></span>
<span data-ttu-id="6842b-188">Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="6842b-188">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>
* <span data-ttu-id="6842b-189">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="6842b-189">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="6842b-190">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="6842b-190">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="6842b-191">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="6842b-191">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="6842b-192">O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:</span><span class="sxs-lookup"><span data-stu-id="6842b-192">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="6842b-193">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="6842b-193">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="6842b-194">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="6842b-194">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="6842b-195">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="6842b-195">Relationships</span></span>

| <span data-ttu-id="6842b-196">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="6842b-196">Relationship name</span></span> | <span data-ttu-id="6842b-197">Tipo</span><span class="sxs-lookup"><span data-stu-id="6842b-197">Type</span></span>                             | <span data-ttu-id="6842b-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="6842b-198">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="6842b-199">**analytics**</span><span class="sxs-lookup"><span data-stu-id="6842b-199">**analytics**</span></span>     | <span data-ttu-id="6842b-200">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="6842b-200">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="6842b-201">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="6842b-201">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="6842b-202">**columns**</span><span class="sxs-lookup"><span data-stu-id="6842b-202">**columns**</span></span>       | <span data-ttu-id="6842b-203">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="6842b-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="6842b-204">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="6842b-204">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="6842b-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="6842b-205">**contentTypes**</span></span>  | <span data-ttu-id="6842b-206">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="6842b-206">Collection([contentType][])</span></span>      | <span data-ttu-id="6842b-207">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="6842b-207">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="6842b-208">**drive**</span><span class="sxs-lookup"><span data-stu-id="6842b-208">**drive**</span></span>         | <span data-ttu-id="6842b-209">[drive][]</span><span class="sxs-lookup"><span data-stu-id="6842b-209">[drive][]</span></span>                        | <span data-ttu-id="6842b-210">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="6842b-210">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="6842b-211">**drives**</span><span class="sxs-lookup"><span data-stu-id="6842b-211">**drives**</span></span>        | <span data-ttu-id="6842b-212">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="6842b-212">Collection([drive][])</span></span>            | <span data-ttu-id="6842b-213">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="6842b-213">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="6842b-214">**items**</span><span class="sxs-lookup"><span data-stu-id="6842b-214">**items**</span></span>         | <span data-ttu-id="6842b-215">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="6842b-215">Collection([baseItem][])</span></span>         | <span data-ttu-id="6842b-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="6842b-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="6842b-218">**lists**</span><span class="sxs-lookup"><span data-stu-id="6842b-218">**lists**</span></span>         | <span data-ttu-id="6842b-219">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="6842b-219">Collection([list][])</span></span>             | <span data-ttu-id="6842b-220">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="6842b-220">The collection of lists under this site.</span></span>
| <span data-ttu-id="6842b-221">**pages**</span><span class="sxs-lookup"><span data-stu-id="6842b-221">**pages**</span></span>         | <span data-ttu-id="6842b-222">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="6842b-222">Collection([sitePage][])</span></span>         | <span data-ttu-id="6842b-223">O conjunto de páginas na lista SitePages no site.</span><span class="sxs-lookup"><span data-stu-id="6842b-223">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="6842b-224">**sites**</span><span class="sxs-lookup"><span data-stu-id="6842b-224">**sites**</span></span>         | <span data-ttu-id="6842b-225">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="6842b-225">Collection([site][])</span></span>             | <span data-ttu-id="6842b-226">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="6842b-226">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="6842b-238">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6842b-238">JSON representation</span></span>

<span data-ttu-id="6842b-239">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="6842b-239">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="6842b-240">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="6842b-240">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
