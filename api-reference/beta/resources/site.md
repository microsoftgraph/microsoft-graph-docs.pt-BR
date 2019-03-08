---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d2fbdcb870d86efb983de1e3ba75154b6e15f619
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481857"
---
# <a name="site-resource-type"></a><span data-ttu-id="068d1-102">tipo de recurso do site</span><span class="sxs-lookup"><span data-stu-id="068d1-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="068d1-103">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="068d1-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="068d1-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="068d1-104">Methods</span></span>

| <span data-ttu-id="068d1-105">Método</span><span class="sxs-lookup"><span data-stu-id="068d1-105">Method</span></span>                         | <span data-ttu-id="068d1-106">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="068d1-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="068d1-107">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="068d1-107">[Get root site][]</span></span>              | <span data-ttu-id="068d1-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="068d1-108">GET /sites/root</span></span>
| <span data-ttu-id="068d1-109">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="068d1-109">[Get site][]</span></span>                   | <span data-ttu-id="068d1-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="068d1-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="068d1-111">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="068d1-111">[Get site by path][]</span></span>           | <span data-ttu-id="068d1-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="068d1-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="068d1-113">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="068d1-113">[Get site for a group][]</span></span>       | <span data-ttu-id="068d1-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="068d1-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="068d1-115">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="068d1-115">[Get analytics][]</span></span>              | <span data-ttu-id="068d1-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="068d1-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="068d1-117">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="068d1-117">[Get activities by interval][]</span></span> | <span data-ttu-id="068d1-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="068d1-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="068d1-119">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="068d1-119">[List pages][]</span></span>                 | <span data-ttu-id="068d1-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="068d1-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="068d1-121">[Lista sites raiz][]</span><span class="sxs-lookup"><span data-stu-id="068d1-121">[List root sites][]</span></span>            | <span data-ttu-id="068d1-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="068d1-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="068d1-123">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="068d1-123">[Search for sites][]</span></span>           | <span data-ttu-id="068d1-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="068d1-124">GET /sites?search={query}</span></span>

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


## <a name="properties"></a><span data-ttu-id="068d1-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="068d1-134">Properties</span></span>

| <span data-ttu-id="068d1-135">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="068d1-135">Property name</span></span>            | <span data-ttu-id="068d1-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="068d1-136">Type</span></span>               | <span data-ttu-id="068d1-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="068d1-137">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="068d1-138">**id**</span><span class="sxs-lookup"><span data-stu-id="068d1-138">**id**</span></span>                   | <span data-ttu-id="068d1-139">string</span><span class="sxs-lookup"><span data-stu-id="068d1-139">string</span></span>             | <span data-ttu-id="068d1-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="068d1-p101">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="068d1-142">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="068d1-142">**createdDateTime**</span></span>      | <span data-ttu-id="068d1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="068d1-143">DateTimeOffset</span></span>     | <span data-ttu-id="068d1-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="068d1-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="068d1-146">**description**</span><span class="sxs-lookup"><span data-stu-id="068d1-146">**description**</span></span>          | <span data-ttu-id="068d1-147">string</span><span class="sxs-lookup"><span data-stu-id="068d1-147">string</span></span>             | <span data-ttu-id="068d1-148">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="068d1-148">The descriptive text for the site.</span></span>
| <span data-ttu-id="068d1-149">**eTag**</span><span class="sxs-lookup"><span data-stu-id="068d1-149">**eTag**</span></span>                 | <span data-ttu-id="068d1-150">string</span><span class="sxs-lookup"><span data-stu-id="068d1-150">string</span></span>             | <span data-ttu-id="068d1-p103">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="068d1-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="068d1-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="068d1-153">**displayName**</span></span>          | <span data-ttu-id="068d1-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="068d1-154">string</span></span>             | <span data-ttu-id="068d1-p104">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="068d1-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="068d1-157">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="068d1-157">**lastModifiedDateTime**</span></span> | <span data-ttu-id="068d1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="068d1-158">DateTimeOffset</span></span>     | <span data-ttu-id="068d1-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="068d1-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="068d1-161">**name**</span><span class="sxs-lookup"><span data-stu-id="068d1-161">**name**</span></span>                 | <span data-ttu-id="068d1-162">string</span><span class="sxs-lookup"><span data-stu-id="068d1-162">string</span></span>             | <span data-ttu-id="068d1-163">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="068d1-163">The name / title of the item.</span></span>
| <span data-ttu-id="068d1-164">**root**</span><span class="sxs-lookup"><span data-stu-id="068d1-164">**root**</span></span>                 | <span data-ttu-id="068d1-165">[root][]</span><span class="sxs-lookup"><span data-stu-id="068d1-165">[root][]</span></span>           | <span data-ttu-id="068d1-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="068d1-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="068d1-168">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="068d1-168">**sharepointIds**</span></span>        | <span data-ttu-id="068d1-169">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="068d1-169">[sharepointIds][]</span></span>  | <span data-ttu-id="068d1-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="068d1-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="068d1-172">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="068d1-172">**siteCollection**</span></span>       | <span data-ttu-id="068d1-173">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="068d1-173">[siteCollection][]</span></span> | <span data-ttu-id="068d1-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="068d1-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="068d1-177">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="068d1-177">**webUrl**</span></span>               | <span data-ttu-id="068d1-178">string (url)</span><span class="sxs-lookup"><span data-stu-id="068d1-178">string (url)</span></span>       | <span data-ttu-id="068d1-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="068d1-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="068d1-181">Relações</span><span class="sxs-lookup"><span data-stu-id="068d1-181">Relationships</span></span>

| <span data-ttu-id="068d1-182">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="068d1-182">Relationship name</span></span> | <span data-ttu-id="068d1-183">Tipo</span><span class="sxs-lookup"><span data-stu-id="068d1-183">Type</span></span>                             | <span data-ttu-id="068d1-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="068d1-184">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="068d1-185">**analytics**</span><span class="sxs-lookup"><span data-stu-id="068d1-185">**analytics**</span></span>     | <span data-ttu-id="068d1-186">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="068d1-186">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="068d1-187">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="068d1-187">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="068d1-188">**columns**</span><span class="sxs-lookup"><span data-stu-id="068d1-188">**columns**</span></span>       | <span data-ttu-id="068d1-189">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="068d1-189">Collection([columnDefinition][])</span></span> | <span data-ttu-id="068d1-190">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="068d1-190">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="068d1-191">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="068d1-191">**contentTypes**</span></span>  | <span data-ttu-id="068d1-192">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="068d1-192">Collection([contentType][])</span></span>      | <span data-ttu-id="068d1-193">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="068d1-193">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="068d1-194">**drive**</span><span class="sxs-lookup"><span data-stu-id="068d1-194">**drive**</span></span>         | <span data-ttu-id="068d1-195">[drive][]</span><span class="sxs-lookup"><span data-stu-id="068d1-195">[drive][]</span></span>                        | <span data-ttu-id="068d1-196">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="068d1-196">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="068d1-197">**drives**</span><span class="sxs-lookup"><span data-stu-id="068d1-197">**drives**</span></span>        | <span data-ttu-id="068d1-198">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="068d1-198">Collection([drive][])</span></span>            | <span data-ttu-id="068d1-199">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="068d1-199">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="068d1-200">**items**</span><span class="sxs-lookup"><span data-stu-id="068d1-200">**items**</span></span>         | <span data-ttu-id="068d1-201">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="068d1-201">Collection([baseItem][])</span></span>         | <span data-ttu-id="068d1-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="068d1-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="068d1-204">**lists**</span><span class="sxs-lookup"><span data-stu-id="068d1-204">**lists**</span></span>         | <span data-ttu-id="068d1-205">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="068d1-205">Collection([list][])</span></span>             | <span data-ttu-id="068d1-206">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="068d1-206">The collection of lists under this site.</span></span>
| <span data-ttu-id="068d1-207">**pages**</span><span class="sxs-lookup"><span data-stu-id="068d1-207">**pages**</span></span>         | <span data-ttu-id="068d1-208">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="068d1-208">Collection([sitePage][])</span></span>         | <span data-ttu-id="068d1-209">O conjunto de páginas na lista SitePages no site.</span><span class="sxs-lookup"><span data-stu-id="068d1-209">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="068d1-210">**sites**</span><span class="sxs-lookup"><span data-stu-id="068d1-210">**sites**</span></span>         | <span data-ttu-id="068d1-211">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="068d1-211">Collection([site][])</span></span>             | <span data-ttu-id="068d1-212">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="068d1-212">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="068d1-224">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="068d1-224">JSON representation</span></span>

<span data-ttu-id="068d1-225">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="068d1-225">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="068d1-226">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="068d1-226">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/site.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
