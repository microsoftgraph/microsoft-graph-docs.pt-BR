---
author: JeremyKelley
description: O recurso site fornece metadados e relações para um site do SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a3389737581e9c327ff48e9ff3065c399c568cb8
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934875"
---
# <a name="site-resource-type"></a><span data-ttu-id="f4465-103">tipo de recurso do site</span><span class="sxs-lookup"><span data-stu-id="f4465-103">site resource type</span></span>

<span data-ttu-id="f4465-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4465-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4465-105">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f4465-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="f4465-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f4465-106">Methods</span></span>

| <span data-ttu-id="f4465-107">Método</span><span class="sxs-lookup"><span data-stu-id="f4465-107">Method</span></span>                         | <span data-ttu-id="f4465-108">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="f4465-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="f4465-109">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="f4465-109">[Get root site][]</span></span>              | <span data-ttu-id="f4465-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="f4465-110">GET /sites/root</span></span>
| <span data-ttu-id="f4465-111">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="f4465-111">[Get site][]</span></span>                   | <span data-ttu-id="f4465-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="f4465-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="f4465-113">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="f4465-113">[Get site by path][]</span></span>           | <span data-ttu-id="f4465-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="f4465-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="f4465-115">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="f4465-115">[Get site for a group][]</span></span>       | <span data-ttu-id="f4465-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="f4465-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="f4465-117">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="f4465-117">[Get analytics][]</span></span>              | <span data-ttu-id="f4465-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="f4465-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="f4465-119">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="f4465-119">[Get activities by interval][]</span></span> | <span data-ttu-id="f4465-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="f4465-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="f4465-121">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="f4465-121">[List pages][]</span></span>                 | <span data-ttu-id="f4465-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="f4465-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="f4465-123">[Lista sites raiz][]</span><span class="sxs-lookup"><span data-stu-id="f4465-123">[List root sites][]</span></span>            | <span data-ttu-id="f4465-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="f4465-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="f4465-125">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="f4465-125">[Search for sites][]</span></span>           | <span data-ttu-id="f4465-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="f4465-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="f4465-127">[Seguir site][]</span><span class="sxs-lookup"><span data-stu-id="f4465-127">[Follow site][]</span></span>                | <span data-ttu-id="f4465-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="f4465-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="f4465-129">[Deixar de seguir site][]</span><span class="sxs-lookup"><span data-stu-id="f4465-129">[Unfollow site][]</span></span>              | <span data-ttu-id="f4465-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="f4465-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="f4465-131">[Listar sites seguidos][]</span><span class="sxs-lookup"><span data-stu-id="f4465-131">[List followed sites][]</span></span>        | <span data-ttu-id="f4465-132">POST /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="f4465-132">POST /me/followedSites</span></span>

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


## <a name="properties"></a><span data-ttu-id="f4465-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4465-145">Properties</span></span>

| <span data-ttu-id="f4465-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f4465-146">Property name</span></span>            | <span data-ttu-id="f4465-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4465-147">Type</span></span>               | <span data-ttu-id="f4465-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4465-148">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="f4465-149">**id**</span><span class="sxs-lookup"><span data-stu-id="f4465-149">**id**</span></span>                   | <span data-ttu-id="f4465-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4465-150">string</span></span>             | <span data-ttu-id="f4465-151">O [identificador exclusivo](#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="f4465-151">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="f4465-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4465-152">Read-only.</span></span>
| <span data-ttu-id="f4465-153">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="f4465-153">**createdDateTime**</span></span>      | <span data-ttu-id="f4465-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4465-154">DateTimeOffset</span></span>     | <span data-ttu-id="f4465-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4465-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f4465-157">**description**</span><span class="sxs-lookup"><span data-stu-id="f4465-157">**description**</span></span>          | <span data-ttu-id="f4465-158">string</span><span class="sxs-lookup"><span data-stu-id="f4465-158">string</span></span>             | <span data-ttu-id="f4465-159">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="f4465-159">The descriptive text for the site.</span></span>
| <span data-ttu-id="f4465-160">**eTag**</span><span class="sxs-lookup"><span data-stu-id="f4465-160">**eTag**</span></span>                 | <span data-ttu-id="f4465-161">string</span><span class="sxs-lookup"><span data-stu-id="f4465-161">string</span></span>             | <span data-ttu-id="f4465-p103">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4465-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="f4465-164">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f4465-164">**displayName**</span></span>          | <span data-ttu-id="f4465-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4465-165">string</span></span>             | <span data-ttu-id="f4465-p104">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4465-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="f4465-168">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f4465-168">**lastModifiedDateTime**</span></span> | <span data-ttu-id="f4465-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4465-169">DateTimeOffset</span></span>     | <span data-ttu-id="f4465-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4465-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f4465-172">**name**</span><span class="sxs-lookup"><span data-stu-id="f4465-172">**name**</span></span>                 | <span data-ttu-id="f4465-173">string</span><span class="sxs-lookup"><span data-stu-id="f4465-173">string</span></span>             | <span data-ttu-id="f4465-174">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="f4465-174">The name / title of the item.</span></span>
| <span data-ttu-id="f4465-175">**root**</span><span class="sxs-lookup"><span data-stu-id="f4465-175">**root**</span></span>                 | <span data-ttu-id="f4465-176">[root][]</span><span class="sxs-lookup"><span data-stu-id="f4465-176">[root][]</span></span>           | <span data-ttu-id="f4465-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4465-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="f4465-179">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="f4465-179">**sharepointIds**</span></span>        | <span data-ttu-id="f4465-180">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f4465-180">[sharepointIds][]</span></span>  | <span data-ttu-id="f4465-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4465-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f4465-183">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="f4465-183">**siteCollection**</span></span>       | <span data-ttu-id="f4465-184">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="f4465-184">[siteCollection][]</span></span> | <span data-ttu-id="f4465-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4465-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="f4465-188">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="f4465-188">**webUrl**</span></span>               | <span data-ttu-id="f4465-189">string (url)</span><span class="sxs-lookup"><span data-stu-id="f4465-189">string (url)</span></span>       | <span data-ttu-id="f4465-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4465-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="f4465-192">propriedade do id</span><span class="sxs-lookup"><span data-stu-id="f4465-192">id property</span></span>
<span data-ttu-id="f4465-193">Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="f4465-193">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="f4465-194">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="f4465-194">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="f4465-195">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="f4465-195">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="f4465-196">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="f4465-196">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="f4465-197">O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:</span><span class="sxs-lookup"><span data-stu-id="f4465-197">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="f4465-198">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="f4465-198">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="f4465-199">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="f4465-199">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="f4465-200">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="f4465-200">Relationships</span></span>

| <span data-ttu-id="f4465-201">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="f4465-201">Relationship name</span></span> | <span data-ttu-id="f4465-202">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4465-202">Type</span></span>                             | <span data-ttu-id="f4465-203">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4465-203">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="f4465-204">**analytics**</span><span class="sxs-lookup"><span data-stu-id="f4465-204">**analytics**</span></span>     | <span data-ttu-id="f4465-205">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="f4465-205">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="f4465-206">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="f4465-206">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="f4465-207">**columns**</span><span class="sxs-lookup"><span data-stu-id="f4465-207">**columns**</span></span>       | <span data-ttu-id="f4465-208">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="f4465-208">Collection([columnDefinition][])</span></span> | <span data-ttu-id="f4465-209">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="f4465-209">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="f4465-210">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="f4465-210">**contentTypes**</span></span>  | <span data-ttu-id="f4465-211">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="f4465-211">Collection([contentType][])</span></span>      | <span data-ttu-id="f4465-212">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="f4465-212">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="f4465-213">**drive**</span><span class="sxs-lookup"><span data-stu-id="f4465-213">**drive**</span></span>         | <span data-ttu-id="f4465-214">[drive][]</span><span class="sxs-lookup"><span data-stu-id="f4465-214">[drive][]</span></span>                        | <span data-ttu-id="f4465-215">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="f4465-215">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="f4465-216">**drives**</span><span class="sxs-lookup"><span data-stu-id="f4465-216">**drives**</span></span>        | <span data-ttu-id="f4465-217">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="f4465-217">Collection([drive][])</span></span>            | <span data-ttu-id="f4465-218">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="f4465-218">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="f4465-219">**items**</span><span class="sxs-lookup"><span data-stu-id="f4465-219">**items**</span></span>         | <span data-ttu-id="f4465-220">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="f4465-220">Collection([baseItem][])</span></span>         | <span data-ttu-id="f4465-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="f4465-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f4465-223">**lists**</span><span class="sxs-lookup"><span data-stu-id="f4465-223">**lists**</span></span>         | <span data-ttu-id="f4465-224">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="f4465-224">Collection([list][])</span></span>             | <span data-ttu-id="f4465-225">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="f4465-225">The collection of lists under this site.</span></span>
| <span data-ttu-id="f4465-226">**pages**</span><span class="sxs-lookup"><span data-stu-id="f4465-226">**pages**</span></span>         | <span data-ttu-id="f4465-227">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="f4465-227">Collection([sitePage][])</span></span>         | <span data-ttu-id="f4465-228">O conjunto de páginas na lista SitePages no site.</span><span class="sxs-lookup"><span data-stu-id="f4465-228">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="f4465-229">**sites**</span><span class="sxs-lookup"><span data-stu-id="f4465-229">**sites**</span></span>         | <span data-ttu-id="f4465-230">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="f4465-230">Collection([site][])</span></span>             | <span data-ttu-id="f4465-231">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="f4465-231">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="f4465-243">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4465-243">JSON representation</span></span>

<span data-ttu-id="f4465-244">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="f4465-244">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="f4465-245">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="f4465-245">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
