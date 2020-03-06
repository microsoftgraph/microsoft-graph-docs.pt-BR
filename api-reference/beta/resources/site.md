---
author: JeremyKelley
description: O recurso site fornece metadados e relações para um site do SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: be567e1ba44790c54127ccee17dbb0d396f15e0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520552"
---
# <a name="site-resource-type"></a><span data-ttu-id="34144-103">tipo de recurso do site</span><span class="sxs-lookup"><span data-stu-id="34144-103">site resource type</span></span>

<span data-ttu-id="34144-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34144-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34144-105">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="34144-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="34144-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="34144-106">Methods</span></span>

| <span data-ttu-id="34144-107">Método</span><span class="sxs-lookup"><span data-stu-id="34144-107">Method</span></span>                         | <span data-ttu-id="34144-108">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="34144-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="34144-109">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="34144-109">[Get root site][]</span></span>              | <span data-ttu-id="34144-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="34144-110">GET /sites/root</span></span>
| <span data-ttu-id="34144-111">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="34144-111">[Get site][]</span></span>                   | <span data-ttu-id="34144-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="34144-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="34144-113">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="34144-113">[Get site by path][]</span></span>           | <span data-ttu-id="34144-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="34144-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="34144-115">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="34144-115">[Get site for a group][]</span></span>       | <span data-ttu-id="34144-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="34144-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="34144-117">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="34144-117">[Get analytics][]</span></span>              | <span data-ttu-id="34144-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="34144-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="34144-119">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="34144-119">[Get activities by interval][]</span></span> | <span data-ttu-id="34144-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="34144-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="34144-121">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="34144-121">[List pages][]</span></span>                 | <span data-ttu-id="34144-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="34144-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="34144-123">[Lista sites raiz][]</span><span class="sxs-lookup"><span data-stu-id="34144-123">[List root sites][]</span></span>            | <span data-ttu-id="34144-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="34144-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="34144-125">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="34144-125">[Search for sites][]</span></span>           | <span data-ttu-id="34144-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="34144-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="34144-127">[Seguir Site][]</span><span class="sxs-lookup"><span data-stu-id="34144-127">[Follow Site][]</span></span>                | <span data-ttu-id="34144-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="34144-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="34144-129">[Deixar de Seguir Site][]</span><span class="sxs-lookup"><span data-stu-id="34144-129">[Unfollow Site][]</span></span>              | <span data-ttu-id="34144-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="34144-130">POST /users/{user-id}/followedSites/remove</span></span>

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


## <a name="properties"></a><span data-ttu-id="34144-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34144-142">Properties</span></span>

| <span data-ttu-id="34144-143">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="34144-143">Property name</span></span>            | <span data-ttu-id="34144-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="34144-144">Type</span></span>               | <span data-ttu-id="34144-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="34144-145">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="34144-146">**id**</span><span class="sxs-lookup"><span data-stu-id="34144-146">**id**</span></span>                   | <span data-ttu-id="34144-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34144-147">string</span></span>             | <span data-ttu-id="34144-148">O [identificador exclusivo](#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="34144-148">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="34144-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34144-149">Read-only.</span></span>
| <span data-ttu-id="34144-150">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="34144-150">**createdDateTime**</span></span>      | <span data-ttu-id="34144-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34144-151">DateTimeOffset</span></span>     | <span data-ttu-id="34144-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34144-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="34144-154">**description**</span><span class="sxs-lookup"><span data-stu-id="34144-154">**description**</span></span>          | <span data-ttu-id="34144-155">string</span><span class="sxs-lookup"><span data-stu-id="34144-155">string</span></span>             | <span data-ttu-id="34144-156">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="34144-156">The descriptive text for the site.</span></span>
| <span data-ttu-id="34144-157">**eTag**</span><span class="sxs-lookup"><span data-stu-id="34144-157">**eTag**</span></span>                 | <span data-ttu-id="34144-158">string</span><span class="sxs-lookup"><span data-stu-id="34144-158">string</span></span>             | <span data-ttu-id="34144-p103">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34144-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="34144-161">**displayName**</span><span class="sxs-lookup"><span data-stu-id="34144-161">**displayName**</span></span>          | <span data-ttu-id="34144-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34144-162">string</span></span>             | <span data-ttu-id="34144-p104">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34144-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="34144-165">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="34144-165">**lastModifiedDateTime**</span></span> | <span data-ttu-id="34144-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34144-166">DateTimeOffset</span></span>     | <span data-ttu-id="34144-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34144-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="34144-169">**name**</span><span class="sxs-lookup"><span data-stu-id="34144-169">**name**</span></span>                 | <span data-ttu-id="34144-170">string</span><span class="sxs-lookup"><span data-stu-id="34144-170">string</span></span>             | <span data-ttu-id="34144-171">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="34144-171">The name / title of the item.</span></span>
| <span data-ttu-id="34144-172">**root**</span><span class="sxs-lookup"><span data-stu-id="34144-172">**root**</span></span>                 | <span data-ttu-id="34144-173">[root][]</span><span class="sxs-lookup"><span data-stu-id="34144-173">[root][]</span></span>           | <span data-ttu-id="34144-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34144-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="34144-176">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="34144-176">**sharepointIds**</span></span>        | <span data-ttu-id="34144-177">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="34144-177">[sharepointIds][]</span></span>  | <span data-ttu-id="34144-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34144-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="34144-180">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="34144-180">**siteCollection**</span></span>       | <span data-ttu-id="34144-181">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="34144-181">[siteCollection][]</span></span> | <span data-ttu-id="34144-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34144-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="34144-185">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="34144-185">**webUrl**</span></span>               | <span data-ttu-id="34144-186">string (url)</span><span class="sxs-lookup"><span data-stu-id="34144-186">string (url)</span></span>       | <span data-ttu-id="34144-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34144-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="34144-189">propriedade do id</span><span class="sxs-lookup"><span data-stu-id="34144-189">id property</span></span>
<span data-ttu-id="34144-190">Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="34144-190">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="34144-191">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="34144-191">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="34144-192">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="34144-192">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="34144-193">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="34144-193">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="34144-194">O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:</span><span class="sxs-lookup"><span data-stu-id="34144-194">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="34144-195">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="34144-195">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="34144-196">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="34144-196">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="34144-197">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="34144-197">Relationships</span></span>

| <span data-ttu-id="34144-198">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="34144-198">Relationship name</span></span> | <span data-ttu-id="34144-199">Tipo</span><span class="sxs-lookup"><span data-stu-id="34144-199">Type</span></span>                             | <span data-ttu-id="34144-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="34144-200">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="34144-201">**analytics**</span><span class="sxs-lookup"><span data-stu-id="34144-201">**analytics**</span></span>     | <span data-ttu-id="34144-202">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="34144-202">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="34144-203">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="34144-203">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="34144-204">**columns**</span><span class="sxs-lookup"><span data-stu-id="34144-204">**columns**</span></span>       | <span data-ttu-id="34144-205">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="34144-205">Collection([columnDefinition][])</span></span> | <span data-ttu-id="34144-206">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="34144-206">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="34144-207">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="34144-207">**contentTypes**</span></span>  | <span data-ttu-id="34144-208">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="34144-208">Collection([contentType][])</span></span>      | <span data-ttu-id="34144-209">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="34144-209">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="34144-210">**drive**</span><span class="sxs-lookup"><span data-stu-id="34144-210">**drive**</span></span>         | <span data-ttu-id="34144-211">[drive][]</span><span class="sxs-lookup"><span data-stu-id="34144-211">[drive][]</span></span>                        | <span data-ttu-id="34144-212">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="34144-212">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="34144-213">**drives**</span><span class="sxs-lookup"><span data-stu-id="34144-213">**drives**</span></span>        | <span data-ttu-id="34144-214">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="34144-214">Collection([drive][])</span></span>            | <span data-ttu-id="34144-215">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="34144-215">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="34144-216">**items**</span><span class="sxs-lookup"><span data-stu-id="34144-216">**items**</span></span>         | <span data-ttu-id="34144-217">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="34144-217">Collection([baseItem][])</span></span>         | <span data-ttu-id="34144-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="34144-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="34144-220">**lists**</span><span class="sxs-lookup"><span data-stu-id="34144-220">**lists**</span></span>         | <span data-ttu-id="34144-221">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="34144-221">Collection([list][])</span></span>             | <span data-ttu-id="34144-222">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="34144-222">The collection of lists under this site.</span></span>
| <span data-ttu-id="34144-223">**pages**</span><span class="sxs-lookup"><span data-stu-id="34144-223">**pages**</span></span>         | <span data-ttu-id="34144-224">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="34144-224">Collection([sitePage][])</span></span>         | <span data-ttu-id="34144-225">O conjunto de páginas na lista SitePages no site.</span><span class="sxs-lookup"><span data-stu-id="34144-225">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="34144-226">**sites**</span><span class="sxs-lookup"><span data-stu-id="34144-226">**sites**</span></span>         | <span data-ttu-id="34144-227">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="34144-227">Collection([site][])</span></span>             | <span data-ttu-id="34144-228">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="34144-228">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="34144-240">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34144-240">JSON representation</span></span>

<span data-ttu-id="34144-241">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="34144-241">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="34144-242">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="34144-242">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
